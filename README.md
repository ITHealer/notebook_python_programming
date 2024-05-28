# Learning python

### Git command

Push code len branch thong thuong:
1. git branch: xem minh dang branch nào
2. git branch -a: xem co bao nhieu branch dang o local cua minh.
Neu co het roi thi continue 3:
Neu chua thi download no ve:

	2.1. git fetch --all

	2.2. git branch -a : de check

	Muon pull branch nao ve de lam viec:
    
	2.3. git checkout -b main origin/man (vd branch main origin/... khi git branch -a se thay)

	Luu y la khi muon add 1 so file chinh sua hien tai vao branch moi pull ve thi copy file do 	bo cho khac chu khi pull ve minh k thay no nua phai mac cong pull lai branch cu cua minh. 	Sau do copy file muon add vao branch kia roi git add . (co the add file can add thoi)

	VD: git add ios/src/TTSCBackend.cpp (git status no se co ios/src/TTSCBackend.cpp) sau do 	check lai git status mau xanh la thanh cong) -> roi git commit -> git push origin -> done.

3. git status: xem nhung file nào thay doi (màu red) 
4. git checkout -b <tên> : de tao branch moi push code hien tai minh code lên 
5. git add  . 
6. git status: xem cac file (mau do) da thanh mau xanh chua (mau xanh la add done)
4. git commit -m ""
5. git push -u origin <ten branch moi tao>
______________________________________________________________________________________________

Connect cu can xoa va tao connect toi repo moi:
cd C:\Users\<username>\Desktop\my-project
git remote -v
# Output:
# origin  https://gitlab.com/<username>/<repo-name-old> (fetch)
# origin  https://gitlab.com/<username>/<repo-name-old> (push)

git remote rm origin
git remote add origin https://gitlab.com/<username>/<repo-name-new>
git checkout dev
git add .
git commit -m "Thay doi repo duoc remote"
git push origin dev
______________________________________________________________________________________________
Merge:
1. git branch: xem mình dang branch nào
2. git checkout -b <tên> : de tao branch moi push code hien tai minh code lên 
3. git add  .
4. git commit -m ""
5. git push -u origin <ten branch moi tao>

Truoc khi merge gi thi phai pull cai source minh muon merge nó o trang thai update moi nhat:
 
1. git checkout <ten branch muon merge>
2. git pull origin <ten branch muon merge>
Dam bao minh dang o branch ma minh muon merge thi moi merge
3. git branch 
4. git merge <merge branch code cua minh>

sau khi xu ly conflict:
git add .
git commit -m "merge branch <tên branch c? minh> into <ten branch merge vo>"
git log --oneline

check out ve lai branch cua minh 
git checkout <>
git merge <ten branch merge vao>
git push origin <branch cua minh>



