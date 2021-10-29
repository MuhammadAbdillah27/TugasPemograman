# Aplikasi Input data siswa


import os
import sys

class Mahasiswa :
             nim=' '
             nama=' '

pilih = 0
datasiswa = []

def menu () :
    os.system('cls')
    print ("Menu Aplikasi Data Siswa") ;
    print ("20*"-")
    print ("1. Input Data Siswa")
    print ("2. Tampilkan Data Siswa")
    print ("3. Update Dta Siswa")
    print ("4. Hapus Data Siswa")
    print ("5. Author")
    print ("6. Keluar Aplikasi")
    pilih = int(input ("Masukkan pilihan anda")
    if pilih == 1 :
        pilih1 ()
        menu ()
    elif pilih == 2:
        tampil ()
        input ("kembali menu utama")
        menu()
    elif pilih == 3:
        index_update=-1
        tampil ()
        id edit = int(input("Input Nim yang akan di update "))
        for a in range (0, len(datasiswa)):
            if id_edit == dataSiswa [a].nim:
                index update = a
                break
        if(index_update > -1) :
                    print ("INPUT DATA YANG DI UPDATE ")
                    siswa = Mahasiswa()
                    siswa.nim = (int(input("masukkan nim : ")))
                    siswa.nama = (input("masukkan nama siswa : "))
                    dataSiswa[index_update] = siswa
                    print("berhasil update data siswa")
        else : print("nim tidak ditemukan")
        input("kembali menu utama")
         menu()
    elif pilih ==4:
        os.system('cls')
        tampil()
        index_delete=-1
        id_hapus + int(input("input nim yang akan dihapus : ")
        for a in range(0, len(dataSiswa)):
            if id edit == dataSiswa[a].nim:
                        index_update = a 
                        break
        if(index_delete > -1) :
            del dataSiswa[index_delete]
            print("Data Telah di hapus")
        else : print("nim tidsk ditemukan")
        input("kembali menu utama")
        menu()
    elif pilih == 5 :
        author()
        input("\n\n kembali menu utama")
        menu()
    elif pilih == 6 :
        sys.exit()

def tampil() :
    os.system('cls') ;
    print("DATA MAHASISWA")
    for data in dataSiswa:
        print("Nim : "+str(data.nim))
        print("Nama : "+data.nama)
        print("------------")

def author():
    os.system('cls')
    print("Pakde Edri")
    print("UnHar")

def pilih1()
    ulang = 'Y'
    while ulang in('y'. 'y') :
        os.system('cls')
        siswaBaru + Mahasiswa()
        print("INPUT DATA MAHASISWA ")
        siswaBaru.nim = (int(input("masukkan nim : ")))
        siswaBaru.nama = (input("masukkan nama siswa : "))
        dataSiswa.append(siswaBaru)
        ulang = input("Apakah Anda Ingin Mengulang (Y/ T)? ")

menu()
