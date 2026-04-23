# uts_strukturdataa_P2
# Fungsi Rekrusif
Fungsi rekursif adalah teknik pemrograman di mana sebuah fungsi memanggil dirinya sendiri secara langsung maupun tidak langsung untuk menyelesaikan masalah. Fungsi ini memecah masalah kompleks menjadi sub-masalah yang lebih kecil, mengulangi proses hingga mencapai kondisi berhenti (base case) agar tidak terjadi perulangan tak terbatas.

Untuk UTS part 2 pada mata kuliah Struktur Data ini, kita disuruh untuk membuat deret Fibonacci dengan menggunakan fungsi rekrusif. </br>
</br> </br>

## Deskripsi tugas
Barisan Fibonacci  0, 1, 1, 2, 3, 5, 8, 13, 21, …. Dapat dinyatakan secara rekursif sebagai berikut:
<img width="294" height="128" alt="2" src="https://github.com/user-attachments/assets/157b1bbe-a247-4c29-93f2-9c8ac7edd53e" />
buat sebuah program Java yang dapat mencetak deret Fibonacci hingga suku ke-n menggunakan pendekatan rekursif
</br> </br>

## Code
```
package UTS;
import java.util.Scanner;

public class Fungsi_Rekrusif {
    public static void main(String[] args) {
        Scanner suku = new Scanner(System.in);   
        System.out.print("Masukkan Jumlah Suku Fibonacci : ");
        int n = suku.nextInt();
        
        System.out.print("Deret Fibonacci hingga Suku ke-" + n + " adalah ");
        for (int i = 0; i <= n; i++) {
            System.out.print(fibonacci(i));
            if (i < n) {
                System.out.print(" ");
            }
        }
        suku.close();
    }
    public static int fibonacci(int n) {
        if (n <= 1) {
            return n;
        }
        return fibonacci(n - 1) + fibonacci(n - 2);
    }
}
```
</br> </br>

## Output
Jika user memasukkan n = 6
<img width="674" height="114" alt="Screenshot 2026-04-23 185820" src="https://github.com/user-attachments/assets/ed38a5dd-2545-44f9-9597-5dab0410ab0f" />

Jika user memasukkan n = 8
<img width="814" height="140" alt="Screenshot 2026-04-23 185748" src="https://github.com/user-attachments/assets/4c0c7510-a4fa-4bb5-9a52-962cf608950d" />

Jika user memasukkan n = 5
<img width="629" height="107" alt="Screenshot 2026-04-23 185715" src="https://github.com/user-attachments/assets/c3881b60-a9d1-465d-b148-7ff42ce3ef76" />
