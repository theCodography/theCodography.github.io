---
title: From Zero to Front-end Hero (Part 2)
layout: post
date: 2020-12-30T9:13:00Z
description: Tôi nhớ khi bắt đầu học front-end. Tôi đã tìm được rất nhiều bài viết, tài nguyên, và vì thế tôi đã bị quá tải, tôi không biết mình cần học gì và thậm chí cũng chẳng biết bắt đầu từ đâu.
imgUrl: front-end.png
---

*Bài viết được dịch từ: [from-zero-to-front-end-hero](https://www.freecodecamp.org/news/from-zero-to-front-end-hero-part-1-7d4f7f0bff02/#.1dfar8kg1)*
## Cross Browser Support
Có nghĩa là code của bạn hỗ trợ hầu hết các trình duyệt mới nhất. Một vài thuộc tính CSS như transition cần vendor prefixes để làm việc trên nhiều trình duyệt khác nhau. Điểm chính là bạn phải kiểm thử website của mình trên nhiều trình duyệt như Chrome, Firefox, và Safari.

![](https://cdn-media-1.freecodecamp.org/images/OHjyoarMjwNNaA1egCa-uqoF15bLNeX2VThf)

## CSS Preprocessors và Postprocessors
Kể từ khi được giới thiệu vào năm 1990, CSS đã đi được một chặng đường dài. Khi mà các hệ thống UI ngày càng trở lên phức tạp, mọi người bắt đầu sử dụng các preprocessors và postprocessors để quản lý sự phức tạp.

CSS preprocessors là ngôn ngữ CSS mở rộng, nó bổ sung thêm biến, mixin và kế thừa. Có hai CSS preprocessors chính là Sass và Less. Trong năm 2016, Sass được sử dụng rộng rãi hơn. Bootstrap, một framework CSS phổ biến, đã chuyển từ Less sang Sass. Cũng cần biết rằng, hầu hết mọi người thường nói về Sass, nhưng thực sự họ đang nói về SCSS.

![alt](https://techmaster.vn/media/fileman/Uploads/users/188/1-7Px9Kzaw8-eLCf2D41yauQ.png)

CSS post processors áp dụng các thay đổi tới CSS sau khi viết hoặc đã được biên dịch bởi một preprocessor. Ví dụ, một vài post processors giống như PostCSS có các plugin thêm các vendor prefixes tự động.

Trong lần đầu tiên khám phá CSS preprocessors và postprocessors, bạn có thể bị hấp dẫn để sử dụng chúng ở mọi nơi. Nhưng, hãy bắt đầu thật đơn giản và thêm các phần mở rộng chẳng hạn như variables và mixins chỉ khi cần thiết.

## Grid Systems và Responsiveness
Grid systems là những cấu trúc CSS giúp bạn xắp xếp và tổ chức các phần tử theo chiều dọc và chiều ngang.

![alt](https://cdn-media-1.freecodecamp.org/images/C0FspsiFiCRj19ot9QpIIqskUdBR3YxdflEx)

Các framework như Bootstrap, Skeleton và Foundation cung cấp các stylesheet để quản lý các dòng và các cột trong layout. Khi sử dụng các framework, bạn cũng cần hiểu cách các grid làm việc.

Một trong những mục đích chính của grid systems là bổ sung khả năng *responsiveness* cho website của bạn. Responsiveness có nghĩa là website của bạn có thể resize dựa theo độ rộng của màn hình. Responsiveness thường đạt được bằng các sử dụng CSS media queries, các quy tắc CSS khác nhau chỉ áp dụng cho một loại màn hình nhất định.

![](https://cdn-media-1.freecodecamp.org/images/Hr08b0o17uzYf3tkczwV4-ecp5ZCho0megI2)

## Luyện tập HTML và CSS
Bây giờ bạn đã được trang bị các best practices, hãy chiến đấu để kiểm nghiệm chúng. Mục tiêu của 2 thí nghiệm tiếp theo là luyện tập viết clean code và quan sát hiệu quả lâu dài của các best practice về tính dễ bảo trì và dễ đọc.

### Thí nghiệm 3
Trong phần này, hãy chọn một thí nghiệm bạn đã thực hiện và refactor code của bạn sử dụng một vài best practices mà bạn đã học được. Refactoring nghĩa là chỉnh sử code của bạn sao cho dễ đọc và ít phức tạp hơn.

Có khả năng refactor code hiệu quả là một kỹ năng quan trọng của một front-end developer. Tạo ra code có chất lượng là một quá trình lặp đi lặp lại. [Các kiến trúc CSS: Refactor code CSS](https://www.sitepoint.com/css-architectures-refactor-your-css/) của bạn là một khởi đầu tốt cho việc refactoring code của bạn.

![alt](https://cdn-media-1.freecodecamp.org/images/mH9nfLYxpdDfk99DZ8OysRJc899BCAxH-zIR)

Đây là một vài câu hỏi bạn cần trả lời khi tiến hành refactoring lại code:

- Tên của các class chưa rõ ràng? 6 tháng sau, bạn sẽ vẫn hiểu ý nghĩa của các class này?
- HTML và CSS đã có ngữ nghĩa rõ ràng? Khi đọc lướt qua code, bạn có thể nhanh chóng hình dung cấu trúc và quan hệ giữa các thành phần?
- Bạn đang tái sử dụng cùng một màu mã hex nhiều lần? Sẽ tốt hơn nếu bạn refactor nó thành một biến Sass?
- Code của bạn có làm việc tốt trên Safari như trên Chrome không?
- Bạn có thể thay thế một vài đoạn code layout bằng một grid system như Skeleton?
- Bạn thường xuyên sử dụng cờ !important? Làm sao để sửa chữa điều này?

### Thí nghiệm 4
Trong thí nghiệm cuối cùng này, bạn sẽ sử dụng các best practices đã học để xây dựng một trang portfolio. Tuy nhiên, hiệu quả của các best practice sẽ không rõ ràng cho đến khi bạn áp dụng chúng vào các dự án lớn hơn.

Với một front-end developer, trang portfolio là một tài sản kỹ thuật số quan trọng nhất của bạn. Portfolio là một trang web giới thiệu về công việc của bạn. Quan trọng hơn, nó giúp bạn ghi lại và theo dõi quá trình phát triển của mình. Vì thế nếu bạn chỉ có 1 hoặc 2 thứ để trưng bày, hãy đặt chúng lên.

![alt](https://cdn-media-1.freecodecamp.org/images/tryDsnrQ7cKm1ixAE5T9qjymy9dGDUvslM8W)

Để bắt đầu, bạn có thể làm theo hướng dẫn trong bài viết của Adham Dannaway, [Một workflow đơn giản để thiết kế và phát triển một trang portfolio](https://www.smashingmagazine.com/2013/06/workflow-design-develop-modern-portfolio-website/).

Nếu portfolio đầu tiên của bạn chưa hoàn hảo, điều đó là bình thường. Hoàn thiện portfolio sau nhiều lần lặp đi lặp lại. Và điều quan trọng là bạn xây dựng nó bằng những kỹ năng của mình.

## Liên tục học hỏi
Khi mà HTML và CSS vẫn sẽ được sử dụng trong một thời gian dài, điều quan trọng là liên tục cập nhật kiến thức front-end.

![alt](https://cdn-media-1.freecodecamp.org/images/2lvHNFA5gjihoYOH4D01MKGCCTfbnjPio4GZ)

Dưới đây là danh sách các wesite, blog và forum tất cả đều thú vị để đọc và tìm hiểu thông tin

- CSSTricks
- Smashing Magazine
- Designer News
- Nettuts+
- CSS Wizard

## Học qua ví dụ
Cuối cùng, cách học tốt nhất là qua ví dụ. Đây là một tập hợp các styleguides và code conventions, sẽ dạy bạn cách làm việc hiệu quả hơn.

### Styleguides

![alt](https://cdn-media-1.freecodecamp.org/images/vLcVFsil3JZ3E9mvD13Tl0mj7bY0nIqtUKlg)

Styleguides là tập hợp các CSS component và các pattern, có thể tái sử dụng trên nhiều trang web. Điều quan trọng cần chú ý từ các styleguides này là cách các thành phần dựa trên HTML và CSS cho phép bạn tái sử dụng code tuân theo quy tắc DRY.

- Mapbox
- LonelyPlanet
- SalesForce
- MailChimp

### Code Conventions
Code conventions được thiết kế để làm cho code của bạn dễ đọc và dễ bảo trì. Một số liên kết như Các hướng dẫn về CSS hướng dẫn viết HTML và CSS tốt hơn trong khi các liên kết khác như Các hướng dẫn và bộ công cụ CSS trên Github lại là những ví dụ về code chất lượng.

- [CSS Guidelines](https://cssguidelin.es/)
- [Các hướng dẫn và bộ công cụ CSS trên Github](https://github.com/primer/css)
- [Styleguide CSS của AirBnB](https://github.com/airbnb/css)

## Tổng kết
Hy vọng, đến cuối bài viết này, bạn đã quen thuộc với HTML và CSS và có một vài dự án từ những thứ bạn đã học được. Cách tốt nhất để học front-end là xây dựng các dự án và thí nghiệm. Nhớ rằng, mọi front-end developer đều bắt đầu từ một nơi nào đó. Và bắt đầu ngay từ hôm nay sẽ tốt hơn ngày mai.