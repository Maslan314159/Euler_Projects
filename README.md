# Euler_Projects
"""
Problem_1:
1'den 10'a kadar olan sayılar içerisinden 3 veya 5'in katı olan sayılar
{3,5,6,9} kümesinin elemanlarıdır ve bu sayıların toplamı 3+5+6+9=23'tür.
Bu bilgiyi örnek alarak 1'den 1000'e kadar olan sayılar içinden 3 veya 5'in katı
olan sayıların toplamını bulunuz.

"""
liste_1 = [i for i in range(1000)
          if i % 3 == 0]
liste_2 = [j for j in range(1000)
          if j % 5 == 0]
liste_3 = [k for k in range(1000)
          if (k % 3 == 0 and k % 5 == 0)]

toplam_1 = sum(liste_1)
toplam_2 = sum(liste_2)
toplam_3 = sum(liste_3)

sonuc = toplam_1 + toplam_2 - toplam_3

print(" 0 ile 1000 arasında 3'e tam bölünen sayıların toplamı"
      " {}'dir.".format(toplam_1))

print(" 0 ile 1000 arasında 5'e tam bölünen sayıların toplamı"
      " {}'dir.".format(toplam_2))

print(" 0 ile 1000 arasında 3'e veya 5'etam bölünen sayıların toplamı"
      " {}'dir.".format(toplam_3))

print(" 0 ile 1000 arasında 3'e veya 5'e tam bölünen sayıların toplamı"
      " {}'dir.".format(sonuc))
