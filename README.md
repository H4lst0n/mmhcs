# mmhcs

## Chương 3: Mã hóa bất đối xứng
<br>

  ![image](https://github.com/H4lst0n/mmhcs/assets/91616280/9a9c53be-64e9-4abb-84b4-560164315f42)

### 1) Hãy trình bày đặc điểm chính của thuật toán mã hóa khóa công khai?. Vẽ sơ đồ minh họa quy trình mã hóa và giải mã của thuật toán mã hóa khóa công khai?.

- Mã hóa công khai ( hay gọi là mã hóa bất đối xứng ): là phương pháp mã hóa mà khóa sử dụng để mã hóa sẽ khác với khóa dùng để giải mã.

- Khóa dùng để giải mã hóa gọi là khóa công khai và khóa dùng để giải mã gọi là khóa bí mật.

- Tất cả mọi người đều có thể biết khóa công khai nhưng chỉ người nhận mới nắm giữ khóa bí mật nên mới có thể giải mã


### 2) Hãy trình bày về chứng thực trong mô hình mã hóa bất đối xứng?.
- Mã hóa bất đối xứng là các phương pháp mà quy trình mã hóa và giải mã sử dụng các khóa khác nhau qua các bước
  - Mã hóa chứng thực
  - Mã hóa bảo mật
  - Giải mã bảo mật
  - Giải mã chứng thực

  ![image](https://github.com/H4lst0n/mmhcs/assets/91616280/fc21b95c-bef9-44ae-a4ef-6afd9b13dbbc)


### 3) Hãy nêu các yêu cầu cơ bản trong thủ tục sinh khóa trong thuật toán mã hóa RSA?. Hãy phân tích các yêu cầu cơ bản đó?.

- Phép tính sinh khóa là chọn p và q nguyên tố để tính N.

- Để phân tích số N thành tích 2 thừa số nguyên tố p và q chỉ có 1 cách duy nhất là thử từng số p và q.

- Do đó p và q phải đủ lớn để việc thử là không khả thi.


  ![image](https://github.com/H4lst0n/mmhcs/assets/91616280/543a098e-ed1a-4bd3-b5b8-8350e76db796)


### 4) Hãy trình bày về quá trình mã hóa và giải mã của thuật toán RSA?. Hãy lấy ví dụ minh họa về quá trình mã hóa và giải mã của thuật toán RSA?.
<br>

  ![image](https://github.com/H4lst0n/mmhcs/assets/91616280/db7b470f-4643-4862-85fc-892d275339f4)

### 5) Hãy phân tích mức độ an toàn của thuật toán RSA?.

- Mức độ an toàn của RSA hiện tại vẫn rất cao nếu sử dụng đúng các phương pháp tạo khóa và duy trì khóa có độ dài đủ lớn. 

- Tuy nhiên, cần liên tục theo dõi và cập nhật các biện pháp bảo mật để đối phó với các tiến bộ trong công nghệ tính toán và toán học.

### 6) Hãy trình bày về ưu nhược điểm của mã hóa bất đối xứng?.

- Ưu điểm:
  - Kích thước khóa lớn, độ an toàn cao;
  - Việc quản lý và phân phối khóa dễ dàng hơn so với mã hóa đối xứng.

- Nhược điểm:
  - Tốc độ mã hóa, giải mã chậm hơn so với mã hóa đối xứng
 
### 7) Hãy nêu một vài ứng dụng của mã hóa bất đối xứng?.

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


## Chương 5: Thám mã

  ![image](https://github.com/H4lst0n/mmhcs/assets/91616280/cbd311f9-4183-4e26-bb07-9e4fd215b56a)


Câu 1. Hãy trình bày khái niện về thám mã?

- Phương pháp thám mã: là các thuật toán, kỹ thuật nhằm phân tích bản mã tìm ra khóa, hoặc bản rõ, hoặc cả khóa và bản rõ. Như vậy, phương pháp thám mã cũng giống như phương pháp mã hóa là đều có những phương pháp và kỹ thuật chung.
- Tuy nhiên, sự khác biệt ở chỗ: phương pháp mã hóa sử dụng thuật toán, kỹ thuật nhằm biến đổi thông điệp thành bản mã, còn phương pháp thám mã dùng phương pháp, kỹ thuật, thuật toán nhằm  tìm ra bản rõ hoặc quy luật mã hóa, hoặc khóa bí mật. 

Câu 2. Hãy trình bày một số kỹ thuât thám mã?
- Thám mã khi chỉ biết bản mã (ciphertext-only attack)
- Thám mã khi đã biết bản rõ (known-plaintext attack)
- Thám mã bản rõ chọn sẵn (chosen plaintext attack)
- Thám mã chọn bản mã thích nghi (adaptive-chosen-ciphertext attack)

Cấu 3. Hãy trình bày về quy trình thám mã?
- Thám mã: bước này thực hiện phân tích bản mã. Trong bước này gồm 2 công việc chính:
  - Thám mã trực tiếp: Nếu bản mã thuộc loại mã hóa truyền thống như các mã hóa thủ công hoặc được mã bằng một máy mã cụ thể nào đó mà có thuật toán thám mã thì có thể tiến hành thám trực tiếp (thực hiện thủ công và sau đó có thể tự động hoá bằng lập trình trên máy tính). 
  
  - Xây dựng phương pháp thám mã: Nếu giải thuật mã hóa thuộc loại mới, công việc yêu cầu phức tạp cần phải xây dựng phương pháp thám mã cho phù hợp.

Cấu 4. Hãy trình bày về phương pháp thám mã vi sai?

Câu 5. Hãy trình bày về phương pháp thám mã tuyến tính?

Câu 6. Hãy trình bày về phương pháp thám mã nội suy?

Câu 7. Hãy trình bày về một số kỹ thuật thám mã dựa trên cơ sở toán học của các giải thuật mã hóa khóa bất đối xứng?

Câu 8. Hãy trình bày về thám mã lựa chọn bản mã thích nghi?

Câu 9. Hãy trình bày về thám mã kênh bên trên giải thuật mã hóa khóa bất đối xứng 
