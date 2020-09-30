<!DOCTYPE html>
<html>
<head>
    <title>Mencari Data</title>
</head>
<body>
    <form action="http://localhost/tugas/array.php" method="post">
    Silahkan Masukan Nama : <input type="text" name="nama">
    <input type="submit" name="tombol" value="kirim">
    </form>
<br>
<br>
    </body>
</html>


<?php
if(isset($_POST['nama'])){

$nama = $_POST['nama'];

echo "Nama Yang anda cari : $nama <br>";

$user = array(
    array(
        "nama"          => "Arsene Lupin",
        "nik"           => "1234",
        "jenis_kelamin" => "male",
        "tgl_lahir"     => "1902-03-23"
    ),
    array(
        "nama"          => "Sherlock Holmes",
        "nik"           => "4321",
        "jenis_kelamin" => "male",
        "tgl_lahir"     => "1812-01-11"
    ),
    array(
        "nama"          => "Irene Adler",
        "nik"           => "7890",
        "jenis_kelamin" => "female",
        "tgl_lahir"     => "1232-04-13"
    )
);

$i=0;
$a=0;

foreach($user as $x){
if(strtoupper($x["nama"]) == strtoupper($nama)){
$i=1;
$a=$x;
} 
}

if($i){

echo "Ditemukan<br>";
echo "Data dari $nama adalah <br>";
echo "NIK: ".$x["nik"]."<br>";
echo "KELAMIN: ".$x["jenis_kelamin"]."<br>";
echo "TGL LAHIR: ".$x["tgl_lahir"]."<br>";

} else{
echo "[".$nama."] <b>Tidak Ketemu</b> <br>";
}

}

?>
