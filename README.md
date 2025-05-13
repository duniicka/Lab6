def calculate(A, n):
    total = 0
    for i in range(n):
        for j in range(i + 1, n):
            if A[i][j] > 0:
                total += A[i][j]
    return total

n = 4
A = [
    [1, 2, 3, 4],
    [0, 5, 6, 7],
    [0, 0, 8, 9],
    [0, 0, 0, 10]
]

total = calculate(A, n)
print(f"The sum of positive elements above the main diagonal is: {total}")
