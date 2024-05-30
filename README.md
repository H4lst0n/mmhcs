# mmhcs

## Chương 3: Mã hóa bất đối xứng
<br>

  ![image](https://github.com/H4lst0n/mmhcs/assets/91616280/9a9c53be-64e9-4abb-84b4-560164315f42)

### 1) Hãy trình bày đặc điểm chính của thuật toán mã hóa khóa công khai?. Vẽ sơ đồ minh họa quy trình mã hóa và giải mã của thuật toán mã hóa khóa công khai?.
<br>
- Mã hóa công khai ( hay gọi là mã hóa bất đối xứng ): là phương pháp mã hóa mà khóa sử dụng để mã hóa sẽ khác với khóa dùng để giải mã.
- Khóa dùng để giải mã hóa gọi là khóa công khai và khóa dùng để giải mã gọi là khóa bí mật.
- Tất cả mọi người đều có thể biết khóa công khai nhưng chỉ người nhận mới nắm giữ khóa bí mật nên mới có thể giải mã
<br>

### 2) Hãy trình bày về chứng thực trong mô hình mã hóa bất đối xứng?.
- Mã hóa bất đối xứng là các phương pháp mà quy trình mã hóa và giải mã sử dụng các khóa khác nhau
  <br>
  ![image](https://github.com/H4lst0n/mmhcs/assets/91616280/fc21b95c-bef9-44ae-a4ef-6afd9b13dbbc)

<br>  
### 3) Hãy nêu các yêu cầu cơ bản trong thủ tục sinh khóa trong thuật toán mã hóa RSA?. Hãy phân tích các yêu cầu cơ bản đó?.
<br>
- Phép tính sinh khóa là chọn p và q nguyên tố để tính N.
- Để phân tích số N thành tích 2 thừa số nguyên tố p và q chỉ có 1 cách duy nhất là thử từng số p và q.
- Do đó p và q phải đủ lớn để việc thử là không khả thi.
<br>

  ![image](https://github.com/H4lst0n/mmhcs/assets/91616280/543a098e-ed1a-4bd3-b5b8-8350e76db796)


### 4) Hãy trình bày về quá trình mã hóa và giải mã của thuật toán RSA?. Hãy lấy ví dụ minh họa về quá trình mã hóa và giải mã của thuật toán RSA?.
<br>

  ![image](https://github.com/H4lst0n/mmhcs/assets/91616280/db7b470f-4643-4862-85fc-892d275339f4)

### 5) Hãy phân tích mức độ an toàn của thuật toán RSA?.
<br>
Độ phức tạp trong tính toán RSA:
Có hai vấn đề về độ phức tạp tính toán trong phương pháp mã hóa RSA. Đó là các 
phép tính sinh khóa và các phép tính mã hóa/giải mã.
<br>

### 6) Hãy trình bày về ưu nhược điểm của mã hóa bất đối xứng?.
<br>
- Ưu điểm:
  - Kích thước khóa lớn, độ an toàn cao;
  - Việc quản lý và phân phối khóa dễ dàng hơn so với mã hóa đối xứng.

- Nhược điểm:
  - Tốc độ mã hóa, giải mã chậm hơn so với mã hóa đối xứng
<br>    
### 7) Hãy nêu một vài ứng dụng của mã hóa bất đối xứng?.
<br>
- Ứng dụng cơ bản của các thuật toán mã hóa bất đối xứng nói chung bao gồm: 
  - Bí mật trong truyền tin (Confidentiality);
  - Chứng thực;
  - Kết hợp tính bí mật và tin cậy.
    
- Ứng dụng thực tế của các thuật toán mã hóa bất đối xứng:
  - Dùng để vận chuyển và bảo mật khóa bí mật cho mã hóa đối xứng;
  - Mã hóa email hoặc xác thực người gửi email (OpenPGP hay S/MIME);
  - Mã hóa hoặc nhận thực văn bản (Các tiêu chuẩn chữ ký XML* hoặc mã hóa XML* khi văn bản được thể hiện dưới dạng XML);
  - Xác thực người dùng ứng dụng (Đăng nhập bằng thẻ thông minh; nhận thực người dùng trong SSL);
  - Ứng dụng trong chữ ký số, chứng chỉ số. 
