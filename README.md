<!-- Banner -->
<p align="center">
  <a href="https://www.uit.edu.vn/" title="Trường Đại học Công nghệ Thông tin">
    <img src="https://i.imgur.com/WmMnSRt.png" alt="UIT - University of Information Technology" width="400">
  </a>
</p>

<h1 align="center"><b>PHÂN TÍCH DỮ LIỆU KINH DOANH – IS403.P21</b></h1>
<p align="center"><i>Học kỳ 2 – Năm học 2024–2025</i></p>

---

## Thông tin môn học

- **Tên môn học:** Phân tích dữ liệu kinh doanh
- **Mã môn học:** IS403
- **Mã lớp:** IS403.P21  
- **Giảng viên hướng dẫn:** ThS. Dương Phi Long

---

## Giới thiệu đề tài

Giá năng lượng luôn là một trong những chỉ số kinh tế quan trọng, tác động mạnh mẽ đến thị trường tài chính, sản xuất công nghiệp và sinh hoạt dân cư. Trong bối cảnh kinh tế toàn cầu nhiều biến động, việc dự đoán chính xác xu hướng giá các loại năng lượng như dầu thô, khí tự nhiên và dầu sưởi ấm sẽ giúp doanh nghiệp và nhà đầu tư đưa ra quyết định kịp thời và hiệu quả hơn.

Đề tài này tập trung vào việc **xây dựng mô hình dự đoán giá năng lượng tại Hoa Kỳ** thông qua dữ liệu lịch sử giá từ năm 2019 đến 2025. Nhóm đã áp dụng nhiều mô hình học máy hiện đại nhằm tối ưu hiệu suất dự báo, đồng thời phân tích các đặc trưng biến động của từng loại năng lượng.

---

## Nội dung thực hiện

### 1. Bộ dữ liệu
- **Nguồn dữ liệu**: Giá Futures của 3 loại nguyên liệu năng lượng:
  - Dầu thô (Crude Oil)
  - Khí tự nhiên (Natural Gas)
  - Dầu sưởi ấm (Heating Oil)
- **Thời gian**: Từ 01/01/2019 đến 30/04/2025
- **Đặc điểm**:
  - Crude Oil: Biến động mạnh, phân phối rộng
  - Natural Gas: Dữ liệu lệch, khó dự báo
  - Heating Oil: Ổn định, dễ học

---

### 2. Phương pháp phân tích và mô hình áp dụng

| Mô hình         | Đặc điểm chính                                                                 |
|-----------------|--------------------------------------------------------------------------------|
| **GRU**         | RNN cải tiến, tối ưu với chuỗi thời gian; áp dụng grid search và early stopping |
| **LSTM**        | Mô hình chuỗi có khả năng ghi nhớ dài hạn; thử nghiệm nhiều tham số             |
| **SARIMA**      | Mô hình thống kê cổ điển, phù hợp dữ liệu có tính mùa vụ                       |
| **SVR**         | Support Vector Regression, áp dụng kernel RBF và linear                        |
| **Prophet**     | Mô hình từ Facebook, dễ giải thích, xử lý tốt xu hướng và mùa vụ               |
| **LightGBM**    | Gradient boosting tree, xử lý tốt dữ liệu dạng bảng, nhiều đặc trưng           |
| **Transformer** | Mô hình hiện đại cho chuỗi thời gian, khai thác quan hệ dài hạn bằng attention |

---

### 3. Thực nghiệm và đánh giá
- **Chỉ số đánh giá**:
  - RMSE – Root Mean Squared Error
  - MAE – Mean Absolute Error
  - MAPE – Mean Absolute Percentage Error
  - R² – Hệ số xác định
- **Các giai đoạn đánh giá**:
  - Dự báo tập validation, test
  - Dự báo 30, 60, 90 ngày tương lai
- **Kết quả**:
  - Mỗi mô hình cho kết quả khác nhau tùy loại năng lượng
  - LSTM và LightGBM cho kết quả tốt nhất trong hầu hết các trường hợp

---

## Kết luận

Đề tài đã khảo sát và áp dụng nhiều mô hình dự đoán giá năng lượng trên dữ liệu thực tế, cho thấy tiềm năng lớn của học máy trong lĩnh vực tài chính – năng lượng. Các mô hình phi tuyến như LSTM, GRU và LightGBM có khả năng thích ứng tốt với dữ liệu biến động mạnh. Trong khi đó, Prophet và SARIMA cung cấp góc nhìn thống kê rõ ràng, dễ giải thích.

Đề xuất hướng phát triển tiếp theo:
- Kết hợp nhiều mô hình (ensemble)
- Sử dụng thêm dữ liệu kinh tế vĩ mô (GDP, CPI,...)
- Phân cụm đặc trưng để cải thiện hiệu suất mô hình

---

## Nhóm thực hiện – Nhóm 9
**Khoa:** Hệ thống Thông tin  
**Trường:** Đại học Công nghệ Thông tin – ĐHQG TP.HCM

| STT | MSSV     | Họ và tên               | Email                    |
|-----|----------|--------------------------|--------------------------|
| 1   | 21520414 | Trần Minh Quân           | 21520414@gm.uit.edu.vn   |
| 2   | 22520958 | Nguyễn Thị Hồng Ngọc     | 22520958@gm.uit.edu.vn   |
| 3   | 22520976 | Nguyễn Phan Thảo Nguyên  | 22520976@gm.uit.edu.vn   |
| 4   | 22520978 | Nguyễn Trung Nguyên      | 22520978@gm.uit.edu.vn   |
| 5   | 22521374 | Phạm Trần Dạ Thảo        | 22521374@gm.uit.edu.vn   |

---


