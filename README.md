# BÀI 2: HTTP SERVER ĐẦU TIÊN
## 1. Mục tiêu
- Tạo HTTP Server bằng Node.js thuần.
- Sử dụng module http để tạo máy chủ.
- Chạy máy chủ tại cổng 3000.
- Truy cập localhost:3000 và hiển thị tên sinh viên.
## 2. Tạo chương trình myFirstNode.js

Tạo file myFirstNode.js và nhập code:

```javascript
var http = require('http');

http.createServer(function (req, res) {
  res.writeHead(200, {'Content-Type': 'text/html; charset=utf-8'});
  res.end('Hello World!<br>Tôi Là Phạm Hoàng Hải!');
}).listen(3000);
```

## 3. Cách chạy chương trình

Mở Terminal tại thư mục chứa file myFirstNode.js, nhập lệnh:

```bash
node myFirstNode.js
```

## 4. Truy cập HTTP Server

Mở trình duyệt và truy cập:

text
http://localhost:3000

## 5. Kết quả chạy chương trình
```text
Hello World!
Tôi Là Phạm Hoàng Hải!
```

## 6. Kết luận

Đã tạo và chạy thành công HTTP Server đầu tiên bằng Node.js, sử dụng module http để khởi tạo máy chủ tại cổng 3000. Truy cập thành công địa chỉ localhost:3000 và hiển thị nội dung Hello World cùng tên sinh viên trên trình duyệt.
