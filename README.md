# Report_HaoThu
This is the report  our group
 # I. Sơ đồ tổng quan về hệ thống GIT
 ![](https://i.imgur.com/aTq5pm7.png)
 # II. Cách tạo một Repository
  ## A. cách tạo Repository
 Bước 1: Trước tiên bạn cần đăng nhập vào Github, sau đó nhấn dấu + trong menu , chọn New repository.
 ![](https://thachpham.com/wp-content/uploads/2015/04/github-create-repository.png)
 Bước 2: Đặt tên repository , chọn chế độ public (công khai), private (riêng tư). 
 ![](https://i.imgur.com/AGSCNd1.png)
  ## B. Cách viết file Readme.md trên Github
  Readme.md là một file mô tả cấu trúc , giao diện, hoạt động cơ bản mà dự án thực hiện.
  Viết bằng ngôn ngữ MARKDOWN,nó là một ngôn ngữ đánh dấu với cú pháp văn bản thô, được thiết kế để có thể dễ dàng chuyển thành HTML và nhiều định dạng khác sử dụng một công cụ cùng tên.
  ### Một số cơ bản về Markdown:
    1. Thẻ tiêu đề (H)
      - #.... <Nội dung thẻ> : với số lượng dấu #, từ # -> ... ###### tương ứng với thẻ tiêu đề cấp 1 đến 6 (h1 -> h6).
      Ví dụ : thẻ h1 : #  <Nội dung thẻ>
                  h2 : ##  <Nội dung thẻ>
                  h3 : ###  <Nội dung thẻ>
    2. Chèn Link, hình ảnh 
       - Để chèn hyperlink bạn chỉ cần paste luôn linh đó vào file .md (VD : https://github.com),<br>
         cũng có thể sử dụng cú pháp sau để thu ngắn đường dẫn của link
           VD : [Github](https://github.com) . khi đó hiện thị : Github , ta click vào "Github" nó sẽ dẫn đến link https://github.com.
       - Chèn ảnh : ![alt_text](Đường dẫn hình ảnh của bạn).
    3. In đậm , in nghiêng, bo chữ
       - In đậm text :
          cú pháp :   **Text cần in đậm**
       - In nghiêng text :
          cú pháp :   **Text cần in nghiêng**
       - Bo chữ:
          cú pháp :  `Đoạn cần bo`
       - Làm nổi bật 1 đoạn văn (bôi nền, khoanh vùng nổi bạt 1 đoạn văn) :
          cú pháp : ``` sh
                      dòng 1
                      .....
                      dòng n
                    ```
     4. Tạo bảng :
      ví dụ :
      cú pháp : 
              | Cột 1 Hàng 1 | Cột 2 | Cột 3| Cột 4 |
              |--------------|-------|------|-------|
              | Hàng 2 | 2 x 1 | 2 x 2 | 2 x 3 | 2 x 4 |
              | Hàng 3 | 3 x 1 | 3 x 2 | 3 x 3 | 3 x 4 |
              | Hàng 4 | 4 x 1 | 4 x 2 | 4 x 3 | 4 x 4 |
 
# III.Các lệnh cơ bản của GIT
 1. Khởi tạo Git trong một repository , vùng lưu trữ data có tên file .git , dưới dạng ẩn file.
    cú pháp : git init
    - Thêm các file vào vùng theo dõi :
      cú pháp : (git add <tên file> ) or (git add . ) ( nếu add tất cả các file)
    - kiểm tra trạng thái xem file nòa đang được theo dõi
      cú pháp : git status
    - kiểm tra xem sự thay đổi , thay đổi bao nhiêu dòng code
      cú pháp : git diff-stat
 2. Push code lên 1 github được lưu trữ online thì remote origin được coi la mặc định :
    cú pháp : git remote origin <đường dẫn của repository trên github của bạn>
 3. Clone : nếu clone 1 project từ github thì nó đã tự hiểu origin rồi, khi đó :
   cú pháp : git clone <đường dẫn của repository trên github của bạn>
 4. git pull origin <ten nhanh> : kéo những thay đổi mới nhất của project của bạn về local repository.
 5. git push origin <ten nhanh> : update những file , sự thay đổi đã được commit lên nhánh đó trên github.
 6. Commit : git commit -m "nội dung commit"
 7. Để đổi tên commit messege, bạn sử dụng amend
  Cú pháp: git commit --amend "Nội dung commit mới" <br>
# VI. Cách tạo merge request trên github
Nhu cầu khi chúng ta đã phát triển xong  1 tính năng ví dụ bar và muốn ghép nó vào với master, lúc này ta sẽ push code mình lên bar branch trên server, sau đó thực hiện yêu cầu được ghép code vào nhánh chính: yêu cầu này chính là pull request.
1. push code nhánh bar lên server :
  cú pháp : git push origin <tên nhánh (ví dụ : bar)>
2. nhấn nút để tạo 1 yêu cầu merge nhánh : 
![](https://i.imgur.com/undefined.png)
Sau đó màn hình sẽ chuyển hướng sang khởi tạo yều cầu pull request này :
![](https://i.imgur.com/XCBYgZL.png)
Điền thông tin cần thiết vào và bấm Create pull request lúc này, người chịu trách nhiệm cho dự án sẽ nhận được yêu cầu của bạn, người ta sẽ kiểm tra và cho phép ghép code vào. Lúc này, tính năng bar sẽ thuộc phần chính của dự án.
    
