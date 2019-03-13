# Modul7_LavedaNafisArshanda
1. Berikan contoh kode keneksi untuk ke database pd php?
Contoh kode koneksi : $connect = mysqli_connect($host, $uname, $pass, $db);

2. Bagaimana cara anda membuat database pada phpMySQl!
Langkah 1 : Buka Localhost PhpMyadmin
Langkah 2 : Klik new
Langkah 3 : Create databae, beri nama database
Langkah 4 : Klik Create

3. Berikan code query untuk menampilkan sebuah data yang ada pada ke database?
contoh kode query :
$query = "SELECT * FROM dosen";
$result = mysqli_query($connect, $query);
$num = mysqli_num_rows($result);

4. Berikan code query untuk mengupdate sebuah data yang ada pada ke database?
Contoh kode query :
$query = "UPDATE dosen SET nama_dosen = '$nama_dosen', telp = '$telp' WHERE id_dosen = $id_dosen";
$result = mysqli_query($connect, $query);
$num = mysqli_affected_rows($connect);


5. Berikan code query untuk menghapus sebuah data yang ada pada ke database?
Contoh kode query :
$query = "DELETE FROM dosen WHERE id_dosen = $id_dosen";
$result = mysqli_query($connect, $query);
$num = mysqli_affected_rows($connect);
