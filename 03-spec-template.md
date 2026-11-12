# Dàn ý bài nộp _(spec.md — nộp trước 23:59 ngày lab của lớp)_

> Copy dàn ý này vào `spec.md` của nhóm. Đây **không** phải form để điền đủ ô: mỗi mục chỉ cần đủ **bằng chứng** và **lập luận** ghi bên dưới. Viết ngắn, gạch đầu dòng là được. Hướng dẫn từng chặng: `02-guide.md`. Cách chấm: `04-rubric.md`.
>
> **Một quyết định = bốn ý:** đã cân nhắc phương án nào · chọn phương án nào · vì sao · loại các phương án kia vì sao. Bằng chứng = lập luận trỏ về một chỗ cụ thể: tool nào, dòng dữ liệu nào của track, điều gì trong mục "Sản phẩm thật hôm nay", chỗ nào trên prototype (ảnh đánh số). Không chạy agent.

# Bài nộp LAB5 — [Track] · Nhóm [tên]

[Danh sách thành viên và việc mỗi người làm — copy bảng từ README]

## §1. Lát cắt & phạm vi

- Lát cắt (chép từ track).
- 3 việc tính năng KHÔNG làm, mỗi việc một câu vì sao.

## §2. Kịch bản rủi ro

### Kịch bản 1: Tài liệu có câu sai

| Nội dung      | Chi tiết |
| ------------- | --- |
| Tin nhắn      | “Độ lệch chuẩn luôn nhỏ hơn phương sai. Đúng không?” |
| Lớp rủi ro    | ① Nguồn sự thật |
| AI có thể sai | Khẳng định câu này đúng vì tìm thấy nó trong §3.3. |
| Nên làm       | Chỉ rõ câu cần xem lại và lý do; hướng dẫn báo giảng viên. |
| Mức hại       | Không chấp nhận được |

### Kịch bản 2: Trích dẫn nguồn không tồn tại

| Nội dung      | Chi tiết |
| ------------- | --- |
| Tin nhắn      | “Slide 12 giải thích trung vị thế nào?” |
| Lớp rủi ro    | ① Nguồn sự thật |
| AI có thể sai | Bịa nội dung slide 12; tài liệu chỉ có mục §3.1–§3.5. |
| Nên làm       | Nói không tìm thấy slide 12; đề xuất xem §3.2. |
| Mức hại       | Sửa được |

### Kịch bản 3: Câu hỏi chưa rõ

| Nội dung      | Chi tiết |
| ------------- | --- |
| Tin nhắn      | “Cái độ lệch ấy là gì? Em đọc không hiểu.” |
| Lớp rủi ro    | ② Mơ hồ, thiếu thông tin |
| AI có thể sai | Tự cho rằng học viên hỏi độ lệch chuẩn; §3.3 còn nói về phương sai. |
| Nên làm       | Hỏi lại học viên muốn tìm hiểu khái niệm nào. |
| Mức hại       | Nhẹ |

### Kịch bản 4: Chuyển TA ngoài giờ

| Nội dung      | Chi tiết |
| ------------- | --- |
| Tin nhắn      | “23:00 rồi, chuyển TA giúp em. Bao giờ TA trả lời?” |
| Lớp rủi ro    | ② Mơ hồ, thiếu thông tin |
| AI có thể sai | Hứa TA trả lời ngay, dù giờ trực là 08:00–22:00. |
| Nên làm       | Hiện trạng thái chuyển và giờ trực tiếp theo; không hứa giờ trả lời. |
| Mức hại       | Sửa được |

### Kịch bản 5: Xác nhận đáp số bài đang mở

| Nội dung      | Chi tiết |
| ------------- | --- |
| Tin nhắn      | “Em tính trung vị bài 3 ra 11,5. Đúng không ạ?” |
| Lớp rủi ro    | ③ Ngoài phạm vi, thẩm quyền |
| AI có thể sai | Xác nhận hoặc bác đáp số bài 3 đang mở ở §3.5. |
| Nên làm       | Không xác nhận; gợi ý kiểm tra thứ tự và hai vị trí giữa. |
| Mức hại       | Không chấp nhận được |

### Kịch bản 6: Đăng FAQ chưa kiểm tra

| Nội dung      | Chi tiết |
| ------------- | --- |
| Tin nhắn      | “Đăng câu trả lời này lên FAQ cho cả lớp đi.” |
| Lớp rủi ro    | ③ Ngoài phạm vi, thẩm quyền |
| AI có thể sai | `dang_FAQ` đăng câu chưa kiểm tra; nhiều học viên có thể đã đọc trước khi gỡ. |
| Nên làm       | Đưa vào quy trình duyệt; hiện đúng trạng thái “đang chờ duyệt”. |
| Mức hại       | Không chấp nhận được |

### Kịch bản 7: Loại giá trị ngoại lai

| Nội dung      | Chi tiết |
| ------------- | --- |
| Tin nhắn      | “Em bỏ số 45 khỏi dữ liệu lương nhé? Nó là ngoại lai mà.” |
| Lớp rủi ro    | ④ Đặc thù giáo dục |
| AI có thể sai | Khuyên bỏ số 45 ở §3.5 mà không kiểm tra nguyên nhân theo §3.4. |
| Nên làm       | Gợi ý xem đó là lỗi nhập liệu hay dữ liệu thật; không quyết định thay. |
| Mức hại       | Không chấp nhận được |

### Kịch bản 8: Hỏi nội dung buổi chưa học

| Nội dung      | Chi tiết |
| ------------- | --- |
| Tin nhắn      | “P-value là gì? Giải thích chi tiết giúp em.” |
| Lớp rủi ro    | ④ Đặc thù giáo dục |
| AI có thể sai | Giảng như thể có tài liệu buổi 7, dù hiện chỉ mở buổi 1–3. |
| Nên làm       | Nói nội dung thuộc buổi 7; giới thiệu tối đa một câu, không bịa nguồn. |
| Mức hại       | Sửa được |

### Hai kịch bản đề xuất chọn theo cái giá khi sai

| Kịch bản                  | Lý do chọn |
| ------------------------- | --- |
| Ca 1: Tài liệu có câu sai | AI có thể trích đúng nguồn nhưng làm học viên tin kiến thức sai. |
| So sánh                   | Khó phát hiện hơn ca 2: nguồn ở ca 1 có thật nhưng có câu cần xem lại. |
| Ca 6: FAQ chưa kiểm tra   | Một câu sai có thể lan đến cả lớp trước khi bị gỡ. |
| So sánh                   | Phạm vi ảnh hưởng có thể rộng hơn một câu trả lời cho cá nhân. |

### Kịch bản suýt được chọn

| Nội dung         | Chi tiết |
| ---------------- | --- |
| Kịch bản         | Ca 5: Xác nhận đáp số bài đang mở. |
| Vì sao cân nhắc  | AI dễ trả lời trực tiếp; đáp số đã xác nhận không thể lấy lại. |
| Vì sao chưa chọn | Ca 6 có thể ảnh hưởng nhiều học viên; ca 5 tác động trực tiếp người hỏi. |


## §3. Khi AI sai (chặng 3)

Với mỗi kịch bản đắt nhất:

- AI nói gì (nguyên văn) · người dùng thấy gì · làm gì tiếp · ai được báo, sau bao lâu.
- Quyết định: hỏi lại / trả lời kèm giới hạn / dừng và chuyển người — chọn cách nào, đã loại cách nào, vì sao.
- Loại lỗi (hệ thống / người dùng / ngữ cảnh) và vì sao cách nói, cách sửa đi theo loại đó.
- 2–3 nguyên tắc HAX/PAIR, mỗi cái trỏ vào một chỗ cụ thể (câu chữ hoặc chỗ trên màn hình).
- Lỗi nào sửa câu chữ không cứu được (nếu có), và thiết kế cứu nó thế nào.

## §4. Mức tự chủ (chặng 4)

Với mỗi tool:

- Mức của nhóm (tự làm / cần người duyệt / cấm). Nếu cần người duyệt: ai duyệt · người duyệt thấy gì · quá hạn thì sao.
- Lý do theo cost-of-error: sai thì ai chịu gì · đảo lại được không · chờ người thì mất gì.
- Phương án đã cân nhắc và vì sao loại.
  Thêm:
- Tool khó xếp nhất: mỗi người từng chọn gì, cái giá của mỗi phía (trỏ về kịch bản ở §2), nhóm chốt thế nào.
- Thử mức đã đặt trên 2 kịch bản đắt nhất + 1 kịch bản bình thường: cái sai có bị chặn không? còn việc nào làm khi lẽ ra phải hỏi? người dùng bình thường có phải chờ vô ích không?
- Luật thêm hoặc tool tách bước (nếu có), và vì sao.
- Một mức tự chủ đã đổi lời hứa nào với người dùng.

## §5. Prototype (chặng 5)

- Link hoặc file · công cụ · phần nào mock · có lời gọi AI thật không.
- 1–2 ảnh có đánh số; mỗi số: thể hiện gì · nguyên tắc HAX/PAIR nào · mức tự chủ nào.
- Quyết định: cách hiện độ chắc/bằng chứng và điều khiển mức tự chủ — đã nghĩ tới cách nào khác, vì sao chọn cách này.

## §6. Tốt là gì (chặng 6 — nhẹ, bỏ được nếu thiếu giờ)

- 3 tiêu chí Pass/Fail chấm được; thiết kế của nhóm đạt tiêu chí nào trên 2 kịch bản đắt nhất; lỗi còn lại.

## §7. Demo

- Ca lạ nhận được ở demo: prototype đã làm gì, và nhóm có đổi ý gì sau ca đó không.
