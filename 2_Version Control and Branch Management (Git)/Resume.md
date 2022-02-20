# Version control and Branch management ( Git )

## A. Apa itu versioning?
  - Versioning adalah mengatur versi dari source program
  - Versioning berguna untuk mengatur file source program yang memiliki banyak version, 
  dengan versioning, kita dapat mengatur atau membuat rapih versi-versi dari source program kita.

## B. Sejarah Vesion control system
  * Single User
    * SCCS  - 1972  : UNIX Only
    * RCS   - 1982  : Cross Platform , Text only
  * Centralized
    * CVS         - 1986  : File focus
    * Perforce    - 1995
    * Subversion  - 2000  : Track directory structur
    * Microsoft Team foundation server
  * Distributed
    * Git       - 2005
    * Mercurial - 2005
    * Bazaar    - 2005
    
## C. Git dan GitHub
  * Git adalah salah satu Version Control System populer yang digunakan oleh banyak para developer
  untuk mengembangkan Software secara bersama-sama ( Real World Collaboration )
  * Git "Terdistribusi" bukan "Tersentralisasi", maksudnya adalah 
  setiap orang dapat memiliki codenya masing-masing, mengeditnya masing-masing itulah maksud dari "Terdistribusi"
  apabila terdapat problem pada server, setiap orang akan memiliki backupnya masing-masing, itulah maksud dari "bukan tersentralisasi"
  * Git dapat mentracking seluruh perubahan yang terjadi pada repository.
  * Melakukan Commit berarti melakukan perubahan dan akan tercatat pada history Git.
  
## D. Setting up Git
  * Setting nama dan email dapat menggunakan
    * git config --global user.name "nama"
    * git config --global user.email "username@gmail.com"
  * Untuk mengecek nama dan email dapat menggunakan
    * git config --list
  * Untuk melakukan clone terhadap repository dapat menggunakan
    * git clone (code SSH/HTTPS)
  * Untuk memindahkan source program kedalam Staging Area dari Working Area
    * git add .
    * git add (directory)
    * git add index.html
  * Untuk memindahkan melakukan Commit source program kedalam repository
    * git commit -m "massage"
    * gunakan massage yang tidak membuat ambigu atau bingung developer
  * Jangan lupa apabila setelah di commit untuk melakukan push
    * git push origin
    
## E. Branching
  * Berfungsi untuk melindungi main/master project kita pada saat melakukan perubahan/collaborative project
  * Untuk melihat daftar branch
    * git branch --list
  * Untuk membuat branch baru dapat menggunakan
    * git branch (nama branch)
  * Untuk menghapus branch dapat menggunakan
    * git branch -d (nama branch)
  * Untuk push branch agar tersimpan di repository dapat menggunakan
    * git push -u origin (nama branch)
  * Untuk berpindah branch dapat menggunakan
    * git checkout (nama branch)
    * checkout juga dapat digunakan untuk berpindah version / commit / stash
    * git checkout (code commit)
  * Untuk menggabungkan branch dapat menggunakan
    * git merge (nama branch)
    * Direkomendasikan untuk tidak melakukan merge terhadap main/master branch apabila pada saat developing belum selesai/tuntas 100%
    * Sangat direkomendasikan untuk melakukan perubahan di branch developer dan apabila ada penambahan fitur, direkomendasikan untuk membuat branch baru, apabila sudah selesai, lakukan push kedalam developer, apabila penambahan fitur di approve, maka akan dilakukan merge kepada branch developer.
    
   
   
