Abstract

Prismer là một mô hình vision-language yêu cầu ít dữ liệu và tham số

Prismer chỉ yêu cầu huấn luyện một số lượng nhỏ các thành phần, với phần lớn trọng lượng mạng được kế thừa từ những mạng sẵn có, được pre-trained, đóng băng trong quá trình huấn luyện

1 Introduction

Trong bài toán image captioning và visual question answering yêu cầu mô hình có khả năng nhận dạng, phát hiện, đếm, và nhận biết đối tượng 3D chi tiết

Giải pháp điển hình là sử dụng một lượng lớn dữ liệu hình ảnh - văn bản để huấn luyện một mô hình duy nhất khổng lồ học cách phát triển các kỹ năng một cách đồng thời dành riêng cho nhiệm vụ này từ đầu và trong cùng một kiến trúc chung

Thay vào đó, tác giả nghiên cứu một cách tiếp cận khác để học những kỹ năng, kiến trức lĩnh vực này thông quay các mạng con (experts) distinct and separate. Mỗi experts có thể được tối ưu hóa độc lập cho một nhiệm vụ cụ thể, cho phép sử dụng dữ liệu và kiến trúc theo miền cụ thể mà không thể thực hiện được với một mạng lớn duy nhất.