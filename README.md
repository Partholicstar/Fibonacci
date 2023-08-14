fib_series = [0, 1] # 0 and 1 are the initial default values
def fib(n):
    if n<= len(fib_series):
       return fib_series[n-1]

    else:
       next_number = fib(n-1)+fib(n-2)
       fib_series.append(next_number)
       print((next_number),end=' ')
       return next_number

n = int(input("Enter the value of n: "))
print(0, 1, end=" ") #initial default values
fib(n)
