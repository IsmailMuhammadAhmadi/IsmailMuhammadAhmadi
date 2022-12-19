# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		      : Ismail Muhammad Ahmadi
<br>NIM		        : 1227050062	
<br>Jurusan		    : [Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
<br>Array dua dimensi adalah sebutan untuk array yang penomoran index-nya menggunakan 2 buah angka. Analogi lain adalah matriks. Matrixs Merupakan kumpulan-kumpulan bilangan yang disusun secara baris (vertikal) dan kolom (horizontal) bisa disebut juga array dua dimensi (multi-dimensional). Transpose Matriks adalah memperoleh sebuah matriks dengan cara menukar baris menjadi kolom dan kolom menjadi baris dari sebuah matriks. Dalam matematika, matriks terdiri dari kolom dan baris. Kembali, untuk menentukan nilai dari sebuah matriks, kita harus sebut secara berpasangan seperti baris 1 kolom 1, atau baris 2 kolom 3, dst. Konsep seperti inilah yang menjadi dasar dari array 2 dimensi. Untuk membuat array 2 dimensi di dalam bahasa C++, caranya tulis 2 kali tanda kurung siku setelah nama variabel, 
<br> seperti contoh berikut:
<br> int arr[2][2];  
Untuk UAS kali ini kami diminta membuat 2 buah program yaitu program pertama adalah membuat array 2 dimensi dengan baris , kolom dan nilai nya di input lalu ditukarkan antara kolom dan baris sedangkan program ke dua digunakan untuk mencari nilai yang dapat di bagi 3, 7, dan 5.

## Source Code
Program Membuat Tukar Kolom Menjadi Baris dan Baris Menjadi Kolom

      #include <iostream>
      using namespace std;

      int main()
      {
        cout << "^Nama  : Ismail Muhammad Ahmadi^" << endl;
        cout << "^NIM   : 1227050062^ " << endl;
        cout << "^Kelas : IF-B^" << endl;
        cout << "==========================================" << endl;
        cout << "^Program C++ Input Matriks 2 Dimensi^" << endl;
        cout << "==========================================" << endl;
        cout << endl;

        int matriks[100][100];
        int jum_baris, jum_kolom, i, j;

        cout << "Input jumlah baris matriks: ";
        cin >> jum_baris;

        cout << "Input jumlah kolom matriks: ";
        cin >> jum_kolom;
        cout << endl;

        // proses input array
        for(i = 0; i < jum_baris ; i++){
          for(j = 0; j < jum_kolom; j++){
            cout << "Baris " <<i+1<<", kolom "<<j+1<< " = ";
            cin >> matriks[i][j];
          }
          cout << endl;
        }
        for(i = 0; i < jum_baris ; i++){
          cout << endl;
          for(j = 0; j < jum_kolom; j++){
            cout << matriks[i][j];
          }
          cout << endl;
        }
        for(i = 0; i < jum_kolom ; i++){
          cout << endl;
          for(j = 0; j < jum_baris; j++){
            cout << matriks[j][i];
          }
          cout << endl;
        }
        return 0;
      }

Program Menampilkan Bilangan Yang Habis Dibagi 3, 5, Dan 7.

      #include <iostream>
      using namespace std;

      const int MAX_ROWS = 100;
      const int MAX_COLS = 100;

      int main()
      {
        cout << "^Nama  : Ismail Muhammad Ahmadi^" << endl;
        cout << "^NIM   : 1227050062^ " << endl;
        cout << "^Kelas : IF-B^" << endl;
        cout << "==========================================" << endl;
        cout << "^Program C++ Input Matriks 2 Dimensi No.2^" << endl;
        cout << "==========================================" << endl;
        cout << endl;

        int array[MAX_ROWS][MAX_COLS];
        int rows, cols;

        cout << "Masukkan jumlah baris array: ";
        cin >> rows;
        cout << "Masukkan jumlah kolom array: ";
        cin >> cols;

        cout << "Masukkan elemen-elemen array: " << endl;
        for (int i = 0; i < rows; i++) {
          for (int j = 0; j < cols; j++) {
            cin >> array[i][j];
          }
        }

        cout << "Bilangan yang habis dibagi 3, 5, dan 7: " << endl;
        for (int i = 0; i < rows; i++) {
          for (int j = 0; j < cols; j++) {
            if (array[i][j] % 3 == 0 && array[i][j] % 5 == 0 && array[i][j] % 7 == 0) {
              cout << array[i][j] << " ";
            }
          }
        }

        return 0;
      }
## Output
![Screenshot (72)](https://user-images.githubusercontent.com/120998345/208373807-1b090e78-484a-4477-bf87-ca2a5d6e8dc5.png)
![Screenshot (73)](https://user-images.githubusercontent.com/120998345/208373875-6cac570e-d9e9-4874-8f98-2ba497a59727.png)

