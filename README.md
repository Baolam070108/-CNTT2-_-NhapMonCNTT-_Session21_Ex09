# BÀI TỔNG HỢP – VOLTCHARGE

## 1. Vấn đề
Câu hỏi ban đầu quá chung chung, không có mã lỗi và thông tin thiết bị nên AI dễ đoán sai nguyên nhân (Hallucination).

## 2. Yêu cầu

**1.** Phân tích nguyên nhân vì sao câu hỏi *'AI ơi phần mềm trạm sạc của tôi bị hỏng rồi'* lại khiến AI đưa ra câu trả lời sai lệch (hiện tượng AI Hallucination)?

**2.** Soạn thảo một câu Prompt 3 Thành phần hoàn chỉnh, chuyên nghiệp dựa trên đoạn nhật ký lỗi trên để gửi cho Trợ lý AI (phân tách rõ 3 phần: \[Context\], \[Raw Error\], \[Instruction\]).

## 3. Cách làm

**Câu 1: Nguyên nhân AI trả lời sai**

Vì câu hỏi thiếu thông tin và mã lỗi cụ thể nên AI phải phỏng đoán, dẫn đến câu trả lời không chính xác.


**Câu 2: Prompt hoàn chỉnh**

Sử dụng Prompt 3 thành phần ở phần Yêu cầu phía trên.


**Câu 3: Giải thích lỗi**

Lỗi có nghĩa là ứng dụng không có quyền ghi dữ liệu vào file `session.log` trong thư mục `Program Files`.


**Câu 4: Ba bước khắc phục**

1. Kiểm tra quyền truy cập của ứng dụng.
2. Nhờ quản trị viên chạy ứng dụng bằng quyền Administrator.
3. Kiểm tra và cấp quyền ghi phù hợp cho thư mục `data`.

**Câu 5: Bảo vệ API Key**

Phải xóa hoặc che API Key trước khi gửi cho AI. Nếu đã bị lộ, cần báo quản trị viên để thu hồi và tạo mã mới.

**Lý do:** Tránh bị đánh cắp thông tin và truy cập trái phép vào hệ thống.
