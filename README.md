# palpi
def generate_fibonacci(n):
    if n <= 0:
        return []
    elif n == 1:
        return [0]
  
    series = [0, 1]
    for _ in range(2, n):
        series.append(series[-1] + series[-2])
    return series

# Example: Print first 10 numbers
print(generate_fibonacci(10))
