# Tác giả: Nguyễn Tấn Dũng

# Giới thiệu
- Bạn không còn xa lạ gì về requests trong các công cụ của mình nhưng nếu dùng requests thì tốc độ lại tương đối kém so với socket và các tầng thấp, requests chúng vốn được tạo lên từ urllib3 mà nó dùng chính python để làm việc lên theo góc nào đó nó vẫn chậm.
- Ngay tại đây tôi đem đến giải pháp xử lý nhanh hơn, ít tốn tài nguyên và tạo ra các xử lý nhanh chóng như cái tên vậy """SR""".
- Thư viện này được tôi xây và nấu trên nền ssl sẵn có và cách dùng như requests để cảm thấy quen thuộc thay vì phải làm quen mới hoặc tự dùng ssl và tự xử lý thì giờ tôi sẽ xử lý giúp bạn, nhằm mục đích nhanh chóng ít call nhiều điểm tránh dùng CPU và MEMORY nhiều.
- Tôi sẽ đẩy mọi phần xử lý về C-Extention để nó tạo ra hiệu năng cũng như đem lại tốc độ xử lý nhanh chóng, hiệu quả, đây luôn là giải pháp tôi hướng tới để nâng cấp trải nhiệm, giúp gần nhất tốc độ vật lí, tuy nhiên phải dõ rằng server phản hồi và tốc độ cũng phải có giới hạn của nó việc tôi làm chỉ giải quyết con số nhỏ.

# Có những gì
- Dùng TLS cao nhất 1.3 cho mọi requests
- Dùng C-Extention để xử lý mọi phản hồi cũng như header và mọi thứ liên quan
- Báo lỗi dõ dàng và nổi bật
- Cú pháp xử dụng quen thuộc
- Tự xử lý để tránh người dùng xử lý vấn đề phức
- Hỗ trợ bất đồng hộ và xử lý bất đồng bộ
- Hỗ trợ h2 và h3 nhưng sẽ ở phiên bản lớn các phiên bản đầu tập chung ở fix lỗi và xử lý
- Có Auth, Cookie, Token, v.v để giao tiếp đăng nhập với server chống phải tự làm lại 
- Hỗ trợ I2P nếu có thể trong tương lại

# Tình trạng
- Hiện tại code chưa có 1 tý gì vì đang cập nhật cho httpmas vì là một mình làm
- Bản 1. sẽ là bản test và fix cũng như cho các Dev khác tham khảo báo cáo và góp ý


# Cập nhật
