# Report_HaoThu
This is the report  our group
# 1.Cách sử dụng .gitignore
*.gitignore là gì ?*<br>
-Tình huống là: Bạn làm việc theo nhóm, bạn muốn sử dụng git để quản lý mã nguồn.Tuy nhiên, dự án của bạn sẽ sinh ra những file build, gen, config, local, password, properties.Những file này thường là sẽ tự sinh và sẽ khác nhau tuỳ từng máy, khi đưa lên git thì khi người khác lấy về sẽ sinh ra xung đột (conflict) => gây cản trở cho công việc của bạn. Ngoài ra thì những file này thường rất nặng => tốn băng thông và tốn thời gian pull/push.Để giải quyết vấn đề này, git đưa ra **.gitignore** file.<br>
-.gitignore là file định nghĩa những file, folder nào sẽ bị bỏ qua (ignore) và không thêm nó vào git. <br>
*Cách tạo file .gitignore*
-Đầu tiên mở terminal trong repository của bạn và gõ lệnh:<br>
**touch .gitignore** <br>
-Lúc này git sẽ tạo ra cho chúng ta 1 tệp tin là .gitignore,dùng notepad mở lên và khai báo các thư và mục tệp tin cần loại bỏ. 
Bạn có thể vào https://github.com/github/gitignore để tham khảo một số mẫu gitignore đã có sẵn của rất nhiều ngôn ngữ & framework (Chỉ việc copy về dùng, thay đổi nếu cảm thấy cần thiết).<br>
# 2.Cách sử dụng SourceTree
-Đầu tiên, bạn cần tải phần mềm Source Tree về cài đặt và đăng nhập vào để có thể sử dụng <br>
-Dưới đây là giao diện chính của Source Tree<br>
![](https://i.imgur.com/8qLgkTV.jpg)
**Kéo dự án về ( Clone project )**<br>
- Lên github để lấy địa chỉ của Responsitory về :<br>
![](https://i.imgur.com/j0s3pK6.jpg) <br><br>
 -Bạn click vào Clone/new một popup sẽ hiện ra , copy địa chỉ vừa lấy vào Source Path , chọn nơi lưu vào Destination Path, đặt tên tệp tùy ý vào Name <br>
 ![](https://i.imgur.com/94uzh1V.jpg)<br><br>
**Đẩy code lên( push code )**<br>
-Đây là việc cần thiết khi có sự thay đổi trong source code, trước khi push được bắt buộc phải click vào unstaged files và comment -> click vào push trên toolbar của source tree. Việc làm này phải được thực hiện thường xuyên khi có sự thay đổi về code để người quản lý có thể quản lý được công việc cũng như là các thành viên khác có thể nắm bắt được sự thay đổi.<br>
![](https://i.imgur.com/oAtO37v.jpg)<br><br>
**Kéo code về( pull code )**<br>
-Cũng giống như Push code lên tuy nhiên việc bây giờ chỉ là lấy code về bao gồm những thay đổi mà thành viên khác đã push lên. Bạn chỉ cần click vào Pull ở trên toolbar của source tree<br>
![](https://i.imgur.com/ab3g1Ha.jpg)<br><br>
 **Lưu ý:**<br>
– Nếu có nhiều người cùng thay đổi trên 1 file và cùng một chỗ thì chắc chắn bạn sẽ bị conflict và việc pull hoặc Push code lên sẽ báo lỗi và không thực hiện được. Dấu hiệu nhận biết lỗi Conflict sẽ xuất hiện dòng lỗi sau:<br>
![](https://i.imgur.com/k66RptC.jpg)<br><br>
– Cách phòng tránh Conflict thì tốt nhất team nên phân chia công việc cụ thể cho riêng từng  người không được làm chung file để tránh tình trạng trên
 # 3. Thêm một Remote vào Git hiện tại : <br>
 Vào Responsitory trên thanh công cụ phía trên, chọn Add Remote , ta có giống như hình dưới :<br>
 ![](https://i.imgur.com/RrHfII5.jpg)<br>
 -Tiếp theo chọn Add , đặt tên cho remote và lấy địa chỉ Responsitory mới trên GitHub về bằng cách copy link rồi chọn Ok <br>
 ![](https://i.imgur.com/XNRkIK8.jpg) 

 # 1. Sơ đồ tổng quan về hệ thống GIT
 ![](https://i.imgur.com/aTq5pm7.png)
 # 2. Cách tạo một Repository
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
 
# 3.Các lệnh cơ bản của GIT
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
# 4. Cách tạo merge request trên github
Nhu cầu khi chúng ta đã phát triển xong  1 tính năng ví dụ bar và muốn ghép nó vào với master, lúc này ta sẽ push code mình lên bar branch trên server, sau đó thực hiện yêu cầu được ghép code vào nhánh chính: yêu cầu này chính là pull request.
1. push code nhánh bar lên server :
  cú pháp : git push origin <tên nhánh (ví dụ : bar)>
2. nhấn nút để tạo 1 yêu cầu merge nhánh : 
![](https://i.imgur.com/undefined.png)
Sau đó màn hình sẽ chuyển hướng sang khởi tạo yều cầu pull request này :
![](https://i.imgur.com/XCBYgZL.png)
Điền thông tin cần thiết vào và bấm Create pull request lúc này, người chịu trách nhiệm cho dự án sẽ nhận được yêu cầu của bạn, người ta sẽ kiểm tra và cho phép ghép code vào. Lúc này, tính năng bar sẽ thuộc phần chính của dự án.

# 5. Cách sử dụng gitlab
- Tạo Repository:
    - Bước 1: Trước tiên bạn cần đăng nhập vào Gitlab, sau đó nhấn dấu chọn Project , chọn create a project.
        ![](https://i.imgur.com/rFLed4n.png)
    - Bước 2: Đặt tên repository , chọn chế độ public (công khai), private (riêng tư), hay internal (cho phép những user xác định) . 
        ![](https://i.imgur.com/ImwXhtq.png) <br>
- Tạo Group :
    - Bước 1: Trước tiên bạn cần đăng nhập vào Gitlab, sau đó chọn mục những groups của bạn, và tạo  1 group mới.
        ![](https://i.imgur.com/4FfphJY.png)
    - Bước 2 : Dẫn đường link đến project của bạn để nhóm tham gia, tên nhóm , ...
        ![] (https://i.imgur.com/ZSP5yLp.png) <br>
- Tạo Merge request :
    - Bước 1 : Sau khi bạn đã làm 1 chức năng và push nó vào 1 nhánh mới vừa tạo. Chọn mục Merge Request để tạo 1 yêu cầu  merge request
    - Bước 2 : Chọn nhánh sẽ merge với nhánh mới tạo của bạn (ví dụ : merge  nhánh bar vào nhánh master), project được mặc định là             project hiện tại đang truy cập.
        ![](https://docs.gitlab.com/ee/gitlab-basics/img/merge_request_select_branch.png)
    - Bước 3: khi đã sẵn sàng chọn nút continue , trang web sẽ chuyển tiếp thành tab điền nội dung message và gửi cho người leader (nhấn       nút submit) , nhằm thông báo cho người đó yêu cầu được merge nhánh , họ sẽ kiểm tra , nếu ổn thì sẽ chấp nhận yêu cầu , cấp phát         quyền merge nhánh, nếu có lỗi người leader đó sẽ yêu cầu kiểm tra lại.
        ![](https://docs.gitlab.com/ee/gitlab-basics/img/merge_request_page.png) <br>
- Phân quyền :
   - Bước 1 : Chọn project muốn add thêm thành viên để phân quyền xem project của họ . sau đó nhấn impersonate.
        ![](https://i.imgur.com/Tj5z97G.png)
   - Bước 2 : add thêm những người vào để sử dụng project.  nhấn " Here " phân quyền xem cho họ.
        ![](https://i.imgur.com/BmtityT.png)
   -Bước 3 : phân quyền xem cho những thành viên vừa add .
       Có 5 mức : Guest, Reporter, Master, Developer và Owner. 
       ![](https://i.imgur.com/6KAozJm.png)
       - Các mức được phép : <br>
       | |Guest | Reporter |Developer | Master|Owner | <br>
       |---|---|---|---|---|<br>
       | Tạo một issue | * | * | * | * |* <br>
       | Để lại ocmment | * | * | * | * |* <br>
       | Pull code của dự án | | * | * | * |* <br>
       | Tải dự án | | * | * | * |* <br>
       | Tạo một code snippets | | * | * | * |* <br>
       | Tạo một merge request | | | * | * |* <br>
       | Push thay đổi vào một nhánh không được bảo vệ | | | * | * |* <br>
       Xoá một nhánh không được bảo vệ | | | * | * |* <br>
       | Thêm Tags | | | * | * |* <br>
       | Viết Wiki| | | * | * |* <br>
       | Quản lý issue tracker | | | * | * |* <br>
       | Thêm một nhóm người dung mới | | | | * |* <br>
       | Push thay đổi vào nhánh được bảo vệ | | | | * |* <br>
       | Quản lý nhánh được bảo vệ | | | | * |* <br>
       | Quản lý Git tags | | | | * |* <br>
       |Sửa chữa dự án | | | | * |* <br>
       |Thêm deploy key vào dự án | | | | * |* <br>
       | Cấu hình dự án| | | | * |* <br>

