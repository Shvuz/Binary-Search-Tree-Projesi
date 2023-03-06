# Binary-Search-Tree-Projesi
Diziyi Binary Search Tree'ye dönüştürmek için ilk önce kök düğüm olarak ilk elemanı seçiyoruz. Daha sonra her bir elemanı sırayla BST'ye ekliyoruz. Ekleme işlemi, eklenecek elemanın kök düğümden büyük veya küçük olduğuna göre sağ veya sol alt ağaçlarda yapılır.

Kök düğüm: 7
5, 1, 8, 3, 6, 0, 9, 4, 2 elemanları sırayla eklenir:
5: Kökün solunda yer alır.
1: 5'in solunda yer alır.
8: Kökün sağına yer alır.
3: 5'in solunda yer alır ve 1'in sağına eklenir.
6: 5'in solunda yer alır ve 3'ün sağına eklenir.
0: 5'in solunda yer alır, 1'in soluna eklenir ve 3'ün soluna eklenir.
9: 8'in sağına yer alır.
4: 5'in solunda yer alır, 3'ün solunda yer alır ve 0'ın sağına eklenir.
2: 5'in solunda yer alır, 3'ün solunda yer alır ve 1'in soluna eklenir.
Bu aşamalar sonunda Binary Search Tree şu şekilde oluşur:

      7
    /   \
   5     8
  / \     \
 1   3     9
    / \   /
   0   6 4
        /
       2

Bu şekildeki bir BST'de arama işlemi, ağaçtaki elemanların sıralı olması sayesinde O(log n) zamanında yapılabilir.
