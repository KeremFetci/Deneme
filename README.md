# Deneme

from random import randint

random1 = randint(1, 100)
random2 = randint(1,100)
random3 = randint(1,100)
sayac = 0

TümRandom = random1 + random2 + random3

while True:
    sayac +=1
    sayi = int(input("1 ile random arasında bir sayı girin 0 çıkıştır, 10000 Verileri almadır):"))
    if sayi == 0:
        print("Oyundan Çıkış Yaptınız!")
        break
    elif sayi == 10000:
        print("Sayı: ",TümRandom)
        print("Sayaç Metre :",sayac)
        break
    elif sayi < TümRandom:
        print("Daha büyük bir sayı girin")
        continue
    elif sayi > TümRandom:
        print("Daha Küçük bir sayı yazın")
        continue
    else:
        print("Rastgele Seçilen sayı {0}!".format(TümRandom)) #.format string'e çevirmektir burada randomu metine çeviriyor
        print("Tahmin Sayınız {0}".format(sayac))

