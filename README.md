# UAS-SOAL-KE-1-RIZQI
INI ADALAH PROGRAM UAS RIZQI NO 1
int main() {
  /*
  Nama : Rizqi Maulana Abdul Aziz
  NIM : 41037002241021
  prodi : Teknik Elektro
  Semester : 2
  */
 
  int A, B, N, D, r, G, L;
 
  // Step 1: Start
  printf("Program GCD dan LCM\n");
  printf("==================\n");
 
  // Step 2: Read two numbers A, B
  printf("Masukkan bilangan pertama (A): ");
  scanf("%d", &A);
  printf("Masukkan bilangan kedua (B): ");
  scanf("%d", &B);
 
  // Step 3 If (A>B) THEN N=A, D=B ELSE N=B, D=A
  if (A > B) {
  N = A;
  D = B;
  } else {
  N = B;
  D = A;
  }
  // Step 4 r = N/D
  r = N % D;
 
  // Step5 WHILE (r !=0) DO N=D, D=r, r=N%D DONE
  while (r != 0) {
  N = D;
  D = r;
  r = N % D;
  }
 
  // Step 6 G = D (GCD)
  G = D;
 
  // Step 7: L = (A*B)/G (LCM)
  L = (A * B) / G;
 
  // Step 8: Display G, L
  printf("\nHasil perhitungan:\n");
  printf("GCD (G) = %d\n", G);
  printf("LCM (L) = %d\n", L);
 
  // Step 9Stop
  printf("Program selesai.\n");
  return 0;
 
}


INi adalah jawaban no 2

#include <stdio.h>
#include <string.h>

int main() {
   char kata[100];
   int i, j, palindrome = 1;

   printf("Masukkan kata atau angka: ");
   scanf("%s", kata);

   int panjang = strlen(kata);
   i = 0;
   while (i < j) {
       if (kata[i] != kata[j]) {
           palindrome = 0;
           break;
       }
       i++;
       j--;
   }

   if (palindrome)
       printf("%s adalah palindrome.\n", kata);
   else
       printf("%s bukan palindrome.\n", kata);

   return 0;
}

