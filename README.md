# insertionsort
Swift eğitimimin bir parçası olan Algoritma ve Veri Yapıları insertion sort konusu icin bir örnek çözüm.


### **Insertion Sort Aşamaları**

Verilen dizi:

**[22,27,16,2,18,6]**

Insertion Sort, diziyi soldan sağa sıralarken her elemanı uygun yerine yerleştirir.

1. İlk eleman (22) zaten sıralı kabul edilir.
    
    **[22,27,16,2,18,6]**
    
2. 27, 22’den büyük olduğu için olduğu yerde kalır.
    
    **[22,27,16,2,18,6]**
    
3. 16, 27’den küçük olduğu için, 27’nin soluna yerleşir. 22’den de küçük olduğu için 22’nin soluna geçer.
    
    **[16,22,27,2,18,6]**
    
4. 2, 27’den küçük → 22’den küçük → 16’dan küçük, en başa yerleşir.
    
    **[2,16,22,27,18,6]**
    
5. 18, 27’den küçük → 22’den küçük → 16’dan büyük, 16 ile 22 arasına yerleşir.
    
    **[2,16,18,22,27,6]**
    
6. 6, 27’den küçük → 22’den küçük → 18’den küçük → 16’dan küçük, 2’den büyük. 2 ile 16 arasına yerleşir.
    
    **[2,6,16,18,22,27]**
    

### **Big-O Gösterimi**

Insertion Sort’un en kötü durumda (tersten sıralı dizi) ve ortalama durumda karmaşıklığı:

**O(n²)**

En iyi durumda (dizi zaten sıralıysa) karmaşıklık:

**O(n)**

### **Time Complexity ve 18 Sayısının Durumu**

Dizi sıralandıktan sonra:

**[2,6,16,18,22,27]**

- **Average Case**: Aradığımız sayı genellikle ortalarda olur. 18, dizinin ortalarına yakın olduğu için **average case**kapsamına girer.

---

## **Selection Sort İlk 4 Adım**

Verilen dizi:

**[7,3,5,8,2,9,4,15,6]**

Selection Sort, her adımda en küçük elemanı bulup, ilgili sıraya koyar.

1. **Adım:** En küçük eleman **2**, en başa (7 ile yer değiştirir).
    
    **[2,3,5,8,7,9,4,15,6]**
    
2. **Adım:** En küçük eleman **3**, zaten ikinci sırada. Değişim yok.
    
    **[2,3,5,8,7,9,4,15,6]**
    
3. **Adım:** En küçük eleman **4**, üçüncü sıradaki 5 ile yer değiştirir.
    
    **[2,3,4,8,7,9,5,15,6]**
    
4. **Adım:** En küçük eleman **5**, dördüncü sıradaki 8 ile yer değiştirir.
    
    **[2,3,4,5,7,9,8,15,6]**
    

Buradan sonra algoritma devam ederek diziyi tamamen sıralar.
