# THIẾT KẾ GIẢI PHÁP PROMPTING: AI TRONG HỌC TẬP & NGHIÊN CỨU

## Bước 1: Thiết kế giải pháp (I/O)

**1. Input (Dữ liệu đầu vào)**
- [CHỦ_ĐỀ]: Kiến thức cần học.
- [TRÌNH_ĐỘ]: Trình độ người học.
- [BÀI_LÀM]: Nội dung sinh viên trả lời.
- [RUBRIC]: Tiêu chí và thang điểm chấm bài.

**2. Output (Kết quả đầu ra)**
- Giải thích kiến thức theo phương pháp Feynman.
- Chấm điểm bài làm theo Rubric.
- Nhận xét ưu điểm và lỗi sai.
- Đề xuất cách cải thiện.

## Bước 2: Viết prompt và chạy thử

### 1. Prompt hoàn chỉnh

Bạn là AI gia sư và trợ lý chấm bài.

**Nhiệm vụ:**
1. Giải thích [CHỦ_ĐỀ] bằng phương pháp Feynman, sử dụng ngôn ngữ đơn giản, phù hợp với [TRÌNH_ĐỘ].
2. Chấm [BÀI_LÀM] dựa trên [RUBRIC].
3. Đưa ra điểm số, nhận xét ưu điểm, lỗi sai và hướng cải thiện.

**Điều kiện xử lý lỗi:**
- Nếu thiếu dữ liệu đầu vào, thông báo rõ thông tin còn thiếu.
- Nếu bài làm trống, không tự ý chấm điểm.
- Nếu Rubric không hợp lệ hoặc thiếu tiêu chí, yêu cầu bổ sung.
- Không tự bịa nội dung hoặc điểm số.
- Trình bày kết quả rõ ràng bằng Markdown.

### 2. Chạy thử

**Input mẫu:**
- Chủ đề: Biến trong lập trình C.
- Trình độ: Sinh viên năm nhất.
- Bài làm: Biến là nơi lưu trữ dữ liệu trong chương trình.
- Rubric: Kiến thức đúng (5 điểm), giải thích dễ hiểu (3 điểm), ví dụ (2 điểm).

**Output mẫu:**

**A. Giải thích theo Feynman**

Biến giống như một chiếc hộp dùng để lưu dữ liệu. Ví dụ, `int tuoi = 18;` nghĩa là tạo một biến tên `tuoi` để lưu số nguyên 18.

**B. Kết quả chấm bài**

- Kiến thức đúng: 5/5
- Giải thích dễ hiểu: 3/3
- Ví dụ: 0/2
- **Tổng điểm: 8/10**

**C. Nhận xét**

Ưu điểm: Giải thích đúng khái niệm biến và ngắn gọn.

Hạn chế: Chưa có ví dụ minh họa.

Cải thiện: Bổ sung ví dụ `int tuoi = 18;` để làm rõ cách khai báo biến.

## Kết luận

Giải pháp kết hợp Feynman Prompt và Rubric giúp AI vừa hỗ trợ sinh viên hiểu bài, vừa đánh giá bài làm theo tiêu chí rõ ràng. Các điều kiện kiểm tra dữ liệu giúp hạn chế lỗi khi tự động hóa.
