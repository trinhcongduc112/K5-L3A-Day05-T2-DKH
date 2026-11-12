# Mạch — Prototype LAB5, Track 2 Education

## Mở giao diện

Mở `index.html` bằng Chrome hoặc Edge. Giữ `index.html`, `styles.css`, `theme.css` và `app.js` trong cùng thư mục.

Không cần npm, API key hay backend. Font Be Vietnam Pro tải từ Google Fonts; khi offline giao diện dùng font hệ thống. Phiếu và FAQ lưu trong localStorage của trình duyệt; không gửi ra ngoài.

## Luồng demo

1. **Tài liệu có câu sai:** đọc cảnh báo và nguồn §3.3 → Gửi báo cáo cho TA → chỉnh câu hỏi/ghi chú → Xác nhận gửi → xem hàng chờ → Hoàn tác / Hủy phiếu nếu cần.
2. **Đăng FAQ:** chọn Đề xuất FAQ → chỉnh bản nháp → Gửi TA duyệt FAQ → Xác nhận → FAQ của lớp vẫn chưa có bản nháp.
3. Chọn **Góc TA** → Kiểm tra / Sửa & duyệt → sửa nội dung → đánh dấu đã kiểm tra → Duyệt & đăng FAQ → mở FAQ của lớp.
4. TA có thể từ chối kèm lý do, phản hồi phiếu báo cáo hoặc gỡ FAQ. Học viên có thể thu hồi đề xuất còn chờ.
5. **Kiểm tra bài 3:** không xác nhận đáp số; chỉ chỉ ra mục §3.2 và gợi ý bước đầu.
6. **Chưa rõ khái niệm:** hiện hai lựa chọn để học viên làm rõ câu hỏi.

## Phạm vi giả lập

- Các câu trả lời và kết quả tra cứu được viết sẵn, chọn theo tình huống hoặc từ khóa; đây không phải LLM và không có lời gọi AI thật.
- Gửi TA, duyệt, hủy và đăng FAQ chỉ thay đổi trạng thái trong trình duyệt. Nút chuyển vai trò dùng để demo, không phải cơ chế bảo mật/phân quyền thật.
- Mốc 23:00 ngày 12/11/2026 là bối cảnh demo cố định. Giờ trực là 08:00–22:00; không hứa TA trả lời đúng 08:00.
- Mỗi lượt hiện một ca hội thoại. Chưa có lịch sử chat đầy đủ hoặc thông báo ngoài trình duyệt.
- Hủy và thu hồi là luồng bổ sung do nhóm thiết kế, không phải khẳng định bộ tool gốc đã có API tương ứng.
- TA kiểm tra thủ công nội dung FAQ; checkbox không chứng minh nội dung đúng hoặc không lộ đáp số.

## Thiết kế §5

| Thành phần | Nguyên tắc theo spec của nhóm | Mức tự chủ |
|---|---|---|
| Nhãn trợ lý AI, giới hạn và giờ trực | G2: làm rõ giới hạn năng lực | Người dùng biết điều AI không làm được |
| Nguồn §3.3, tô câu cần xem lại, phản ví dụ | PAIR Explainability / Trust | Tra cứu chỉ đọc, tự làm |
| Thẻ xác nhận gửi TA | G10: giới hạn khi không chắc | Học viên duyệt trước khi gửi |
| Bản nháp chưa công khai, nút hủy | G10; quyền kiểm soát của người dùng | Soạn nháp tự làm, đảo được |
| Kiểm tra / Sửa & duyệt ở Góc TA | G10; người kiểm soát quyết định | TA duyệt trước khi đăng FAQ |

Nhãn cảnh báo dùng chữ và biểu tượng kèm màu vàng, không dựa riêng vào màu. Hành động chính dùng gradient tím–xanh, hành động phụ nền sáng, hủy/gỡ dùng đỏ trầm. Animation ngắn cho câu trả lời, trạng thái chờ và thông báo; tự giảm chuyển động theo thiết lập hệ điều hành.

Chọn bằng chứng nguồn và trạng thái cụ thể thay vì phần trăm độ tin cậy vì không có mô hình đo confidence. Tách bản nháp khỏi FAQ công khai thay vì đăng ngay kèm cảnh báo vì nhãn cảnh báo không thu hồi được kiến thức người khác đã đọc.

## Khác biệt cần thống nhất với §3–§4

- Thay “phản hồi sau 08:00” bằng giờ trực và “chưa xác định giờ trả lời”.
- Thay nút “tiếp tục với công thức gốc” bằng “Tiếp tục học”, tránh khuyến khích dùng kết luận sai.
- Trạng thái xác nhận lấy từ thao tác của prototype, không từ văn bản sinh bởi AI.

## Kiểm tra

- Cú pháp JavaScript: `node --check app.js`.
- Đã bấm thử trong trình duyệt: gửi phiếu, thu hồi, gửi duyệt FAQ, chặn duyệt khi chưa xác nhận kiểm tra, TA duyệt thành công.
- Cần phân biệt các bước kiểm tra giao diện này với việc đánh giá AI thật.
