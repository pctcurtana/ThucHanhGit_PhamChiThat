# ThucHanhGit_HoTen

## 1. Mục đích
Repository này ghi lại quá trình thực hành Git và GitHub: quản lý phiên bản
cục bộ, làm việc với nhánh, cộng tác trên GitHub, khôi phục lịch sử và các
công cụ nâng cao.

- Sinh viên: Họ Tên - MSSV: xxxxxxx
- Lớp: xxxxxxx

## 2. Cách sử dụng
```bash
git clone https://github.com/TenBan/ThucHanhGit_HoTen.git
cd ThucHanhGit_HoTen
git log --oneline --graph --all
```
- Xem lịch sử commit và nhánh bằng lệnh `git log` ở trên.
- Trang GitHub Pages: https://TenBan.github.io/ThucHanhGit_HoTen/
- Release: https://github.com/TenBan/ThucHanhGit_HoTen/releases

## 3. Các kỹ thuật đã thực hiện

### A. Git cơ bản
- Cài đặt và kiểm tra Git (`git --version`)
- Cấu hình `user.name`, `user.email`
- Khởi tạo repository (`git init`)
- Tạo README.md và commit đầu tiên (`git add`, `git commit`)
- Kiểm tra trạng thái (`git status`)
- Xem lịch sử (`git log`, `git log --oneline`)
- So sánh thay đổi (`git diff`)
- Tạo `.gitignore`
- Sửa commit gần nhất (`git commit --amend`)

### B. Nhánh và hợp nhất
- Tạo và chuyển nhánh (`git switch -c`)
- Commit trên nhánh tính năng
- Hợp nhất nhánh (`git merge`)
- Xóa nhánh đã hợp nhất (`git branch -d`)
- Xem sơ đồ nhánh (`git log --graph --all`)
- Đổi tên nhánh (`git branch -m`)
- Giải quyết xung đột hợp nhất
- Rebase và so sánh với merge

### C. GitHub và cộng tác
- Tạo repository trên GitHub
- Kết nối remote và push (`git remote add`, `git push`)
- Clone repository (`git clone`)
- Xem nhánh remote (`git branch -r`)
- Pull thay đổi (`git pull`)
- Tạo Pull Request
- Tạo tag và Release (v1.0.0)
- Xuất bản GitHub Pages
- Thiết lập SSH key
- Làm việc với nhiều remote

### D. Kiểm tra, khôi phục, tìm lỗi
- Khôi phục thay đổi chưa commit (`git restore`, `git restore --staged`)
- Khôi phục tệp từ commit trước (`git restore --source`)
- Ngừng theo dõi tệp nhưng giữ lại (`git rm --cached`)
- Xem nội dung tệp tại commit cụ thể (`git show hash:file`)
- Xem lịch sử của một tệp (`git log -- file`)
- Tìm chuỗi trong repository (`git grep`)
- Tìm commit gây lỗi (`git bisect`)
- Khôi phục commit đã xóa (`git reflog`)
- Hoàn tác commit đã push (`git revert` so với `git reset`)

### E. Công cụ nâng cao
- Tạm cất thay đổi (`git stash`)
- Tạo Git alias (`st`, `lg`, `co`, `cm`)
- Sử dụng submodule (`git submodule add`)
- Dùng alias để rút gọn lệnh
- Hoàn thiện repository (README)

## 4. Ghi chú
- `revert` an toàn cho nhánh chung; `reset` + force push viết lại lịch sử remote nên có rủi ro.
- Không `amend` hoặc `rebase` các commit đã push và chia sẻ.
