# Phân tích và xếp loại đánh giá Tiếng Việt trên Foody
### Mục lục
1. [Giới thiệu](#introduction)
2. [Tập dữ liệu](#dataset)
3. [Phương pháp](#method)
4. [Kết quả](#result)
5. [Thành viên](#author)

## Giới thiệu<a name="introduction"></a>

Trong vài năm trở lại đây, dịch vụ vận chuyển nói chung hay giao và đặt đồ ăn nói riêng cực kỳ phát triển. Tuy nhiên cũng chính vì thế mà cũng không thể đảm bảo hết được mọi nguồn chất lượng dịch vụ. Chính vì thế chúng ta cần có những đánh giá review để người tiêu dùng có thể sử dụng những sản phầm chất lượng, phù hợp với bản thân. Tuy nhiên con người luôn bận rộn với những mục tiêu đề ra vì thế thời gian luôn là vấn đề nan giải với mỗi các nhân chúng ta. Chúng ta không thể tự trải nghiệm và tự đánh giá hết đồ ăn trên mạng được. Ứng dụng này sẽ giúp chúng ta tiết kiệm thời gian bằng cách đưa ra đánh giá rating của các comment về món ăn trên Foody bằng cách sử dụng mô hình LSTM

Bài báo cáo này được trình bày bởi nhóm INT3405_20_NQT. Nhóm đang xếp hạng thứ 32 trên bảng xếp hạng của Kaggle với điểm số là 0.92174   


## Dataset<a name="dataset"></a>

Trong project này, toàn bộ dữ liệu dùng cho đồ án được thu thâp từ Foody [dataset](https://www.kaggle.com/competitions/int3405-sentiment-analysis-problem/data) 

## Method<a name="method"></a>

A.	Recurrent Neural Network

Recurrent Neural Network (RNN – Mạng thần kinh hồi quy) là một lớp của mạng thần kinh nhân tạo mà trong đó đầu ra của bước trước là đầu vào cho bước này. Khác với các mạng thần kinh trước đó với đầu vào và đầu ra độc lập với nhau, khi cần tiên đoán trước các từ tiếp theo trong một câu, ta cần biết và lưu trữ từ trước đó. RNN đã được đưa ra để giải quyết vấn đề với Hidden Layer (tầng ẩn). Phần quan trọng nhất ở RNN là Hidden State (trạng thái ẩn) lưu trữ những thông tin về một chuỗi.

Các kiến trúc của RNN:
- Long short-term memory (LSTM)
- Gated recurrent units (GRUs)


B.	Long short-term memory (LSTM)

Mạng LSTM (Bộ nhớ ngắn hạn – dài hạn) là một loại RNN (Mạng thần kinh tái phát) được sử dụng rộng rãi để học các bài toán dự đoán dữ liệu tuần tự. Giống như mọi mạng thần kinh khác, LSTM cũng có một số lớp giúp nó học và nhận dạng mẫu để có hiệu suất tốt hơn

## Kết quả

* Các chỉ số đánh giá mô hình trong quá trình training được mô tả qua biểu đồ.
* Accuracy lớn nhất là 0.92174

## Thực thi

### Cài đặt thư viện 
* Tất cả các thư viện yêu cầu được trình bày trong requirements.txt
* Để cài đặt thư viện, chạy các lệnh bên dưới
```bash

pip install requirements.txt
```

## Thành viên
```
Nguyễn Phúc Tuệ - 19020652@vnu.edu.vn
Trần Hồng Quân - 19020597@vnu.edu.vn 
Cao Kỳ Nam - 19020581@vnu.edu.vn


