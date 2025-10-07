# Test-git
Các bước clone 1 dự án về:
B1: Tạo ssh key nếu chưa có:
    Mở terminal rồi chạy lệnh : ssh-keygen rồi cứ bấm enter đến khi xong
    Mở file C:/Users/<tên users>/.ssh/id_rsa.pub rồi copy toàn bọ nội dung file
B2: add ssh key vào tài khoản git
    Vào github chon icon profile ở góc trên bên phải
    Chọn setting > SSH and GPG keys > new SSH key
    Điền nội dung vừa copy vào mục key và điền vào mục title tùy ý
B3: git clone <Link ssh url>
    Link SSH lấy ở project trên github mục code màu xanh lá rồi chọn tab SSH trong đó sẽ thấy link ssh url

----------------------GIẢI THÍCH CÁC LỆNH GIT---------------------------
-git pull: kéo code mới nhất ở nhánh hiện tại về
-git push: Đẩy những commit chưa có trên remote của nhánh lên
-git checkout <Tên nhánh>: Chuyển sang nhánh <Tên nhánh>
-git checkout -b <Tên nhánh>: Tạo nhánh mới từ nhánh hiện tại và checkout sang nhánh mới đó
-git add .: add để commit tất cả các file đang thay đổi 
-git add file1 file2 file3 ...: add file1 file2 file3 ... để commit 
-git commit -m "Tên commit": commit những file đã được add vào một lịch sử
-git merge <tên nhánh>: Nhập nhánh <Tên nhánh> vào nhánh hiện tại
-git clone <ssh url hoặc https url>: kéo project về máy
-git log: Kiểm tra lịch sử nhánh hiện tại
-git log --oneline: Nếu có nhiều lịch sử thì dùng lệnh này để xem được nhiều hơn
-git status: Kiểm tra những file thay đổi
-git status --untracked-files=all: Kiểm tra những file thay đổi có đầy đủ đường dẫn
-git fetch: Cập nhật origin của nhánh hiện tại tức là nhánh hiện tại ở trên github 
-git log --graph --decorate --oneline --all: Xem lịch sử các nhánh bằng biểu đồ 