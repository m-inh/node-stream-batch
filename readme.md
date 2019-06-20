# Stream vs Batch

## Yêu cầu

Các bài tập yêu cầu hiện thực hóa bằng 2 cách (stream và batch), viết trong 2 tệp server tương ứng (`batch-server.js`, `stream-server.js`)

1. Viết API đọc vào tệp `truyen-kieu.txt` trả về khổ thơ đã được format 6, 8. Hiển thị ở phía client giống như sau:
```
Tà tà bóng ngả về tây,
Chị em thơ thẩn dan tay ra về.
Bước dần theo ngọn tiểu khê,
Lần xem phong cảnh có bề thanh thanh.
Nao nao dòng nước uốn quanh,
Dịp cầu nho nhỏ cuối ghềnh bắc ngang.
Sè sè nấm đất bên đàng,
Dàu dàu ngọn cỏ nửa vàng nửa xanh.
Rằng: Sao trong tiết thanh minh,
Mà đây hương khói vắng tanh thế mà?
Vương Quan mới dẫn gần xa:
Đạm Tiên nàng ấy xưa là ca nhi.
Nổi danh tài sắc một thì,
Xôn xao ngoài cửa hiếm gì yến anh.
....
```

2. Viết API phục vụ tĩnh (serve static) một tệp lớn bất kì trên 1Gb (ví dụ: `https://speed.hetzner.de/1GB.bin`), sau đó thực hiện đánh giá 2 cách làm với tiêu chí sau:
- Thời gian tải đối với 1 request
- Thực hiện gọi 10 request đồng thời, thống kê số lượng request thành công và thất bại, thời gian tải tương ứng với mỗi request

## Nộp bài tập

Tạo issue với định dạng: 
- Tiêu đề: Họ và tên
- Nội dung: Đường dẫn tới repo chứa mã nguồn