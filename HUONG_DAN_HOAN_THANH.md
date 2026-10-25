# Huong dan hoan thanh bai 4

Kho nay co lich su Git thuc, gom commit, merge, conflict da xu ly, rebase, stash, tag va trang HTML.

## Can thuc hien tren may Windows va GitHub
1. Cai Git for Windows, mo Git Bash va chup `git --version`.
2. Cau hinh danh tinh THUC: `git config --global user.name "Nguyen Dai Loc"` va `git config --global user.email "EMAIL_GITHUB_CUA_BAN"`. Email trong kho mau la gia tri gia, can doi khi thuc hanh.
3. Giai nen ZIP, mo Git Bash tai thu muc; `git log --oneline --graph --all`, `git status`, `git branch -a`.
4. Tao repository RONG tren GitHub: `ThucHanhGit_NguyenDaiLoc` (KHONG tick tao README).
5. Chay `git remote add origin https://github.com/Loc273-clod/ThucHanhGit_NguyenDaiLoc.git` va `git push -u origin main --tags`.
6. Clone sang thu muc khac: `git clone https://github.com/Loc273-clod/ThucHanhGit_NguyenDaiLoc.git ../git-clone-demo`; kiem tra `git remote -v` va `git branch -r`.
7. Tao thay doi README tren giao dien GitHub; ve may chay `git pull`.
8. Tao nhanh PR: `git switch -c feature/pr-demo`, sua file, `git add .`, `git commit -m "PR demo"`, `git push -u origin feature/pr-demo`; mo Pull Request tren GitHub.
9. Tao Release v1.0.0 trong tab Releases (tag da tao trong kho).
10. GitHub Settings > Pages > Deploy from a branch > main / (root). Cho Pages xuat ban, lay URL.
11. SSH: `ssh-keygen -t ed25519 -C "EMAIL_GITHUB_CUA_BAN"`; them public key vao GitHub Settings > SSH and GPG keys; `ssh -T git@github.com`. KHONG chia se private key.
12. Remote thu hai: can URL repo do giang vien cung cap; `git remote add upstream URL`; `git remote -v`.
13. Submodule: can repo duoc phep su dung; `git submodule add URL vendor/example`; `git submodule status`; commit.
14. Thuc hanh bisect, reflog, revert tren ban clone THU NGHIEM, khong viet lai lich su main da push. Chup man hinh cac lenh va ket qua.

## Cau lenh bo sung cho phan D
- `git show HEAD:README.md` (xem tep o commit)
- `git log -- README.md` (lich su tep)
- `git grep Git` (tim chuoi)
- `git rm --cached TEN_TEP` (ngung theo doi nhung giu tep tren may)
- `git restore --source=HEAD~1 -- README.md` (lay tep tu commit truoc, xem lai truoc khi commit)
- `git revert SHA` (hoan tac commit an toan tren remote)
- `git reflog` (tim commit da mat khoi branch)
- `git bisect start`, `git bisect bad`, `git bisect good SHA_TOT`, `git bisect reset` (can lich su loi mau)

## Minh chung
- Tep `MINH_CHUNG_LENH.txt` la transcript lenh thuc su chay trong moi truong mau, KHONG phai anh chup Windows cua sinh vien.
- Chup man hinh Git Bash, GitHub repository, Pull Request, Release va Pages tren tai khoan cua ban de nop.
