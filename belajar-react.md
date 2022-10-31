## Pengenalan: React

Jika sebelumnya kita dalam membuat web masih dengan cara manuadan dibantu dengan menggunakan DOM. Ternyata setelah dirasakan cara tersebut sangatlah tidak efektif dan terlalu banyak buang waktu dengan sia-sia. Keluhan yang terjadi ketika kita membuat codingan web dengan cara manual (DOM):

- bolak balik liat id dan dan class
- repot saat mau menggunakan event
- line jadi terlihat banyak, terus harus crete element dulu

diatas merupakan beberapa keluhannya. Dari situlah react diciptakan. Cara menginstal react:

1. Install terlebih dahulu nodeJs

![instalNodeJsversiterbaru](/images/Screenshot%202022-10-26%20063418.png)

2. Setelah terpasang kita chech terlebih dahulu yaitu dengan membuka gitbash perintahnya: node -v

![keadaanJikaSudahTerpasang](/images/Screenshot%202022-10-25%20212115.png)

Di web browser mechine yang digunakan untuk menjalankan javascript yaitu dinamakan v8. Dengan adanya nodeJs file javascript tidak lagi membutuhkan browser untuk dapat dijalankan. 

React diciptakan oleh facebook dan diperuntukkan bagi para programmer front end. Selain dari react terdapat library lainnya yaitu Angular dibuat Google, dan vue. Keuntungan menggunakan react:

- Membuat web dalam waktu yang cepat
- jika terdapat codingan web reusable kita cukup memanggilnya saja tanpa harus mengcopy ulang codingannya.

Sehingga kesimpulan apa itu react? react adalah library yang untuk membuat tampilan web.

3. Download react

![downloadReact](/images/Screenshot%202022-10-26%20071517.png)

4. Selanjutnya dicek terpasang reactnya tau belum menggunakan perintah: npm -v

![cekInstalReact](/images/Screenshot%202022-10-26%20071856.png)

5. Keadaan setelah selesai install react pada VSCode

![setelahInstalldiVSCode](/images/Screenshot%202022-10-26%20075346.png)

React menggunakan konsep SPA (Single Page Application) artinya hanya memiliki satu file html saja. React berinteraksi dengan DOM menggunakan konsep "REAL and Virtual DOM", jika sebelumnnya kita menggunakan manipulasi html menggunakan innerHTML maka itu akan langsung mengakses DOMnya. Namun di react ia menggunakan Virtual DOM sebagai perantara. Untuk menjalankan running file App yaitu menggunakan perintah: npm start

![hasildariNpmStart](/images/Screenshot%202022-10-26%20075729.png)

File App pada react berperan sebagai gerbang utama menampilkan berbagai komponen untuk ditampilkan pada browser. Pada App juga ia hanya mengizinkan satu element saja, jika terdapat dua element maka ia akan error. Mengakalinnya kita dapat menggunakan tag fragment(tag kosong).

Contoh dua element jadinya error:

![contohDuaElement](/images/Screenshot%202022-10-26%20080341.png)

Contoh penggunaan tag react fragment sebagai alternatif:

![penggunaanTagFragment](/images/Screenshot%202022-10-26%20080419.png)

## React Component
 
Pengertian dari react component yaitu salah satu cara untuk membagi UI kedalam satu-satuan kecil. Yang artinya di dalam satu page terdapat beberapa component yang bisa kita custom. Kondisi disaat menggunakan component ketika component tersebut bersifat reusable code (code yang digunakan pada page lainnya). Hal yang harus diperhatikan ketika penulisan function yaitu huruf pertama nama function harus huruf kapital. Penulisan class di react juga berbeda, jika sbelumnya kita cukup tulis saja "class" sedangkan react "className". Cara membuat Component react:

- Kita dapat membuat folder baru di dalam folder src, setelah itu membuat file js dengan nama filenya sesuai componen yang dibutuhkan.

![membuatFolderdiSrc](/images/Screenshot%202022-10-26%20173923.png)

- Setelah itu memebuat codingan function di dalam file home dan nama function menyesuaikan nama filenya. Lalu lakukan export function.

![membuatCodingandiHome](/images/Screenshot%202022-10-26%20174018.png)

- Kemudian memanggil function dan file kedalam file App, dengan cara mengimportnya.

![memanggilFunctiondanFilediApp](/images/Screenshot%202022-10-26%20173952.png)

## React Styling

- Kita bisa membuat folder component di src dan file jsx dengan nama file yang sama sesuai nama functionnya.

![membuatComponent](/images/Screenshot%202022-10-27%20080957.png)

- Selanjutnya membuat function sesuaikan namanya dengan nama file dan lakukan export

![membuatFunction](/images/Screenshot%202022-10-27%20081035.png)

- Kemudian kita akan melakukan styling di di file yang sudah disediakan yaitu App.css untuk class profile-container, profile-img dan profile-info

![membuatStyle](/images/Screenshot%202022-10-27%20081055.png)

- Setelah component sudah selesai dibuat maka saatnya melakukan import pada file App.jsx guna dapat ditampilkan pada browser

![importKeApp](/images/Screenshot%202022-10-27%20081115.png)

Setelah melakukan styling sederhana, kita juga dapat melakukannya menggunakan framework yaitu bootstrap. Berikut caranya:

- Kita bisa memasang bootstrap di file index.html. setelah dipasang maka kita bebas menggunakan template style dari bootstrap, namun ada beberapa penamaannya harus disesuaikan dengan format react.

![memasangBootstrap](/images/Screenshot%202022-10-29%20142846.png)

## React State dan Props

Dari yang dicontohkan diatas data yang ditampilkan pada file MemberInfo masihlah data statis. Kali ini kita akan membuatnya dinamis. Yaitu dengan menggunakan react state dan props. Pengertian State yaitu data yang ada didalam component, sedangkan props merupakan data yang diberikan.

Gambar 1

![gambarContohState](/images/Screenshot%202022-10-30%20155459.png)

Gambar 2

![gambarContohProps](/images/Screenshot%202022-10-30%20155536.png)

Pada gambar 1 merupakan contoh dari state, di state itu memberikan data berupa nama, umur dan info ke file component MemberInfo.jsx. Sehingga file MemberInfo.jsx merupakan sebuah props yang menerima data yang dikirimkan oleh file App.jsx, terlihat pada gambar 2.

Didalam state ada dua jenis kategori yaitu:

- Statefull Component ialah sebuah component yang tidak memiliki state didalamnya.
- Stateless Component ialah sebuah component yang tidak memiliki state.

## React Event

![contohPenulisanEvent](/images/Screenshot%202022-10-30%20172707.png)

Pada gambar diatas penulisan event disontohkan dua penulisan yang berbeda. Di button yang pertama contoh penulisan jika kita ingin menambahkan argument di fungsi dengan menggunakan onClick. Sedangkan di button kedua masih menggunakan event onClick yang hanya memanggil fungsinya tanpa arguments.

## React Lifecycle

Lifecycle atau diartikan dengan siklus hidup react ini,terbagi menjadi 3 kategori:

1. Mounting yaitu ketika suatu comopent ini ditampilkan
2. Update
3. Unmount yaitu kondisi componentnya menghilang.

dari ketiga siklus tersebut terdapat juga yang disebut efek samping. Istilah tersebut disebut "Side Effect".

![contohLifecycle](/images/Screenshot%202022-10-30%20203403.png)

Pada contoh diatas merupakan contoh dari siklus hidup mounting. Untuk membuat efek sampingnya itu menggunakan fungsi useEffect yang sudah disediakan oleh react. Proses eksekusinya:

1. React akan menjalankan function dulu
2. Setelah menjalankan function ia akan menjalankan yang ada di return
3. Kemudian baru akan menjalankan side effectnya.

## React Form

Seperti di form html, form react juga digunakan untuk mengambil atau mengcapture inputan data daru user untuk digunakan atau diolah kembali. Yang nantinya data tersebut akan disimpan ke server ketika user telah mengsubmit. Berikut contoh pembuatan formnya:

![contohForm](/images/Screenshot%202022-10-31%20205236.png)

Pada contoh diatas untuk bagian menampilkan formnya masih sama dengan cara membuat form pada html. Yang membedakan yaitu penulisan "for" pada label yang menjadi "htmlFor". Untuk mengambil setiap data inputannya kita harus membuat state disetiap kategori inputannya. Ketika menekan button submit ia akan menjalankan function handleSubmit.
