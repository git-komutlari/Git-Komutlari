### İnit

- **git init —>** ilk projeyi oluşturma.

### Add

- **git add * . -a —>** repoya dosya ekleme.

### Commit

- **git commit -m "First Commit" —>** snapshot almak için

### Amend

- **git amend —>** Son yapılan commiti geri alır.
- **git commit --amend —>** son yapılan commit üzerine ekler (yeni commit oluşturmaz).
- **git commit --amend -m "yeni mesaj" —>** son commitin mesajını değiştirir.

### Status

- **git status —>** durumu görmek için

### Push, Pull ve Clone

- **git push —>** uzak bilgisayara göndermek için.
- **git pull —>** uzak bilgisayardan çekmek için.
- **git clone —>** projeyi kopyalayarak çeker.

### Checkout

- **git checkout isim —>** isim adındaki brancha geçiş yapar.
- **git checkout -b isim2 —>** isim2 adında bir branch oluşturup direkt geçiş yapar.

### Rm

- **git rm —>** dosya ve klasör silmek için
- **git rm --cached name —>** Staged ortamına eklenmiş bir dosyanın takibinin bırakılması yani untracked (izlenmeyen) hale getirilmesi sağlayan komuttur.

### Diff ve Log

- **git diff —>** Değişiklikleri gösterir.
- **git diff log1 .. log2 [index.md](http://index.md/) —>** [index.md](http://index.md/) nin log1 ve log2 arasındaki değişiklikleri gösterir.
- **git log —>** tüm snapshotları gösterir.
- **git log -n 1 —>** son snapshotı gösterir 2 3 diye devam eder

### Revert

- **git revert lognumarasi —>** lognumarasi logu geri alır. Geri alma logunu geri alırsak eski haline döner.

### Reset

- **git reset --hard donmekistediginlog —>** dönmek istediğin yere kadar olan logları siler.

### Branch

- **git branch —>** Branchları gösterir.
- **git branch isim —>** "isim" adında bir branch oluşturur.
- **git branch -d isim2 —>** isim2 adlı branchi siler.

### Touch

- **touch [isim.md](http://isim.md/) —>** [isim.md](http://isim.md/) adında bir dosya oluşturdu.

### Stash

- **git stash —>** son commite kadar olan bölümü geçici olarak depolar ve son commite döner.
- **git stash list —>** stashları gösterir.
- **git stash clear —>** stash kaydını siler.
- **git stash pop —>** en üstteki kaydı geri getirir ve kaydı listeden siler.
- **git stash apply stash@{1} —>** 2. stash kaydına döner ama listeden silmez.
- **git stash drop stash@{0} —>** 1. stash kaydını siler.

### Merge

- **git merge branch_ismi —>** Master ile branch_ismi'ni birleştirir.
- **git merge --squash branch_ismi —>** Master ile branch_ismi'ni birleştirir fakat branch_ismi'nin commit geçmişini tek bir commit'de toplar. Geçmişin çok uzamasını engeller. Bunu yaptıktan sonra son bir commit daha yapmamızı bekler.
- **git merge --abort —>** Yapmakta olduğumuz merge'ü iptal eder.
- **git rebase branch_ismi —>** Değişiklikleri sanki ana branch'da yapmış gibi gösterir ve commit tarihçesine bir şey eklemez.
