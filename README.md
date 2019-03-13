# Modul7-PHP
Jawab :
1.
$host = "localhost";
$db = "db_universitas";
$uname = "root";
$pass = "";

$connect = mysqli_connect($host, $uname, $pass, $db);

2.
Ada beberapa cara Untuk membuat database pada phpMysql :
a.Pertama membuat dengan menggunakan kode pada vcs , atom, dll. jadi membuatnya dengan kode
kodenya :
$sql = " CREATE DATABASE profile";

b.Kedua membuatnya manual dengan cara membuka localhost admin dan membuatnya dengan menual

3.
    $sql = "SELECT * FROM user";
    $result = $koneksi->query($sql);
      foreach($result as $result)
        $id = $result["id"];
        $nama = $result["nama"];
        $role = $result["role"];
        $availability = $result["availability"];
        $age = $result["age"];
        $location = $result["location"];
        $experience = $result["years_expereience"];
        $email = $result["email"];
        echo "id : ".$id." nama : ".$nama." role : ".$role;
        
4.
  $id_dosen = $_POST['id'];
  $nama_dosen = $_POST['nama_dosen'];
  $telp = $_POST['telp'];

  $query ="UPDATE dosen SET nama_dosen = '$nama_dosen', telp = '$telp' WHERE id = '$id_dosen'";

  $result = mysqli_query($connect, $query);

  $num = mysqli_affected_rows($connect);

5.
$id_dosen = $_GET['id'];

$query = "DELETE FROM dosen WHERE id = $id_dosen";

$result = mysqli_query($connect, $query);

$num = mysqli_affected_rows($connect);


![alt text](https://github.com/GhufronAndriansyah/Modul7-PHP/blob/master/Modul7(1).png)
![alt text](https://github.com/GhufronAndriansyah/Modul7-PHP/blob/master/Modul7(2).png)
![alt text](https://github.com/GhufronAndriansyah/Modul7-PHP/blob/master/Modul7(3).png)
![alt text](https://github.com/GhufronAndriansyah/Modul7-PHP/blob/master/Modul7(4).png)
![alt text](https://github.com/GhufronAndriansyah/Modul7-PHP/blob/master/Modul7(5).png)
![alt text](https://github.com/GhufronAndriansyah/Modul7-PHP/blob/master/Modul7(6).png)
![alt text](https://github.com/GhufronAndriansyah/Modul7-PHP/blob/master/Modul7(7).png)
![alt text](https://github.com/GhufronAndriansyah/Modul7-PHP/blob/master/Modul7(8).png)
![alt text](https://github.com/GhufronAndriansyah/Modul7-PHP/blob/master/Modul7(9).png)
![alt text](https://github.com/GhufronAndriansyah/Modul7-PHP/blob/master/Modul7(10).png)
