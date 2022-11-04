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

## React Proptypes

Kegunaan menggunakan proptypes itu untuk check typing (mengecek tipe data). Istilah proptypes sendiri terdiri dari dua makna yaitu prop dan types. Alhasil ia lebih tepatnya akan digunakan untuk mengecek tipe data sebuah props. Manfaat dari propstype ini sebagai bentuk pencegahan agar data yang kita kirimkan ke child selalu sesuai dengan apa yang diinginkan.

- Install terlebih dahulu extension prop-typesnya di folder project, dengan perintah: npm install prop-types.

![contohPerintahInstall](/images/Screenshot%202022-11-01%20152240.png)

- Bentuk penulisan codenya

![contohPenulisanCode](/images/Screenshot%202022-11-01%20153051.png)

Didalam proptypes yang dicontohkan, prop name dan age ia hanya akan diterima/diakses jika type data yang dikirimkan berupa string dan number saja, selain itu maka tampilkan pesan error.

![contohLainnya](/images/Screenshot%202022-11-01%20160821.png)


## React Router

Sederhananya kegunaan dari react router ini untuk melakukan perpindahan page. Penulisan react router (routingan) terdapat di file App.jsx dan nantinya akan disambungkan ke component page yang telah dibuat. Terdiri dari istilah path, element, dan link. Sebelum menggunakan react router kita diharuskan untuk menginstalnya terlebih dahulu:

- Install react router: npm install react-router-dom@6

![contohInstall](/images/Screenshot%202022-11-02%20192754.png)

Setelah melakukan proses install selanjutnya ke tahap codingan.

- Pada tahap codingan kita akan melakukan import BroserRouter ke file main.jsx. Yang akan dijadikan pembungkus component App. Artinya yang dapat menikmati layanan routing hanyalah component App.

![settinganAwaldiMainjsx](/images/Screenshot%202022-11-02%20193759.png)

- Selanjutnya membuat folder Pages didalam folder src. Kemudian membuat dua buah file, serta import extensi router dom ke file App.

![contohGambarMembuatFolderdanFile](/images/Screenshot%202022-11-02%20215659.png)

![contohGambarCodinganApp](/images/Screenshot%202022-11-02%20215751.png)

- Tahapan berikutnya kita tulislah perintah perpindahan halamannya di file App. Dengan menambahkan tag Route didalam tag Routes. Isi bagian path sebagai alamat/keterangan perpindahan pagenya, beserta element untuk diisikan element page yang dituju.

![contohPenulisanPerintahRoute](/images/Screenshot%202022-11-02%20220823.png)

Dengan path berupa "/" saja merupakan tanda sebagai page utama.

- Kemudian kita akan menggunakan tag Link dengan membuatnya sebagai navbar, untuk button berpindah page. property "to" diisikan alamatnya seperti yang ada diproperty path.

![contohNavbardenganTagLink](/images/Screenshot%202022-11-02%20221924.png)

Hasilnya:

![hasilSinglePage](/images/Screenshot%202022-11-02%20222420.png)

Jenis lain dari React Routing:

1. Params Router yaitu kondisi ketika kita ingin mengirimkan sebuah parameter/data di dalam routingan.

- Membuat alamat Route baru, bedanya ditambahkan id pada pathnya karena kita akan mengirim data idnya juga.

![contohPembuatanRoute](/images/Screenshot%202022-11-02%20230130.png)

- Membuat data di Homepage dan function onsubmitnya. Penggunaan useNavigate berfungsi untuk menagkap id yang dikirimkan, jika kita menggunakan tag Link ia tidak bisa digunakan ketika kita ingin menyisipkan code logic.

![contohPenulisanMenambahData](/images/Screenshot%202022-11-02%20230316.png)

- Membuat loopingan data menggunakan method map.

![contohLoopinganData](/images/Screenshot%202022-11-02%20230353.png)

- Selanjutnya kita ingin menampilkan data yang lebih detail di halaman detail page dengan memanfaatkan idnya.

![ContohmembuatDatadiDetailPage](/images/Screenshot%202022-11-02%20232716.png)

- Membuat looping. Apabila idnya sama dengan yang klik maka datanya tampilkan.

![membuatLoopingCondition](/images/Screenshot%202022-11-02%20232800.png)

2. Nested Route yaitu routingan halamannya bercabang. Contoh: ketika kasusnya seperti ini "/about/student".

- Kita setting syntax penulisannya di file App. Kemudian kita bungkus file yang ingin dibuat nested route. Apabila file yang dijadikan nested  route terdapat property "index" mengartikan bahwa page itu yang akan pertama kali di akses.

![contohPenulisanNestedRoute](/images/Screenshot%202022-11-03%20072111.png)

- Selanjutnya kita import perintah "Outlet" di file AboutPage yang menjadi parent/pembungkus dari nested routenya.

![memanggilOutlet](/images/Screenshot%202022-11-03%20072154.png)


## React Redux

Redux merupakan library yang berdiri sendiri yang dapat berkolaborasi dengan berbagai framework dan UI layer. Termasuk didalamnya yaitu React, Angular, Vue, Ember dan Vanila JS. Meskipun Redux dan React bisa melakukan kolaborasi bersama, mereka tetap memiliki sisi kemandiriannya masing-masing. React redux resminya adalah redux UI yang ada di library react. Dsn jika ingin menggunakan redux dan react secara bersamaan harus juga menggunakan React Redux untuk menggabungkan kedua libray tersebut. 

Alasan menggunakan redux ketika terjadi kasus dimana setiap komponen parent dan child memerlukan data/properti yang sama untuk ditampilkan sehingga terjadi yang dinamakan props drilling. Apakah prop drilling itu? Prop drilling adalah situasi ketika data yang sama dikirim di hampir setiap level karena persyaratan tertentu sampai di level akhir. Berikut Penggambarannya:

![contohPenggambaranPropDrilling](/images/propdrilling.png)

Nah ketika sebuah data itu melakukan perubahan, maka otomatis kita harus mengubah disetiap komponen yang menggunakan data tersebut.

Sehingga perlulah adanya State Management yaitu:

- Redux
- Content
- Jotai
- Zustand

Awal kita membuat menggunakan redux berikut tahapannya:

- Menginstal terlebih dahulu library redux dan react-redux

![perintahInstalReduxdanReactRedux](/images/Screenshot%202022-11-04%20124254.png)

- Membuat component yang dibutuhkan

![componentsYangdibutuhkan](/images/Screenshot%202022-11-04%20124327.png)

![tampilanPenulisandiApp](/images/Screenshot%202022-11-04%20124405.png)

- Membuat store/tempat penampungnya

![membuatFiledanFolder](/images/Screenshot%202022-11-04%20144023.png)

![membuatStoreRedux](/images/Screenshot%202022-11-04%20143801.png)

- selanjutnya membuat Reducernya (rak penyimpanan di gudang)

![membuatFiledanfolder](/images/Screenshot%202022-11-04%20153917.png)

![membuatReducerStore](/images/Screenshot%202022-11-04%20154008.png)

- Memberitahu bahwa store yang telah dibuat telah tersedia untuk component yang ingin menggunakan

![membuatProviderRedux](/images/Screenshot%202022-11-04%20154221.png)

- Ambil data dari store, menggunakan syntax useSelector

![membuatUseSelector](/images/Screenshot%202022-11-04%20154403.png)

- membuat perintah action yang dibutuhkan guna merubah data

![membuatFileAction](/images/Screenshot%202022-11-04%20154823.png)

![membuatAction](/images/Screenshot%202022-11-04%20154600.png)

- Ubah data menggunakan useDispatch

![membuatuseDispatch](/images/Screenshot%202022-11-04%20154950.png)

## React Async Action with Middleware and Thunk

Thunk middleware untuk Redux. Memungkinkan menulis fungsi dengan logika didalamnya serta dapat berintarksi dengan Redux store seperti dispatch dan getState method. Alasan menggunakan Middleware yaitu kita dapat melakukan pembaharuan data/action tidak hanya disatu kondep sederhana synchronous saja. Melainkan dengan menggunakan Middleware dapat memperluas kemampuan mengakses store serta dapat berinteraksi dengan storenya.

Thunk merekomendasi middleware untuk efek logika dengan redux sederhana, termasuk logika sinkron kompleks yang memerlukan akses ke penyimpanan, dan logika asinkron sederhana seperti permintaan AJAX.

Untuk membuat Thunk sederhana step by stepnya:

- Download terlebih dahulu redux-thunk. Dengan perintah: npm install redux-thunk
- Selanjutnya seperti bisa kita create tahapan-tahapan membaut code redux sesuai dengan kebutuhan.
- Selanjutnya pada file store kita menambahkan applyMiddleware(thunk)

![contohPenulisandenganapplyMidleware](/images/Screenshot%202022-11-04%20221042.png)

untuk penjelasan yang lebih detailnya bisa klik [ini](https://github.com/reduxjs/redux-thunk)


