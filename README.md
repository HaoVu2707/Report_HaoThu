# Report_HaoThu
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
# 4. Tạo pull request trên github:
-Đề đảm bảo cho việc tương tác nhóm được tốt hơn, và hạn chế tối đa conflict có thể xảy ra, cũng như dễ dàng theo dấu dự án (để khôi phục trạng thái nếu lỡ có biến cố xảy ra), pull request ra đời:<br>
-Nhìn hình ta thấy có 2 branch là master , bar:<br>
![](https://i0.wp.com/appconus.com/blog/wp-content/uploads/2015/08/Screen-Shot-2015-08-07-at-2.36.55-PM.png)<br>
Vẫn ở trên github, chuyển sang anhthu branch và bấm vào Compare & pull request bạn sẽ được điều hướng sang màn hình Open a pull request<br>
![](https://i1.wp.com/appconus.com/blog/wp-content/uploads/2015/08/Screen-Shot-2015-08-07-at-2.41.01-PM.png)<br>
-Điền thông tin cần thiết vào và bấm Create pull request lúc này, người chịu trách nhiệm cho dự án sẽ nhận được yêu cầu của bạn, người ta sẽ kiểm tra và cho phép ghép code vào. Lúc này, tính năng bar sẽ thuộc phần chính của dự án
# 5.Tạo group và phân quyền trong github:<br>
-Để tạo một nhóm cho nhiều người cùng làm việc ta làm như sau:<br>
+Truy cập URL: https://github.com/settings/organizations, chọn New Organizations<br>
+Đặt tên và email cho tổ chức:
![](https://camo.githubusercontent.com/dba455a769d2a5c16e65978fb6b67089c61f433f/687474703a2f2f692e696d6775722e636f6d2f497648656357652e706e67)<br><br>
-Tại mục Choose the organization’s plan chọn Open Source để miễn phí, nhưng lúc này các Repo trong tổ chức sẽ là public.<br>
+Mời các thành viên cho tổ chức<br>
![](https://camo.githubusercontent.com/938a1967fd1c18ac6b9eb7ff2efaeef8c59366e7/687474703a2f2f692e696d6775722e636f6d2f78563343756b632e706e67)<br><br>
+ Tạo một team mới <br>
![](https://camo.githubusercontent.com/22088fab52bd8e29fe1a9ef5f6d7285d237fe6ee/687474703a2f2f692e696d6775722e636f6d2f376b574c4e59452e706e67)<br><br>
![](https://camo.githubusercontent.com/daf9deade83a8e0aefcfba21fd00f187d4550c63/687474703a2f2f692e696d6775722e636f6d2f7a4f336b767a5a2e706e67)<br><br>
Các member của team này có quyền write với các repo của team.
Với 3 mức: Read Access, Write Access, Admin Access Github cho phép chúng ta phân quyền tới các thành viên của nhóm.
Để mời một người dùng khác vào team, ta click vào team đó và search tên của người dùng cần tìm
![](https://camo.githubusercontent.com/73070ffe87ce06e0ee497cbd9a8b48ce14aa05bc/687474703a2f2f692e696d6775722e636f6d2f557365703947502e706e67)<br><br>
-Sau đó hệ thống sẽ yêu cầu bạn nhập password để xác thực, nếu thành công, một email xác nhận sẽ được gửi đến người được mời và người này sẽ xác nhận có tham gia vào tổ chức hay không.

-Để tạo một repo cho tổ chức, ta chỉ cần click vào tổ chức đó, sau đó chọn Create new Repostory. Các hành động clone, add, commit,... làm như bình thường.
# 6. Sơ lược về phân nhánh trong git :
**CÁC NHÁNH CHÍNH**<br>
-Repo trung tâm giữ hai branch chính với vòng đời vô tận:<br>
master<br>
develop<br>
Song song với master branch, một branch khác tồn tại gọi là develop.<br>
Chúng tôi sẽ coi origin/develop như một branch chính mà source code của HEAD luôn phản ánh trạng thái của những update mới nhất ở bản release tiếp theo. Đây là nơi những thay đổi được update thường xuyên.Khi source code trong develop branch đạt đến một điểm ổn định nó sẽ được release, sau đó tất cả các thay đổi đó cần phải được merge vào master branch.Sau mỗi lần thay đổi được merge vào master branch, nó sẽ được coi là sản phẩm mới được phát hành bởi sự xác định trước. <br>

**CÁC NHÁNH HỖ TRỢ**<br>
Tiếp theo 2 nhánh chính là master và develop, mô hình phát triển sử dụng rất nhiều các nhánh hỗ trợ để hỗ trợ việc phát triển song song giữa các thành viên trong team, dễ dàng theo dõi các tính năng, chuẩn bị cho phiên bản sắp phát hành và để hỗ trợ việc fix bug nhanh chóng. Không giống như các branch chính, các branch này luôn có vòng đời hạn chế, vì thế chúng sẽ được loại bỏ dần dần.
Các kiểu branch khác nhau:<br>
Feature branches<br>
Release branches<br>
Hotfix branches<br>
Mỗi branch có một mục đích riêng và bị ràng buộc với các quy tắc nghiêm ngặt như ở branch gốc của nó và ở các branch là mục tiêu thực hiện merge của chúng.<br>

*Nhánh feature* <br>
Có thể phân nhánh từ: develop<br>
Phải merge trở lại vào: develop<br>
Quy ước đặt tên branch: không được trùng tên với các định danh sau master, develop, release- hay hotfix-<br>
Nhánh feature (đôi khi được gọi là các nhánh topic) được sử dụng để phát triển các tính năng mới cho sản phẩm tiếp theo hoặc một bản phát hành trong tương lai. Khi bắt đầu phát triển một tính năng, đôi khi bạn sẽ không thể xác định được trước việc nó có nằm ở bản release tiếp theo hay không. Về cơ bản, một feature branch cứ tồn tại miễn là tính năng đó vẫn được phát triển, nhưng sẽ được merge trở lại vào develop (để chắc chắn thêm các tính năng mới cho bản phát hành kế tiếp) hoặc bỏ đi (trong trường hợp thất bại).<br>
Khi bắt đầu làm việc trên một tính năng mới, bạn hãy phân nhánh từ nhánh develop.<br>

*Nhánh Release*<br>
Có thể phân nhánh từ: develop<br>
Phải merge lại vào: develop<br>
Quy ước đặt tên branch:release -<br>
Nhánh release hỗ trợ việc chuẩn bị release một sản phẩm mới hay một version mới. Bạn cần phải tỉ mỉ từng chút một để hoàn thành sản phẩm một cách tốt nhất. Hơn nữa, nó cho phép sửa chữa các lỗi nhỏ và chuẩn bị meta-data để release (version, ngày tháng xây dựng,…). Bằng cách thực hiện tất cả các công việc này trên nhánh release, nhánh develop được giải phóng để nhận các tính năng cho sản phẩm tiếp theo.<br>
Thời điểm quan trọng để phân nhánh một release branch mới từ develop là khi develop (gần như) đã bao gồm các tính năng mong muốn ở bản release tới. Ít nhất tất cả các tính năng được định hướng cho việc phát hành sản phẩm-chuẩn bị được xây dựng phải được merge vào develop tại thời điểm này. Tất cả các tính năng được nhắm đến ở các phiên bản trong tương lai có thể không cần đến – chúng phải đợi sau khi release branch được phân nhánh.<br>
Release branch được tạo ra từ develop branch<br>
Khi release branch đã sẵn sàng để trở thành một phiên bản thực sự, chúng ta cần phải làm một số việc sau. Đầu tiên, nhánh release sẽ được merge vào nhánh master. Tiếp theo, commit trên master phải được đánh tagged để lưu lại và tham chiếu với các phiên bản cũ. Cuối cùng, những thay đổi được thực hiện trên nhánh release cần được merge trở lại vào nhánh develop, do đó phiên bản tiếp theo cũng chứa các lỗi được fix.<br>

*Nhánh Hotfix*<br>
Có thể phân nhánh từ: master<br>
Phải merge trở lại vào: Develop và master<br>
Quy ước đặt tên branch: **hotfix -***<br>
Nhánh hotfix rất giống nhánh release ở chỗ chúng cùng có nghĩa là chuẩn bị cho một bản update mới sắp release, mặc dù nó không nằm trong kế hoạch. Chúng phát sinh từ sự cần thiết của một hành động tức khắc khi có một bug không mong muốn trong một phiên bản sản phẩm. Khi một bug nghiêm trọng trong một phiên bản sản phẩm xảy ra, nó cần phải được giải quyết ngay lập tức. Một nhánh hotfix có thể được phân nhánh từ các tag tương ứng trên nhánh master.<br>
Bản chất là công việc của các thành viên trong team (trên nhánh develop) vẫn có thể tiếp tục, trong khi một số người khác thì chuẩn bị việc fix bug.<br>
Nhánh hotfix được tạo ra từ nhánh master.<br>
Khi hoàn thành, bugfix cần được merge lại vào nhánh master, đồng thời cũng cần merge vào nhánh develop, để fix khi bugfix có thể xuất hiện trong phiên bản tiếp theo. Nó hoàn toàn tương tự như cách thực hiện nhánh release.<br>
