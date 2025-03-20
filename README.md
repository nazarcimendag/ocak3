# 1'den 100'e kadar olan sayıları ekrana yazdırma
for sayi in range(1, 101):
    print(sayi)
# 1'den 100'e kadar olan sadece çift sayıları yazdırma
for sayi in range(1, 101):
    if sayi % 2 == 0:
        print(sayi)
# faktoriyel hesaplama
sayi = int(input("Faktöriyelini hesaplamak istediğiniz sayıyı girin: "))

faktoriyel = 1
for i in range(1, sayi + 1):
    faktoriyel *= i

print(f"{sayi}! = {faktoriyel}")
# 1'den 100'e kadar olan asal sayıları bulma
for sayi in range(2, 101):
    asal = True
    for i in range(2, int(sayi ** 0.5) + 1):
        if sayi % i == 0:
            asal = False
            break
    if asal:
        print(sayi)

