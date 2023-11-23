| fungsi | keterangan |
| --- | --- |
| `git add .` | menambahkan semua file dari working directory ke staging area |
| `git add <nama file>` | menambahkan file dari working directory ke staging area |
| `git commit -m "isi commit"` | menyimpan perubahan di staging area ke local repository |
| `git push origin main` | mengirim perubahan dari local repository ke remote repository `origin/main` |
| `git push -u origin main` | mengirim perubahan dari local repository ke remote repository `origin/main` sekaligus mengeset upstream dari branch tersebut untuk menuju ke `origin/main`. Fungsi ini dijalankan ketika kalian ingin menambahkan branch baru yang ada di local repository ke remote repository. Jika upstream sudah pernah di set maka kalian bisa mengirim perubahan dengan cara `git push` |
| `git pull origin main` | menarik perubahan yang ada di remote repository `origin/main` ke local repository. Fungsi ini adalah gabungan dari fungsi `git fetch` + `git merge` atau `git rebase`. Jika upstream sudah pernah di set ketika `git push -u`, maka kalian bisa menarik perubahan dengan cara `git pull` |
