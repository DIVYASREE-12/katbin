# katbin
first_input = input().rstrip().split()
n = int(first_input[0])
m = int(first_input[1])
matrix = [input() for _ in range(n)]

result = ' '.join(''.join(c * (c.isalnum() or ' ' == c) for c in matrix[i]) for i in range(m)).replace('  ', ' ')

print(result)
