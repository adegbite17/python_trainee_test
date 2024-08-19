def sequence_output(seq):
    output = ''
    count = 0
    for char in seq:
        if char == '1':
            count += 1
            if count == 3:
                output += '1'
                count = 0
        else:
            output += '0'
            count = 0
    return output

input_seq = '0101101011101011011101101000111'
output = sequence_output(input_seq)
print(output)
