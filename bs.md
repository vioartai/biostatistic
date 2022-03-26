# biostatistic
import time
while True:

    print("  ---  HİPOTEZ TESTLERİ  ---  ")

    print("Uygulamak istediğiniz testi seçin. (1/2/3/4)\n")
    tests = "1- z ve T değeri hesabı. \n2- Student t testi. (Henüz çalışmıyor :D) \n3- Güven sınırları. (Henüz çalışmıyor :D) \n4- Test istatistiği hesaplaması. (Henüz çalışmıyor :D)\n\n"

    for letters in tests:
        time.sleep(0.02)
        print(letters, end = "")

    seçenek = int(input("Seçtiğiniz test: "))
    if seçenek == 1:
        
        print("\n\n -- Z VE T DEĞERİ HESABI -- \n ")

        değer = float(input("Veri seti içinde hesaplamak istediğiniz değeri girin: "))
        ortalama = float(input("Veri setinin ortalamasını giriniz: "))
        sp = float(input("Dağılımın standart sapmasını giriniz: "))

        z = (değer - ortalama)/sp
        t = (10 * z) + 50

        print("\n")
        print("z değeri : ", z)
        print("T değeri : ", t, "\n")

    time.sleep(0.5)
    print("Yeniden başlatılıyor...\n")
    time.sleep(1)

"""
    elif seçenek == 2:
        pass
       
    elif seçenek == 3:
        pass

    elif seçenek == 4:
        pass


"""

