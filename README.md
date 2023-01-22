# InsertionSortProject

1.Hafta ödevi

Insertion Sort yaparken n elemanlı bir dizi içinde en küçük sayı seçilerek ilk sıraya yazılır. En küçük sayının eski yerine ilk sıradaki sayı yazılır.
En küçük eleman en başa yazıldıkça listede sıralama yapılacak eleman sayısı azalır. n elemanlı bir dizi için n-1,n-2...,1 eleman kalıncaya kadar işlem devam ettirilir.

Aşağıdaki dizi için insertion sort yapalım.
[22,27,16,2,18,6]

1.adım:
Dizi içerisindeki en küçük değere sahip sayı seçilir. Bu dizide bu değer 2'dir ve ilk sıradaki 22 ile yerleri değiştirilir.
[2,27,16,22,18,6]

2.adım:
En küçük değer dizinin en başına yazıldığı için dizideki kalan kısım kontrol edilir. Kalan kısımda en küçük değer 6'dır. 6 ile hali hazırda 2.sırada yer alan 27 yer değiştirilir ve dizi aşağıdaki halini alır.
[2,6,16,22,18,27]

3. adım:
2 ve 6 küçükten büyüğe sıralandığı için dizinin o kısmına müdahele edilmez ve kalan sayılar içerisindeki en küçük sayı sorgulanır. Bu sayı 16'dır ve zaten büyükten küçüğe sıralandığında olması gereke 3. sıradadır.
[2,6,16,18,22,27]

4.adım: 
Listenin sıralı olmayan kısmı sorgulandığında en küçük sayı 18'dir ve 18 de olması gereken küçükten büyüğe sıralı yerindedir. Bu şekilde 1 adım daha bakıldığında 22 ve 27' de listede küçükten büyüğe olması gereken sıradadır. Insertion sort tamamlanmıştır. 
[2,6,16,18,22,27]


Big-O gösterimi:
Yukarıdaki insertion sort projesi n elemanlı bir dizi için n+(n-1)+(n-2)+...+1 olacak şekilde 1'den n'e kadar olan sayıların toplamıdır. Bu fonsiyonda (n^2+n)/2 formülüne tekabül etmektedir. Big-O Notation'da en büyük/domine eden fonksiyon alınır. Bu nedenle insertion sort'un time complexity'si, worst case senaryosu n^2'dir.


Time Complexity: 
Dizi sıralandıktan sonra 18 sayısı average case'e girer çünkü ortadaki elemandır.

[7,3,5,8,2,9,4,15,6]

1.adım:
[2,3,5,8,7,9,4,15,6]

2.adım:
[2,3,4,8,7,9,5,15,6]

3.adım:
[2,3,4,5,7,9,8,15,6]

4.adım:
[2,3,4,5,6,9,8,15,7]

