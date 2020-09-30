# praktikum3

Diberikan array campuran seperti di bawah ini:
$user = array(
  array(
    ‘nama’ 		=> ‘Arsene Lupin’, 
    ‘nik’			=> ‘1234’, 
    ‘jenis_kelamin’	=> ‘male’,
    ‘tgl_lahir’		=> ‘1902-03-23’), 
  array(
    ‘nama’ 		=> ‘Sherlock Holmes’, 
    ‘nik’			=> ‘4321’, 
    ‘jenis_kelamin’	=> ‘male’,
    ‘tgl_lahir’		=> ‘1876-08-16’), 
  array(
    ‘nama’ 		=> ‘Irene Adler’, 
    ‘nik’			=> ‘6789’, 
    ‘jenis_kelamin’	=> ‘female’,
    ‘tgl_lahir’		=> ‘1884-10-07’
  ),
);

Dari array tersebut, lakukan pencarian dengan menggunakan looping for dan foreach untuk mencari seorang user berdasarkan nama. Contoh, untuk mencari nama "Sherlock Holmes", ketika data array yang dilooping dan menemukan array yang elemen nama memiliki value Sherlock Holmes, program akan keluar dari looping. Jika keyword pencarian adalah "Watson", di mana datanya tidak ada di dalam arraym, program tidak akan pernah keluar dari looping.
