# Bài 1: Khởi tạo Local Repository và Cấu hình danh tính

## Các lệnh đã thực hiện

### 1. Khởi tạo repository
```bash
mkdir my-first-project && cd my-first-project
git init
```

### 2. Cấu hình danh tính (local)
```bash
git config --local user.name "Ten Cua Ban"
git config --local user.email "email-cua-ban@example.com"
```

### 3. Tạo tệp và đưa vào Staging Area
```bash
echo "# My First Project" > README.md
git add README.md
```

### 4. Commit đầu tiên
```bash
git commit -m "Initial commit: add README.md"
```

## Kết quả kiểm tra

### Cấu hình local
```
$ git config --local user.name
Ngo Quang Anh
$ git config --local user.email
ngoquanganh2003a@gmail.com
$ git config --local --list
```

### Lịch sử commit
```
$ git log --oneline
```

## Nhận xét
- Dùng `--local` để cấu hình chỉ áp dụng cho repository này, được lưu trong `.git/config`, không ảnh hưởng cấu hình toàn cục (`~/.gitconfig`).
- Luồng làm việc: Working Directory → `git add` → Staging Area → `git commit` → Repository.
