pengerjaan problem set yang ada di tlx pada bagian menentuan bilangan agak prima
n = int(input()) #input line bil interger
for i in range(n): # melakukan perulangan untuk meminta user daftar angka yang ingin di tentukan
    input_line = int(input())
    jumlah_faktor = 0 #jumlah faktor yang tersedia
    for j in range(1, int(input_line ** 0.5) + 1): #mengefiessi tle dengan akar N ini
        if input_line % j == 0:
            if j * j == input_line:
                jumlah_faktor += 1
            else:
                jumlah_faktor += 2
        if jumlah_faktor > 4:
            break
    if jumlah_faktor <= 4:
        print("YA")
    else:
        print("BUKAN")
