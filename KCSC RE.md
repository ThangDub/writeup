### POKEMON HOF PANEL LEVEL 1

# 1.Phân tích:

Từ Hint của bài ta biết được việc lợi dụng 'Insecure Deserialization' để giải challenge, cụ thể ở đây là của PHP

Qua HInt, ta đồng thời cũng biết được rằng ta có thể diều chỉnh các thuộc tính của hàm `O:4:"User"` , hàm `s:10:"isLoggedIn"` và hàm `b:1` để lấy được Flag

![image](https://github.com/ThangDub/writeup/assets/86946032/0509efeb-24eb-46de-8824-ee9a7877f4c4)

# 2. Khai thác:
Sử dụng Burpsuit và sau đó sử dụng chức năng 'intercept' của Burp , ta phát hiện được thuộc tính hàm `b:` đang được để bằng 0 và đổi nó về giá trị 1

![image](https://github.com/ThangDub/writeup/assets/86946032/38413b6d-fdcf-435b-b395-96c80a5bbd33)

# 3.Flag:
Sau khi thay đổi Flag xuất hiện

`KCSC{n0w_y0u_kn0w_s3r1al1z3_f0m4rt}`



