# Python-Temel-Proje


Flatten.py


"""
1- Write a function that flattens a list. Its elements can consist of multi-layered lists (such as [[3],2]) or non-scalar data. For example:
input: [[1,'a',['cat'],2],[[[3]],'dog'],4,5]
output: [1,'a','cat',2,3,'dog',4,5]
"""


a = [[1,'a',['cat'],2],[[[3]],'dog'],4,5]
a1 = []

def flatten(n):
    for i in n:
        if isinstance(i,list):
            flatten(i)
        else:
            a1.append(i)
flatten(a)
print(a1)



Reverse.py

@@ -0,0 +1,16 @@
"""
2- Verilen listenin içindeki elemanları tersine döndüren bir fonksiyon yazın. Eğer listenin içindeki elemanlar da liste içeriyorsa onların elemanlarını da tersine döndürün. Örnek olarak:
input: [[1, 2], [3, 4], [5, 6, 7]]
output: [[[7, 6, 5], [4, 3], [2, 1]]
"""


g = [[1, 2], [3, 4], [5, 6, 7]]
g.reverse()
for i in range(len(g)):
    (g[i]) = (g[i]) [::-1]

print(g)
