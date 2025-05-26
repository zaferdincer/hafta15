

def fibonacci(n):
    if n == 1 or n == 2:
        return 1
    else:
        return fibonacci(n-1) + fibonacci(n-2)

n = int(input("Sayı giriniz: "))
d = {}  
toplam = 0

for x in range(1, n+1):
    d[x] = fibonacci(x)
    print(f"sıralama: {x}, Fibonacci Değeri: {d[x]}")
    toplam += d[x]

print("Toplam:", toplam)
