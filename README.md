# SEO-for-Angular-app
<h1> SEO là gì ? </h1>
 SEO( Search Engine Optimization) là một tập hợp các phương pháp nhằm nâng cao thứ hạng của một website trong các trang kết quả của các công cụ tìm kiếm (phổ biến nhất là Google). Các phương pháp đó bao gồm việc tối ưu hóa website (tác động mã nguồn HTML và nội dung website) và xây dựng các liên kết đến trang để các công cụ tìm kiếm chọn lựa trang web phù hợp nhất phục vụ người tìm kiếm trên Internet ứng với một từ khóa cụ thể được người dùng truy vấn. SEO là các kĩ thuật, hướng website tương tác tốt nhất với đối tượng là các công cụ tìm kiếm . SEO không quan tâm tới trải nghiệm lướt web mượt mà, mà quan tâm nhiều hơn tới các yếu tố như keyword trong nội dung của website, lượng link liên kết, hay tối ưu hóa trang web sao cho trình thu thập thông tin của các công cụ tìm kiếm thực hiện việc đánh mục lục được một cách dễ dàng nhất. 
 
<h1> Tạo một ứng dụng Angular 4 đơn giản </h1>

Đầu tiên,  chúng ta hãy xây dựng một ứng dụng đơn giản sử dụng Angular. Ứng dụng sẽ là một trang liệt kê một loạt chủ đề trên trang chủ.

<h2>Tạo một ứng dụng mới sử dụng ng-cli</h2>

Chúng ta sẽ sử dụng ng new command để tạo ứng dụng Angular 4.<br>

<img src="https://i.imgur.com/Q6eI95d.png"><br>

Tiếp theo, chúng ta sẽ tạo ra một component mà sau đó có thể thêm code logic vào. Chúng ta sẽ sử dụng ng g component command cho điều này:

<img src="https://i.imgur.com/Fmo61G1.png"><br>

<h2>Thêm mock data vào PostComponent</h2>

Để đơn giản, chúng ta sẽ không kết nối với một API bên ngoài. Thay vào đó, sẽ chỉ tạo ra một số dữ liệu mô phỏng và sử dụng dữ liệu đó trong ứng dụng của chúng ta.
Mở file ./src/app/blog/posts.component.ts, chúng ta sẽ thêm một số logic code để đảm bảo rằng nó hoạt động như mong muốn. Đầu tiên, mã hóa một số dữ liệu vào tệp. Thêm một method mới được gọi là postsData cho component.

<img src="https://i.imgur.com/lmoXVr7.png"><br>

Để sử dụng mock data đã đuợc tạo phía trên, chúng ta thay constructor method của PostsComponent class bằng đoạn code dưới đây:

<img src="https://i.imgur.com/hn9Hine.png"><br>

Trong đoạn code phía trên, chúng ta chỉ đơn giản gán cho thuộc tính posts bằng giá trị mà postsData method trả về, đây chính là cách chúng ta giả lập API response.

<h2>Tạo View cho PostsComponent</h2>
Bây giờ chúng ta đã có mock posts data. Chúng ta sẽ tạo một view hiển thị tất cả posts từ mock data.

Mở view ./app/blog/posts.component.html và thêm vào đoạn code dưới đây:
<img src="https://i.imgur.com/lZiQMLw.png"><br>

Đoạn code trên chỉ lấy về posts data sau đó lặp và hiển thị title của post.

Tiếp theo, mở file index.html và trong thẻ <head> thay nội dung với code dưới đây. Nó chỉ đơn giản sử dụng Bootstrap và thêm navigation bar:
<img src="https://i.imgur.com/O6Fgw9r.png"><br> 
 
 Sau đó, trong mảng NgModule declarations, thêm PostsComponent:<br>
 
 <img src="https://i.imgur.com/rVEqeDh.png"><br> 
