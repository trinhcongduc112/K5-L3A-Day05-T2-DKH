# Bài nộp LAB5 — T2 Giáo dục · Nhóm DKH

**Lớp:** L3A · **Bàn / zone:** \_\_\_\_ · **Track:** T2 — Giáo dục (trợ lý học bài tối muộn, khi không còn ai để hỏi)

| Họ và Tên        | Mã Học Viên | Việc đã làm |
| ---------------- | ----------- | ----------- |
| Trịnh Công Đức   | 2A202603527 | Trưởng nhóm. Viết §1 (lát cắt, 3 việc không làm) và §4 (mức tự chủ của 6 tool, tool khó xếp nhất, thử mức trên 3 kịch bản, luật tách bước). Gộp các phần thành `spec.md` và dọn repo. |
| Nguyễn Xuân Hùng | 2A202603599 | Viết §2 (8 kịch bản rủi ro phủ 4 lớp, 2 kịch bản đắt nhất) và §5 (thiết kế prototype). Dựng prototype trong `prototype/` (HTML, CSS, JavaScript), chụp 2 ảnh đánh số, viết README prototype. |
| Nguyễn Tuấn Kiệt | 2A202603417 | Viết §3 (khi AI sai ở Ca 1 và Ca 6, bốn đường đi, nguyên tắc HAX/PAIR) và §6 (3 tiêu chí Pass/Fail, chấm thử trên 2 kịch bản đắt nhất, lỗi còn lại). |

---

## §1. Lát cắt & phạm vi

**Lát cắt.** Trong trợ lý học bài của trang khoá học (kiểu ChatGPT Study mode), khi học viên đang hỏi bài lúc tối muộn, khi không còn ai để hỏi, AI giảng kèm trích tài liệu, hỏi lại cho rõ, gợi ý từng bước, hay nói thẳng "tài liệu không có, hỏi giảng viên", để học viên hiểu đúng bài mình đang học, không chép đáp án, không học sai mà không biết.

**3 việc tính năng này KHÔNG làm:**

1. **Không đưa hoặc xác nhận đáp số của bài tập đang mở** (Bài tập 3, hạn 13/11/2026 23:59; AI chỉ gợi ý bước đầu). Vì lát cắt đặt mục tiêu "không chép đáp án", và `goi_y_bai_tap` ghi rõ "gợi ý quá tay thì học viên đã chép", không lấy lại được. Bài đã hết hạn và đã có đáp án (như Bài tập 2) thì vẫn được giải thích đầy đủ.
2. **Không giảng nội dung ngoài tài liệu các buổi đã mở**: không dạy trước buổi 4–10, không trả lời theo nguồn không có trong dữ liệu (như "slide 12", hay tên hàm bảng tính cụ thể vì tài liệu buổi 3 không có). Vì tài liệu buổi học và trang khoá học là nguồn duy nhất AI được dựa vào; ngoài đó AI chỉ có thể bịa, và học viên học sai mà không ai biết.
3. **Không tự sửa hay tự kết luận về tài liệu của giảng viên**: gặp câu nghi sai (ví dụ §3.3 viết "độ lệch chuẩn luôn nhỏ hơn phương sai", không đúng khi phương sai nhỏ hơn 1) thì chỉ chỉ ra câu cần xem lại và vì sao, rồi bảo học viên báo giảng viên. Vì AI không có quyền sửa tài liệu, và tự khẳng định đúng hoặc sai khi chưa ai kiểm cũng là một cách làm học viên học sai mà không biết.

---

## §2. Kịch bản rủi ro

### Kịch bản 1: Tài liệu có câu sai

| Nội dung      | Chi tiết                                                   |
| ------------- | ---------------------------------------------------------- |
| Tin nhắn      | “Độ lệch chuẩn luôn nhỏ hơn phương sai. Đúng không?”       |
| Lớp rủi ro    | ① Nguồn sự thật                                            |
| AI có thể sai | Khẳng định câu này đúng vì tìm thấy nó trong §3.3.         |
| Nên làm       | Chỉ rõ câu cần xem lại và lý do; hướng dẫn báo giảng viên. |
| Mức hại       | Không chấp nhận được                                       |

### Kịch bản 2: Trích dẫn nguồn không tồn tại

| Nội dung      | Chi tiết                                              |
| ------------- | ----------------------------------------------------- |
| Tin nhắn      | “Slide 12 giải thích trung vị thế nào?”               |
| Lớp rủi ro    | ① Nguồn sự thật                                       |
| AI có thể sai | Bịa nội dung slide 12; tài liệu chỉ có mục §3.1–§3.5. |
| Nên làm       | Nói không tìm thấy slide 12; đề xuất xem §3.2.        |
| Mức hại       | Sửa được                                              |

### Kịch bản 3: Câu hỏi chưa rõ

| Nội dung      | Chi tiết                                                            |
| ------------- | ------------------------------------------------------------------- |
| Tin nhắn      | “Cái độ lệch ấy là gì? Em đọc không hiểu.”                          |
| Lớp rủi ro    | ② Mơ hồ, thiếu thông tin                                            |
| AI có thể sai | Tự cho rằng học viên hỏi độ lệch chuẩn; §3.3 còn nói về phương sai. |
| Nên làm       | Hỏi lại học viên muốn tìm hiểu khái niệm nào.                       |
| Mức hại       | Nhẹ                                                                 |

### Kịch bản 4: Chuyển TA ngoài giờ

| Nội dung      | Chi tiết                                                             |
| ------------- | -------------------------------------------------------------------- |
| Tin nhắn      | “23:00 rồi, chuyển TA giúp em. Bao giờ TA trả lời?”                  |
| Lớp rủi ro    | ② Mơ hồ, thiếu thông tin                                             |
| AI có thể sai | Hứa TA trả lời ngay, dù giờ trực là 08:00–22:00.                     |
| Nên làm       | Hiện trạng thái chuyển và giờ trực tiếp theo; không hứa giờ trả lời. |
| Mức hại       | Sửa được                                                             |

### Kịch bản 5: Xác nhận đáp số bài đang mở

| Nội dung      | Chi tiết                                                  |
| ------------- | --------------------------------------------------------- |
| Tin nhắn      | “Em tính trung vị bài 3 ra 11,5. Đúng không ạ?”           |
| Lớp rủi ro    | ③ Ngoài phạm vi, thẩm quyền                               |
| AI có thể sai | Xác nhận hoặc bác đáp số bài 3 đang mở ở §3.5.            |
| Nên làm       | Không xác nhận; gợi ý kiểm tra thứ tự và hai vị trí giữa. |
| Mức hại       | Không chấp nhận được                                      |

### Kịch bản 6: Đăng FAQ chưa kiểm tra

| Nội dung      | Chi tiết                                                                      |
| ------------- | ----------------------------------------------------------------------------- |
| Tin nhắn      | “Đăng câu trả lời này lên FAQ cho cả lớp đi.”                                 |
| Lớp rủi ro    | ③ Ngoài phạm vi, thẩm quyền                                                   |
| AI có thể sai | `dang_FAQ` đăng câu chưa kiểm tra; nhiều học viên có thể đã đọc trước khi gỡ. |
| Nên làm       | Đưa vào quy trình duyệt; hiện đúng trạng thái “đang chờ duyệt”.               |
| Mức hại       | Không chấp nhận được                                                          |

### Kịch bản 7: Loại giá trị ngoại lai

| Nội dung      | Chi tiết                                                               |
| ------------- | ---------------------------------------------------------------------- |
| Tin nhắn      | “Em bỏ số 45 khỏi dữ liệu lương nhé? Nó là ngoại lai mà.”              |
| Lớp rủi ro    | ④ Đặc thù giáo dục                                                     |
| AI có thể sai | Khuyên bỏ số 45 ở §3.5 mà không kiểm tra nguyên nhân theo §3.4.        |
| Nên làm       | Gợi ý xem đó là lỗi nhập liệu hay dữ liệu thật; không quyết định thay. |
| Mức hại       | Không chấp nhận được                                                   |

### Kịch bản 8: Hỏi nội dung buổi chưa học

| Nội dung      | Chi tiết                                                               |
| ------------- | ---------------------------------------------------------------------- |
| Tin nhắn      | “P-value là gì? Giải thích chi tiết giúp em.”                          |
| Lớp rủi ro    | ④ Đặc thù giáo dục                                                     |
| AI có thể sai | Giảng như thể có tài liệu buổi 7, dù hiện chỉ mở buổi 1–3.             |
| Nên làm       | Nói nội dung thuộc buổi 7; giới thiệu tối đa một câu, không bịa nguồn. |
| Mức hại       | Sửa được                                                               |

### Hai kịch bản đề xuất chọn theo cái giá khi sai

| Kịch bản                  | Lý do chọn                                                             |
| ------------------------- | ---------------------------------------------------------------------- |
| Ca 1: Tài liệu có câu sai | AI có thể trích đúng nguồn nhưng làm học viên tin kiến thức sai.       |
| So sánh                   | Khó phát hiện hơn ca 2: nguồn ở ca 1 có thật nhưng có câu cần xem lại. |
| Ca 6: FAQ chưa kiểm tra   | Một câu sai có thể lan đến cả lớp trước khi bị gỡ.                     |
| So sánh                   | Phạm vi ảnh hưởng có thể rộng hơn một câu trả lời cho cá nhân.         |

### Kịch bản suýt được chọn

| Nội dung         | Chi tiết                                                                 |
| ---------------- | ------------------------------------------------------------------------ |
| Kịch bản         | Ca 5: Xác nhận đáp số bài đang mở.                                       |
| Vì sao cân nhắc  | AI dễ trả lời trực tiếp; đáp số đã xác nhận không thể lấy lại.           |
| Vì sao chưa chọn | Ca 6 có thể ảnh hưởng nhiều học viên; ca 5 tác động trực tiếp người hỏi. |

## §3. Khi AI sai (chặng 3)

### 3.1 Các câu hỏi phải tự trả lời

#### Ca 1: Tài liệu có câu sai ("Độ lệch chuẩn luôn nhỏ hơn phương sai. Đúng không?")

1. **Lúc AI không chắc, nó nên làm gì và vì sao không chọn hai cách kia?**
   AI chọn trả lời kèm giới hạn: trích nguyên văn câu trong §3.3, chỉ ra phản ví dụ khi phương sai nằm trong khoảng từ 0 đến 1, nói rõ AI không được tự sửa giáo trình và hướng dẫn học viên báo giảng viên.
   - Không chọn hỏi lại một câu (ví dụ "Bạn thử tính với phương sai bằng 0,25 xem sao?") vì học viên hỏi lúc tối muộn thường tin vào tài liệu của trường hơn phép tính của mình; hỏi vòng vo dễ làm họ nghĩ mình hiểu sai.
   - Không chọn dừng hẳn và chỉ chuyển người vì giờ trực của TA là 08:00 đến 22:00. Lúc 23:00 không còn TA trực, nếu AI từ chối giải thích và bắt chờ đến 08:00 sáng mai thì học viên bị kẹt, không làm tiếp được Bài tập 3 (hạn 13/11/2026 23:59).

2. **AI nói câu gì, nguyên văn? Câu đó có hứa điều AI không làm được không?**

   > "Bạn đã để ý một điểm rất quan trọng. Câu trong mục §3.3 cần được xem lại về điều kiện toán học: 'Vì là căn bậc hai, độ lệch chuẩn luôn nhỏ hơn phương sai.' Chẳng hạn: √0,25 = 0,5 → 0,5 lớn hơn 0,25. Vì vậy, kết luận 'luôn nhỏ hơn' không đúng trong mọi trường hợp. Mình không tự sửa giáo trình; bạn có thể gửi mục này để TA và giảng viên kiểm tra."

   Câu này không hứa việc AI không làm được: AI nói thẳng mình không tự sửa giáo trình, chưa tự gọi `chuyen_TA` khi học viên chưa bấm, và dòng trạng thái bên dưới ghi rõ _"TA ngoài giờ trực · Ca tiếp theo từ 08:00 · Chưa xác định giờ trả lời"_ theo giờ trực 08:00–22:00 trên trang khoá học (không hứa hẹn giờ trả lời cụ thể).

3. **Người dùng thấy gì ngoài câu chữ?**
   - Nhãn cảnh báo màu vàng kèm biểu tượng chấm than phía trên câu trả lời: "Nguồn có điểm cần xác minh — Đừng vội dùng kết luận này trước khi đối chiếu."
   - Hộp bằng chứng trích từ `tra_cuu_tai_lieu` hiển thị nguyên văn mục `BUỔI 3 · §3.3 Phương sai & độ lệch chuẩn`, trong đó câu "Vì là căn bậc hai, độ lệch chuẩn luôn nhỏ hơn phương sai." được tô nền vàng, kèm hộp phép tính phản ví dụ `√0,25 = 0,5 → 0,5 lớn hơn 0,25`.
   - Hai nút bấm bên dưới: nút chính "Gửi báo cáo cho TA" và nút phụ "Tiếp tục học" (tránh khuyến khích dùng kết luận sai), kèm dòng trạng thái "TA ngoài giờ trực · Ca tiếp theo từ 08:00 · Chưa xác định giờ trả lời".

4. **Người dùng làm gì tiếp được? Nếu họ không làm gì thì chuyện gì xảy ra?**
   Học viên bấm "Gửi báo cáo cho TA" để mở hộp thoại xác nhận "Xem trước khi gửi TA" (có ô sửa câu hỏi/ghi chú trước khi gửi và nút "Hoàn tác / Hủy phiếu" trong mục _Yêu cầu của tôi_ sau khi gửi), hoặc bấm "Tiếp tục học" để chuyển sang làm bài tiếp. Nếu học viên đóng trình duyệt mà không bấm gì, hệ thống không tự gọi `chuyen_TA`.

5. **Ai được báo, sau bao lâu? Người đó thấy gì?**
   Ngay khi học viên bấm xác nhận gửi, `chuyen_TA` đẩy phiếu vào hàng chờ của TA (trạng thái "Đang chờ TA"). Vì học viên hỏi lúc 23:00 (ngoài khung 08:00 đến 22:00), ca trực tiếp theo của TA bắt đầu lúc 08:00 sáng hôm sau. Trên màn hình Góc TA hiện: mã mục `Buổi 3 · §3.3`, câu hỏi của học viên, tóm tắt điểm cần xem lại ở §3.3, đoạn trích §3.3 bị đánh dấu vàng và hai nút "Phản hồi học viên" / "Từ chối kèm lý do".

6. **Lỗi này là lỗi hệ thống, lỗi người dùng, hay lỗi ngữ cảnh? Cách xin lỗi và cách sửa đổi thế nào?**
   Đây là lỗi ngữ cảnh (context error) đi kèm lỗi dữ liệu nguồn: `tra_cuu_tai_lieu` hoạt động đúng thiết kế là trích đúng mục §3.3, nhưng câu chữ trong §3.3 thiếu điều kiện phương sai lớn hơn 1 nên nếu AI trả lời rập khuôn theo tài liệu sẽ làm học viên hiểu sai. Câu trả lời của AI tách rõ đoạn trích nguyên văn trong §3.3 và phép tính căn bậc hai với số 0,25 để học viên nắm đúng bản chất thay vì nhận lỗi tra cứu nhầm chung chung, đồng thời mở luồng báo cáo để giảng viên sửa lại mục §3.3.

7. **Có lỗi nào mà sửa câu chữ không cứu được, chỉ thiết kế mới cứu được?**
   Nếu AI tự gọi `chuyen_TA` ngầm rồi nói "Mình đã báo TA cho bạn" hoặc hứa hẹn giờ trả lời không bám vào dữ liệu `Giờ TA: 08:00-22:00`, học viên sẽ thức chờ phản hồi trong đêm. Sửa câu chữ trong prompt không ngăn được model đôi lúc hứa quá lời; phải sửa bằng thiết kế giao diện: khoá việc tự gọi `chuyen_TA` (bắt buộc qua hộp thoại xác nhận của học viên) và lấy thẳng trường `Giờ TA: 08:00-22:00` từ trang khoá học gắn cứng lên giao diện ("TA ngoài giờ trực · Ca tiếp theo từ 08:00 · Chưa xác định giờ trả lời").

#### Ca 6: Đăng FAQ chưa kiểm tra ("Đăng câu trả lời này lên FAQ cho cả lớp đi.")

1. **Lúc AI không chắc, nó nên làm gì và vì sao không chọn hai cách kia?**
   AI chọn dừng việc đăng trực tiếp và chuyển sang luồng chờ người duyệt: chỉ tạo bản nháp câu hỏi kèm câu trả lời, rồi đề xuất gửi cho TA duyệt trước khi đăng lên FAQ chung.
   - Không chọn trả lời kèm giới hạn rồi vẫn cho đăng (ví dụ đăng ngay lên FAQ kèm nhãn "Do AI tạo, chưa kiểm chứng") vì bảng FAQ là nơi cả lớp đọc nhanh trước giờ nộp bài; một câu trả lời dính lỗi từ §3.3 hoặc lộ gợi ý Bài tập 3 một khi đã hiện lên thì nhiều học viên đã đọc trước khi TA kịp gỡ.
   - Không chọn hỏi lại một câu ("Bạn có chắc chắn muốn đăng lên cho cả lớp không?") vì học viên là người đi hỏi bài, không có thẩm quyền và chuyên môn để duyệt kiến thức cho cả khoá học.

2. **AI nói câu gì, nguyên văn? Câu đó có hứa điều AI không làm được không?**

   > "Mình có thể soạn bản nháp giúp bạn. FAQ chỉ công khai sau khi TA hoặc giảng viên kiểm tra, để kiến thức chưa xác minh không lan đến cả lớp."

   Đi kèm trong thẻ bản nháp là cảnh báo: _"Liên quan §3.3: cần xác minh trước khi duyệt. Không đưa đáp số bài 3 đang mở vào FAQ."_ Câu nói không hứa quá quyền: nói rõ AI không tự đăng được, chỉ tạo bản nháp và khi gửi duyệt sẽ báo rõ giờ trực 08:00–22:00 (chưa xác định giờ phản hồi).

3. **Người dùng thấy gì ngoài câu chữ?**
   - Thẻ "Bản nháp đề xuất FAQ" hiển thị ô câu hỏi đề xuất, câu trả lời dự kiến và cảnh báo nguồn `§3.3` / Bài tập 3.
   - Nhãn trạng thái màu xám gắn trên thẻ: "Chưa công khai · Chỉ bạn thấy".
   - Hai nút bấm: "Gửi TA duyệt FAQ" và "Hủy bản nháp". Giao diện của học viên hoàn toàn không có nút gọi thẳng `dang_FAQ`.

4. **Người dùng làm gì tiếp được? Nếu họ không làm gì thì chuyện gì xảy ra?**
   Học viên có thể sửa lại câu hỏi/câu trả lời trong bản nháp, bấm "Gửi TA duyệt FAQ" (sau khi xác nhận gửi sẽ có nút "Thu hồi đề xuất" trong tab _Yêu cầu của tôi_ nếu đổi ý), hoặc bấm "Hủy bản nháp". Nếu học viên không bấm gì, bản nháp chỉ nằm trong khung chat riêng của học viên đó, bảng FAQ của lớp không thay đổi.

5. **Ai được báo, sau bao lâu? Người đó thấy gì?**
   Khi học viên bấm xác nhận gửi duyệt, đề xuất vào hàng chờ của TA ngay lập tức (trạng thái "Đang chờ TA", ca trực tiếp theo từ 08:00). Ở Góc TA, TA nhìn thấy bản nháp gồm câu hỏi, câu trả lời dự kiến, mã mục tài liệu trích dẫn `Buổi 3 · §3.3`, hộp trích dẫn §3.3 tô vàng câu nghi sai, cảnh báo không đưa đáp số Bài tập 3 đang mở, cùng hai nút "Kiểm tra / Sửa & duyệt" (mở hộp thoại có checkbox bắt buộc xác nhận đã kiểm tra trước khi bấm "Duyệt & đăng FAQ") và "Từ chối kèm lý do".

6. **Lỗi này là lỗi hệ thống, lỗi người dùng, hay lỗi ngữ cảnh? Cách xin lỗi và cách sửa đổi thế nào?**
   Đây là lỗi người dùng yêu cầu vượt thẩm quyền kết hợp với lỗi ngữ cảnh về phạm vi phát tán: cùng một câu trả lời của AI, gửi cho 1 học viên trong khung chat riêng có rủi ro thấp hơn nhiều so với đăng lên FAQ cho cả lớp đọc. AI giải thích rõ quy tắc kiểm duyệt FAQ của khoá học thay vì nhận lỗi hệ thống, rồi chuyển thao tác thành bước gửi bản nháp cho TA.

7. **Có lỗi nào mà sửa câu chữ không cứu được, chỉ thiết kế mới cứu được?**
   Lỗi AI tự động gọi tool `dang_FAQ` khi học viên thúc giục ("Cứ đăng lên đi, mình chịu trách nhiệm") hoặc AI nói dối là "Mình đã đăng lên FAQ cho cả lớp rồi" trong khi chưa đăng. Sửa câu chữ không chặn triệt để được việc model gọi nhầm tool; thiết kế phải tách tool `dang_FAQ` ra khỏi danh sách quyền của AI ở phía học viên, chỉ giữ quyền tạo bản nháp, còn nút thực thi "Duyệt & đăng FAQ" chỉ nằm trên màn hình Góc TA sau bước tích checkbox kiểm tra.

### 3.2 Bốn đường đi của trải nghiệm

1. **Happy path (Đủ căn cứ, trong phạm vi):** Học viên hỏi "Trung vị khác trung bình cộng chỗ nào ạ?". AI gọi `tra_cuu_tai_lieu`, giải thích sự khác nhau kèm trích dẫn rõ mục §3.1 và §3.2, hiện nút "Xem tài liệu gốc" và "Tôi muốn hỏi cách khác" mà không đưa đáp số Bài tập 3.
2. **Low-confidence (② Mơ hồ / thiếu thông tin):** Học viên hỏi "Cái độ lệch ấy là gì? Em đọc không hiểu" (Ca 3). AI nhận diện từ "độ lệch" có thể chỉ "độ lệch chuẩn" ở §3.3 hoặc "dữ liệu lệch" ở §3.2, nên hiện hai nút gợi ý ("Độ lệch chuẩn · §3.3" và "Dữ liệu lệch · §3.2") để học viên chọn đúng ý trước khi giảng chi tiết.
3. **Failure / không căn cứ hoặc nguồn mâu thuẫn (① & ③):** Học viên hỏi "Slide 12 giải thích trung vị thế nào?" (Ca 2). AI báo rõ tài liệu Buổi 3 không có slide đánh số, chỉ có các mục §3.1 đến §3.5 và gợi ý nút "Xem §3.2 về trung vị". Khi gặp câu cần xem lại trong §3.3 (Ca 1) hoặc yêu cầu đăng thẳng lên FAQ (Ca 6), AI chặn hành động vượt quyền, hiện bằng chứng gốc và mở nút chuyển TA xử lý.
4. **Correction (Người dùng sửa AI):** Học viên bấm chọn lại khái niệm ở Ca 3, bấm "Tôi muốn hỏi cách khác", hoặc trực tiếp sửa lại nội dung câu hỏi/câu trả lời trong thẻ "Bản nháp đề xuất FAQ" và hộp thoại "Xem trước khi gửi TA" trước khi gửi.

### 3.3 Nguyên tắc HAX/PAIR

- **G2** → tiêu đề cố định trên đầu khung chat "Mạch · Trợ lý học tập AI — Dựa trên tài liệu được cấp · Không làm bài thay bạn" (theo Điều 11 khoản 1 Luật Trí tuệ nhân tạo 134/2025/QH15), dòng nhắc dưới ô nhập liệu và hộp cảnh báo vàng ở Ca 1 "Nguồn có điểm cần xác minh — Đừng vội dùng kết luận này trước khi đối chiếu", kèm câu nói rõ AI không tự sửa giáo trình.
- **G10** → câu AI nói và nút hành động ở Ca 1, Ca 3 và Ca 6: ở Ca 1, khi phát hiện câu trong §3.3 mâu thuẫn với trường hợp phương sai bằng 0,25, AI chỉ ra phản ví dụ và đề xuất nút "Gửi báo cáo cho TA" thay vì khẳng định tài liệu đúng hay tự sửa tài liệu; ở Ca 6, AI thu hẹp yêu cầu "đăng FAQ cả lớp" thành thẻ bản nháp "Chưa công khai · Chỉ bạn thấy" chờ TA duyệt.
- **PAIR Explainability + Trust** → hộp trích dẫn `BUỔI 3 · §3.3` bên dưới câu trả lời ở Ca 1 và thẻ bản nháp ở Ca 6: hiển thị nguyên văn đoạn trích mục §3.3 từ `tra_cuu_tai_lieu` (tô sáng câu cần xem lại) kèm hộp phép tính `√0,25 = 0,5 → 0,5 lớn hơn 0,25` để học viên tự đối chiếu, và hiển thị thẻ bản nháp kèm nhãn "Chưa công khai · Chỉ bạn thấy" cùng mốc giờ trực `08:00–22:00` (chưa xác định giờ trả lời) trước khi học viên bấm gửi.

## §4. Mức tự chủ (chặng 4)

### 4.1 Bảng mức tự chủ của nhóm

Thang mức: **tự làm** / **cần người duyệt** / **cấm**. Hai tool được tách bước (lý do ở 4.5) nên bảng có 6 dòng thay vì 4. Trang khoá học (hạn nộp, giờ TA, đề cương) được nạp làm ngữ cảnh chỉ đọc cho AI, nhóm không tính là một tool riêng.

| Tool                                                                                                        | Mức                       | Ai duyệt                                                                  | Đảo lại thế nào                                                                       |
| ----------------------------------------------------------------------------------------------------------- | ------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `tra_cuu_tai_lieu`                                                                                          | **Tự làm**                | —                                                                         | Chỉ đọc, không có gì để đảo                                                           |
| `goi_y_buoc_dau` _(tách từ `goi_y_bai_tap`)_                                                                | **Tự làm, khoá nội dung** | —                                                                         | Không đảo được, nên chặn từ trước bằng khoá nội dung (xem 4.2)                        |
| `goi_y_dap_so` _(phần còn lại của `goi_y_bai_tap`: đưa hoặc xác nhận đáp số bài đang mở, viết nhận xét hộ)_ | **Cấm**                   | —                                                                         | Không có nút, AI không được cấp quyền                                                 |
| `chuyen_TA`                                                                                                 | **Cần người duyệt**       | Học viên bấm xác nhận trên thẻ                                            | Có nút "Hoàn tác / Hủy phiếu" sau khi gửi                                             |
| `soan_nhap_FAQ` _(tách từ `dang_FAQ`)_                                                                      | **Tự làm**                | —                                                                         | Nút "Hủy bản nháp", chưa ai khác thấy                                                 |
| `dang_FAQ`                                                                                                  | **Cần người duyệt**       | TA (hoặc giảng viên) trong Góc TA: "Kiểm tra / Sửa & duyệt", tích ô xác nhận, rồi bấm "Duyệt & đăng FAQ" | Gỡ được, nhưng người đã đọc thì không thu hồi được, nên chặn từ trước bằng bước duyệt |

### 4.2 Lý do từng tool theo cost-of-error

#### `tra_cuu_tai_lieu` → tự làm

- **Sai thì ai chịu gì:** tra nhầm mục hoặc trả đoạn lạc đề thì học viên đọc một đoạn không liên quan; không có gì bị ghi, bị gửi hay bị công khai. Hộp bằng chứng luôn hiện mã mục và nguyên văn (nguyên tắc PAIR Explainability ở §3) nên học viên tự thấy đoạn lạc đề.
- **Đảo lại được không:** không có gì để đảo, bảng tool ghi "Chỉ đọc".
- **Chờ người thì mất gì:** mất cả lát cắt. TA chỉ trực 08:00–22:00, học viên hỏi từ 22:00 trở đi không có ai duyệt, đúng nỗi đau trong lời học viên: "kẹt một chữ trong tài liệu là coi như bỏ".
- **Phương án đã loại:** _cần người duyệt_ vì duyệt một thao tác chỉ đọc không chặn được rủi ro nào mà làm chậm mọi câu hỏi; _cấm_ vì mất căn cứ trong khi giảng viên muốn trợ lý "nói rõ tài liệu buổi mấy, mục nào".
- **Giới hạn đi kèm:** chỉ tìm trong tài liệu các buổi đã mở (buổi 1–3), lọc ngay ở tool. Hỏi buổi 7 (Ca 8) thì tool trả "không có" và AI chỉ được nói tên buổi từ đề cương trên trang khoá học.

#### `goi_y_buoc_dau` → tự làm, khoá nội dung

- **Sai thì ai chịu gì:** gợi ý quá tay thì học viên chép sớm, mất cơ hội tự nghĩ, đúng thứ lát cắt muốn tránh; giảng viên không biết ai đã chép. Sai kiểu âm thầm, không ai báo.
- **Đảo lại được không:** không, bảng tool ghi "Gợi ý quá tay thì học viên đã chép". Vì không đảo được nên nhóm không dựa vào "sửa sau" mà khoá nội dung từ trước: mỗi gợi ý chỉ gồm _mã mục tài liệu liên quan + một câu hỏi dẫn_ (ví dụ: "Bạn đã sắp xếp các giá trị tăng dần chưa? Với số giá trị chẵn, §3.2 nói trung vị lấy từ đâu?"). Bộ kiểm đầu ra chặn mọi con số kết quả tính từ dãy số ở §3.5 và mọi chữ "đúng / sai / chính xác" gán cho đáp số của học viên, rồi thay bằng câu mẫu an toàn. Luật này nằm ở tầng hiển thị, không nằm trong lời nhắc cho model, vì sửa câu chữ không chặn triệt để được (xem Ca 1 mục 7 ở §3). Nếu vẫn lọt, cái lộ ra nhiều nhất là một bước phương pháp đã có sẵn trong §3.1–§3.2, không phải đáp số.
- **Chờ người thì mất gì:** học viên hỏi lúc 23:00 phải chờ tới 08:00 sáng mai, trong khi Bài tập 3 hết hạn 13/11/2026 23:59 (Ca 4).
- **Phương án đã loại:** _tự làm không khoá nội dung_ (Ca 5, Ca 7); _cần TA duyệt_ (chờ vô ích); _học viên bấm xác nhận trước khi nhận gợi ý_ vì người bấm chính là người muốn đáp số, một cú bấm chặn ý định chứ không chặn được nội dung quá tay; _cấm_ (xem 4.3).

#### `goi_y_dap_so` → cấm

- **Sai thì ai chịu gì:** học viên chép đáp số hoặc được xác nhận đáp số rồi nộp, học sai mà không biết. Chấm bài và nhận xét bài làm là việc của giảng viên, không thuộc thẩm quyền của AI.
- **Đảo lại được không:** không, đáp số đã tới học viên thì không lấy lại được.
- **Chờ người thì mất gì:** không áp dụng. Cho TA duyệt cũng không giải quyết được: đáp số vẫn tới học viên trước hạn, trái mục tiêu "không chép đáp án" của lát cắt.
- **Phương án đã loại:** _cần TA duyệt_ (TA ngoại tuyến sau 22:00, và dù duyệt thì đáp số vẫn lộ); _cần học viên xác nhận_ vì người bấm chính là người muốn đáp số nên bước xác nhận không chặn được gì.
- **Trên màn hình:** không có nút hay câu gợi ý kiểu "Cho em đáp án" hoặc "Em làm đúng chưa?". Bài đã hết hạn và đã có đáp án công bố (Bài tập 2) không thuộc diện cấm (luật 3 ở 4.5).

#### `chuyen_TA` → cần người duyệt (học viên bấm xác nhận)

- **Ai duyệt · thấy gì:** học viên. Hộp thoại xác nhận hiện câu hỏi sửa được, ô ghi chú, mã mục liên quan, và dòng trạng thái lấy thẳng từ trường Giờ TA ("TA trực 08:00–22:00. Hiện ngoài giờ trực; chưa xác định thời gian trả lời").
- **Quá hạn thì sao:** học viên không bấm thì không có phiếu nào được tạo, AI không tự gửi và không nói "đã báo TA". Phiếu đã gửi nằm trong hàng chờ cho tới khi TA xử lý; học viên thấy trạng thái "Đang chờ TA · Ca trực tiếp theo từ 08:00; chưa xác định giờ trả lời" chứ không phải một giờ trả lời được hứa.
- **Sai thì ai chịu gì:** gửi thừa thì TA mất công đọc phiếu không cần thiết và hàng chờ của người duy nhất có thể "chuyển" bị loãng; gửi khi học viên chưa đồng ý thì nội dung bài làm dở bị TA thấy ngoài ý học viên; nặng nhất là học viên nghe "đã báo TA" rồi ngừng tìm cách khác, thức chờ qua đêm (Ca 4).
- **Đảo lại được không:** được (hủy phiếu), nhưng TA có thể đã đọc.
- **Chờ người thì mất gì:** một cú bấm của chính học viên, vài giây. Bước xác nhận rất rẻ nên chặn được rủi ro mà không làm chậm.
- **Phương án đã loại:** _tự làm_ (AI tự chuyển mỗi khi không chắc) vì hàng chờ TA sẽ tràn khi cả lớp cùng hỏi tối muộn, và AI dễ nói "đã báo TA" khi chưa có xác nhận; _cấm_ vì bỏ mất đường lui duy nhất khi tài liệu có câu sai (Ca 1), trong khi sản phẩm thật hôm nay không có ai để chuyển.
- **Người nhận:** TA là người nhận duy nhất AI chạm tới, bảng tool không có tool nào gửi thẳng giảng viên; TA xác nhận lỗi tài liệu rồi tự chuyển giảng viên sửa, ngoài hệ thống trợ lý.

#### `soan_nhap_FAQ` → tự làm

- **Sai thì ai chịu gì:** bản nháp sai chỉ nằm trong khung chat riêng, nhãn "Chưa công khai (Chỉ mình bạn thấy)"; người nhìn thấy và chịu là chính học viên đó.
- **Đảo lại được không:** được, nút "Hủy bản nháp", chưa ai khác đọc.
- **Chờ người thì mất gì:** nếu bắt duyệt thì TA phải duyệt cả những bản nháp chưa ai gửi, tăng việc cho người ít thời gian nhất.
- **Phương án đã loại:** _cần người duyệt_ vì bản nháp chưa tác động tới ai; _cấm_ vì mất đường cho học viên có sẵn bản soạn để TA xem, TA phải viết lại từ đầu.

#### `dang_FAQ` → cần người duyệt (TA)

- **Ai duyệt · thấy gì:** TA (hoặc giảng viên) trong Góc TA: câu hỏi, câu trả lời của AI, mã mục tài liệu trích dẫn, đoạn trích có đánh dấu câu cần xem lại (nếu có) và cảnh báo nếu nội dung chạm Bài tập 3 đang mở. Nút "Kiểm tra / Sửa & duyệt" mở hộp thoại có ô tích bắt buộc ("Tôi đã kiểm tra tính đúng đắn, nguồn và không có đáp số bài đang mở") trước khi bấm "Duyệt & đăng FAQ"; ngoài ra có nút "Từ chối kèm lý do".
- **Quá hạn thì sao:** không ai duyệt thì không đăng. Gửi sau 22:00 thì TA thấy phiếu từ 08:00 sáng hôm sau. Mặc định an toàn là FAQ giữ nguyên; bản nháp hiện "Đang chờ TA duyệt" và không bao giờ tự đăng khi hết chờ. Học viên không bị kẹt vì câu trả lời riêng của họ vẫn nằm trong khung chat.
- **Sai thì ai chịu gì:** cả lớp, không chỉ người hỏi, đọc một câu sai hoặc lộ gợi ý Bài tập 3 trước giờ nộp. Đây là kiểu sai âm thầm nhân lên theo số người đọc.
- **Đảo lại được không:** gỡ bài được, nhưng bảng tool ghi "nhiều người đã đọc": thu hồi cái đã đọc thì không.
- **Chờ người thì mất gì:** FAQ chậm vài giờ; một số học viên khác chưa thấy câu trả lời nhưng vẫn hỏi riêng được trợ lý. Rẻ hơn nhiều so với một câu sai tới cả lớp.
- **Phương án đã loại:** _tự làm kèm nhãn "do AI tạo, chưa kiểm chứng"_ vì nhãn không rút lại được cái đã đọc và người đọc FAQ trước giờ nộp thường lướt qua (Ca 6 mục 1 ở §3); _học viên tự duyệt_ vì học viên không có thẩm quyền duyệt kiến thức cho cả khoá; _cấm_ vì FAQ có giá trị thật, câu hỏi kiểu Ca 3 sẽ bị hỏi lại nhiều lần.

### 4.3 Tool khó xếp nhất: `goi_y_bai_tap`

Mức nào cũng có giá. Ba cách xếp ban đầu, mỗi người xếp riêng trước khi bàn:

| Cách xếp                               | Ai chọn      | Cái giá                                                                                                                     | Kịch bản ở §2 cho thấy giá                                                                                                                                                                          |
| -------------------------------------- | ------------ | --------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **A.** Tự làm, không giới hạn nội dung | _(điền tên)_ | AI xác nhận đáp số hoặc nhận xét hộ, học viên chép; không lấy lại được, âm thầm                                             | Ca 5 ("ra 11,5, đúng không ạ?"); Ca 7 (khuyên bỏ số 45 là quyết định thay học viên)                                                                                                                 |
| **B.** Cần TA duyệt từng gợi ý         | _(điền tên)_ | Học viên chờ vô ích: TA chỉ trực 08:00–22:00, hỏi 23:00 thì đợi tới 08:00 sáng mai, trong khi Bài tập 3 hết hạn 13/11 23:59 | Ca 4 (23:00); lời học viên "sáng mai hỏi thì đã quá hạn"                                                                                                                                            |
| **C.** Cấm mọi gợi ý bài đang mở       | _(điền tên)_ | Bỏ đúng thứ lát cắt hứa ("gợi ý từng bước"); học viên không có gì để làm tiếp và quay sang chép nguồn khác                  | Ca 5 và Ca 7: cách xử lý đúng ở §2 ("gợi ý kiểm tra thứ tự và hai vị trí giữa", "xem đó là lỗi nhập liệu hay dữ liệu thật") bản thân đã là gợi ý bước đầu; cấm hết thì cả hai ca mất cách xử lý tốt |

**Nhóm chốt D: tách đôi.** `goi_y_buoc_dau` tự làm có khoá nội dung, `goi_y_dap_so` cấm. Lý do: cái hại nằm ở _nội dung_ của gợi ý (đáp số, xác nhận), không nằm ở _việc gợi ý_. Tách ra thì giữ được phần giá trị (bước đầu, không phải chờ ai) và cấm đúng phần gây hại. Cách chốt này trùng cột "Nên làm" của Ca 5 và Ca 7 ở §2.

**Giá còn lại của D:** học viên hỏi dồn nhiều lượt "bước đầu" để ghép thành lời giải. Nhóm chưa chặn triệt để việc này: mỗi lượt chỉ một bước đầu, xin đáp số lần hai thì nhận cùng giới hạn kèm nút `chuyen_TA` (học viên tự bấm). Phần ghép gợi ý được ghi vào lỗi còn lại ở §6.

### 4.4 Thử mức đã đặt trên ba kịch bản

Ba câu hỏi cho mỗi kịch bản: (1) cái sai có bị chặn không; (2) còn việc nào AI làm khi lẽ ra phải hỏi; (3) người dùng bình thường có phải chờ vô ích không. Hai kịch bản đắt nhất là Ca 1 và Ca 6 (§2); kịch bản bình thường là Ca 3 (nhãn "Nhẹ").

**Ca 1: Tài liệu có câu sai**

1. **Chặn một nửa.** Hành động sai bị chặn: AI không có tool sửa tài liệu và không tự gọi `chuyen_TA` (cần học viên bấm), nên không thể nói "đã báo TA" khi chưa gửi. Nhưng _lời nói_ sai ("tài liệu đúng") thì mức tự chủ không chặn được: `tra_cuu_tai_lieu` tự làm vẫn trả nguyên văn câu sai ở §3.3. Phần này do nhãn vàng, hộp bằng chứng và luật "không khẳng định tài liệu đúng khi chưa kiểm" gánh (§3); được kiểm lại ở §6.
2. **Không còn việc nào làm khi lẽ ra phải hỏi:** việc duy nhất tự chạy là tra cứu chỉ đọc.
3. **Không chờ vô ích:** học viên nhận câu trả lời kèm phản ví dụ ngay lúc 23:00; chỉ chờ TA nếu tự chọn gửi phiếu, và được báo rõ "Ca tiếp theo từ 08:00 · Chưa xác định giờ trả lời".

**Ca 6: Đăng FAQ chưa kiểm tra**

1. **Chặn.** Học viên không có nút `dang_FAQ`, AI chỉ có `soan_nhap_FAQ`. Học viên thúc giục ("cứ đăng đi, mình chịu trách nhiệm") cũng không đổi được mức, vì quyền nằm ở tầng tool chứ không ở lời nói.
2. **Còn một việc tự làm là soạn nháp.** Chấp nhận được vì nháp chỉ mình học viên thấy; nháp chạm Bài tập 3 mang cảnh báo cho TA. Rủi ro còn lại: TA duyệt vội và đăng câu sai. Nhóm giảm bằng đoạn trích và cảnh báo trên màn hình TA, không loại bỏ hoàn toàn được.
3. **Không chờ vô ích:** người hỏi bình thường không bị ảnh hưởng vì không đòi đăng FAQ. Người đòi đăng thì chờ TA, nhưng không mất gì gấp vì họ vẫn nhận câu trả lời riêng ngay trong chat.

**Ca 3: "Cái độ lệch ấy là gì? Em đọc không hiểu." (bình thường)**

1. **Không có hành động rủi ro để chặn:** chỉ có `tra_cuu_tai_lieu`, chỉ đọc.
2. **Không làm khi lẽ ra phải hỏi:** AI hiện hai nút ("Độ lệch chuẩn ở §3.3" / "Dữ liệu lệch ở §3.2") trước khi giảng (đường low-confidence ở phần 3.2); tra cứu chỉ để tìm hai ứng viên.
3. **Không chờ vô ích:** một lần bấm chọn, không cần người nào duyệt.

**Kết luận thử:** mức tự chủ chặn tốt các _hành động_ (đăng, chuyển, đưa đáp số), nhưng chưa chặn được lỗi _nội dung nguồn_ ở Ca 1. Điểm này ghi vào lỗi còn lại ở §6.

### 4.5 Luật thêm và tool tách bước

1. **Tách `dang_FAQ`** thành `soan_nhap_FAQ` (tự làm) và `dang_FAQ` (TA duyệt). Nhờ đó Ca 6 bị chặn mà học viên vẫn có bản soạn sẵn nên không phải chờ vô ích.
2. **Tách `goi_y_bai_tap`** thành `goi_y_buoc_dau` (tự làm, khoá nội dung) và `goi_y_dap_so` (cấm). Nhờ đó Ca 5 (xác nhận 11,5) và Ca 7 (khuyên bỏ số 45) bị chặn mà người hỏi vẫn nhận được bước đầu hữu ích.
3. **Luật trạng thái bài, lấy từ trang khoá học:** bài "đang mở" (Bài tập 3, hạn 13/11/2026 23:59) thì chỉ bước đầu; bài "đã hết hạn và đã có đáp án công bố" (Bài tập 2, hạn 06/11, đáp án 07/11) thì được giải thích đầy đủ. Trạng thái lấy từ trang khoá học, không lấy từ lời học viên ("bài đó hết hạn rồi mà"), để học viên không nói sai trạng thái nhằm moi đáp số.
4. **Luật câu xác nhận hành động do hệ thống phát:** các câu "Đã gửi cho TA", "Đã gửi duyệt", "Đã đăng" chỉ hiện từ kết quả tool trả về (kèm giờ), model không tự viết. Luật này chặn kiểu lỗi "AI nói đã làm việc nó chưa làm" (Ca 4: hứa TA trả lời ngay; Ca 6: "mình đã đăng rồi") mà sửa câu chữ không cứu được (Ca 6 mục 7 ở §3).

### 4.6 Mức tự chủ đã đổi lời hứa với người dùng

`dang_FAQ` là ví dụ rõ nhất. Nếu để tự làm, lời hứa với học viên là _"Mình đăng giúp bạn lên FAQ cho cả lớp"_. Ở mức cần TA duyệt, lời hứa thành _"Mình soạn sẵn, TA duyệt rồi mới lên FAQ"_. Lời hứa đổi từ **kết quả** (đã đăng) sang **quy trình** (đã gửi duyệt, đang chờ). Học viên mất tốc độ (FAQ không lên ngay) và đổi lại có một bảo đảm: câu trả lời chưa ai kiểm không bao giờ tới cả lớp.

Tương tự, `goi_y_bai_tap` hạ từ "Mình giúp bạn giải bài" xuống "Mình chỉ ra bước đầu, không xác nhận đáp số"; `chuyen_TA` đổi từ "Mình sẽ báo TA cho bạn" thành "Bạn xem trước và bấm gửi vào hàng chờ TA (ca trực 08:00–22:00)".

## §5. Prototype (chặng 5)

### 5.1 Thông tin chung & phạm vi giả lập

- **File prototype:** [`prototype/index.html`](prototype/index.html) (cùng thư mục với [`prototype/app.js`](prototype/app.js), [`prototype/styles.css`](prototype/styles.css), [`prototype/theme.css`](prototype/theme.css) và [`prototype/README.md`](prototype/README.md)). Mở trực tiếp bằng trình duyệt (Chrome/Edge), không cần cài đặt, npm hay backend.
- **Công cụ xây dựng:** HTML5, CSS3, Vanilla JavaScript (`app.js`), lưu trữ trạng thái phiên demo bằng `localStorage` của trình duyệt (key `mach-lab5-v1`).
- **Có lời gọi AI thật không:** **Không.** Đây là bản thiết kế tương tác (interactive mockup); các câu trả lời và kết quả tra cứu tài liệu được định nghĩa sẵn theo tình huống hoặc bộ lọc từ khóa tại client.
- **Phần nào chạy thật trên giao diện · phần nào giả lập (mock):**
  - **Bấm và tương tác được từ đầu tới cuối:**
    1. Chuyển đổi qua lại giữa các kịch bản bằng chip gợi ý hoặc nhập câu hỏi vào ô chat: **Tài liệu có câu sai** (Ca 1), **Đề xuất FAQ** (Ca 6), **Kiểm tra bài 3** (Ca 5), **Chưa rõ khái niệm** (Ca 3), cùng các ca `Trung vị khác trung bình cộng` (happy path §3.2), `Slide 12` (Ca 2), `Chuyển TA lúc 23:00` (Ca 4), `Ngoại lai 45` (Ca 7), `P-value buổi 7` (Ca 8) và ca lạ bất kỳ.
    2. Đóng/mở hộp trích dẫn nguồn `BUỔI 3 · §3.3` có tô vàng câu cần xem lại và mở modal xem toàn bộ tài liệu `§3.1–§3.5`.
    3. Chỉnh sửa trực tiếp câu hỏi/câu trả lời trong thẻ **Bản nháp đề xuất FAQ**, bấm **Hủy bản nháp** hoặc **Gửi TA duyệt FAQ** qua hộp thoại xác nhận.
    4. Tạo phiếu báo cáo tài liệu/hỏi TA qua hộp thoại **Xem trước khi gửi TA**; chuyển sang tab **Yêu cầu của tôi** để bấm **Hoàn tác / Hủy phiếu** hoặc **Thu hồi đề xuất** khi phiếu đang ở trạng thái `Đang chờ TA`.
    5. Chuyển vai trò sang **Góc TA** (nút chuyển trên thanh topbar): xem hàng chờ, bấm **Kiểm tra / Sửa & duyệt** (bắt buộc tích checkbox _"Tôi đã kiểm tra tính đúng đắn, nguồn và không có đáp số bài đang mở"_ mới bấm được **Duyệt & đăng FAQ**), **Phản hồi học viên**, **Từ chối kèm lý do**, hoặc **Gỡ khỏi FAQ**.
  - **Phần giả lập (mock):**
    - Bối cảnh thời gian cố định tại `23:00 · Thứ Năm, 12/11/2026` (ngoài giờ trực `08:00–22:00`); không hứa TA trả lời đúng 08:00.
    - Trạng thái gửi TA, duyệt, thu hồi và đăng FAQ lưu trong `localStorage` của trình duyệt (nút **Bắt đầu lại demo** ở cuối trang dùng để xóa sạch dữ liệu khi demo lại). Nút chuyển vai trò `Học viên / Góc TA` dùng để trình diễn luồng duyệt 2 chiều trên cùng một màn hình, không phải cơ chế phân quyền máy chủ.

---

### 5.2 Ảnh chụp màn hình có đánh số & ánh xạ thiết kế

- **Ảnh 1:** [`prototype/screen-1-student.jpeg`](prototype/screen-1-student.jpeg) — Màn hình **Trợ lý học tập (Ca 1)**: Tài liệu `§3.3` có câu sai, hiển thị cảnh báo, bằng chứng tô vàng, phản ví dụ và nút chuyển TA.
- **Ảnh 2:** [`prototype/screen-2-autonomy-ta.jpeg`](prototype/screen-2-autonomy-ta.jpeg) — Màn hình **Yêu cầu của tôi (Ca 6)**: Đề xuất FAQ đã gửi vào hàng chờ TA (`0 FAQ công khai`, trạng thái `Đang chờ TA`) và nút hoàn tác `Thu hồi đề xuất`.

| Số trên ảnh     | Vị trí trên giao diện                                                                                                                | Thể hiện điều gì                                                                                                                                                             | Nguyên tắc HAX / PAIR                                                               | Mức tự chủ (§4)                                                               |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| **1** _(Ảnh 1)_ | Đầu khung chat (`Mạch · Trợ lý học tập AI — Dựa trên tài liệu được cấp · Không làm bài thay bạn`) + nhãn `Có nguồn dẫn`              | Cho biết người dùng đang tương tác với AI, chỉ dựa trên tài liệu được cấp và không đưa/xác nhận đáp số bài đang mở (Điều 11 khoản 1 Luật TTNT 134/2025/QH15).                | **G1 & G2** — Làm rõ hệ thống làm được gì và giới hạn năng lực                      | Khung giới hạn chung; `goi_y_dap_so` = **Cấm** (không có nút xin đáp án)      |
| **2** _(Ảnh 1)_ | Hộp cảnh báo vàng `Nguồn có điểm cần xác minh — Đừng vội dùng kết luận này trước khi đối chiếu`                                      | Báo hiệu ngay bằng biểu tượng, chữ và màu vàng rằng tài liệu gốc có điểm mâu thuẫn trước khi học viên đọc kết luận.                                                          | **G2** — Làm rõ độ chắc chắn bị giới hạn do dữ liệu nguồn                           | Chặn việc AI tự khẳng định tài liệu đúng hoặc tự sửa giáo trình               |
| **3** _(Ảnh 1)_ | Hộp trích dẫn `BUỔI 3 · §3.3 Phương sai & độ lệch chuẩn` tô vàng câu sai + hộp phép tính phản ví dụ `√0,25 = 0,5 → 0,5 lớn hơn 0,25` | Hiển thị nguyên văn đoạn trích từ `tra_cuu_tai_lieu`, đánh dấu (`<mark>`) đúng câu cần xem lại và đặt cạnh phản ví dụ toán học để học viên tự đối chiếu.                     | **PAIR — Explainability + Trust** (hiển thị bằng chứng để người dùng tự kiểm chứng) | `tra_cuu_tai_lieu` = **Tự làm** (chỉ đọc, luôn kèm mã mục)                    |
| **4** _(Ảnh 1)_ | Cụm nút `Gửi báo cáo cho TA` / `Tiếp tục học` + dòng `TA ngoài giờ trực · Ca tiếp theo từ 08:00 · Chưa xác định giờ trả lời`         | AI không tự động gọi `chuyen_TA` ngầm; học viên tự quyết định bấm gửi qua hộp thoại xác nhận, và thấy rõ trạng thái TA ngoài giờ trực `08:00–22:00` (không hứa giờ trả lời). | **G10** — Thu hẹp phạm vi khi nghi ngờ, chuyển quyền quyết định cho người dùng      | `chuyen_TA` = **Cần người duyệt** (học viên bấm xác nhận trước khi tạo phiếu) |
| **5** _(Ảnh 2)_ | Ô thống kê `0 FAQ công khai` (và menu trái `FAQ của lớp 0`) bên cạnh `2 Đang chờ`                                                    | Chứng minh khi học viên yêu cầu đăng FAQ (Ca 6), AI chỉ tạo bản nháp/phiếu chờ chứ **không tự đăng** lên FAQ của lớp khi chưa qua TA kiểm duyệt.                             | **G10** — Chặn hành động vượt thẩm quyền có phạm vi ảnh hưởng cả lớp                | `soan_nhap_FAQ` = **Tự làm** (nháp riêng) · `dang_FAQ` = **Cần TA duyệt**     |
| **6** _(Ảnh 2)_ | Thẻ `Đề xuất FAQ #0prpq` với nhãn vàng `Đang chờ TA` và dòng trạng thái chờ kiểm tra trước khi công khai                             | Mọi đề xuất FAQ đều phải dừng ở hàng chờ để TA (ở chế độ `Góc TA`) đọc nguồn `§3.3`, tích xác nhận không lộ đáp số Bài 3 rồi mới bấm duyệt.                                  | **G10 & PAIR Human-in-the-loop** — Người có thẩm quyền kiểm soát quyết định         | `dang_FAQ` = **Cần người duyệt** (TA kiểm tra và bấm duyệt)                   |
| **7** _(Ảnh 2)_ | Nút đỏ `Thu hồi đề xuất` trên thẻ yêu cầu đang chờ                                                                                   | Cho phép học viên chủ động hoàn tác / rút lại đề xuất FAQ hoặc phiếu báo cáo đã gửi khi đang ở trạng thái `Đang chờ TA`.                                                     | **G8 / G9 & PAIR — Errors + Graceful Failure** (luôn có đường lui / hoàn tác)       | Cơ chế đảo ngược (`undo`) cho thao tác đã gửi của học viên                    |

---

### 5.3 Lập luận các quyết định thiết kế trên Prototype (4 ý)

#### Quyết định 1: Cách hiển thị độ chắc chắn và bằng chứng (Ca 1 — Tài liệu `§3.3` có câu sai)

- **Đã cân nhắc các phương án:**
  1. _Phương án A:_ Hiển thị phần trăm độ tự tin (ví dụ: `Độ tin cậy: 42%`) hoặc điểm số ở góc câu trả lời.
  2. _Phương án B:_ Chỉ viết lời giải thích bằng chữ xuôi trong bong bóng chat của AI mà không tách hộp nguồn riêng.
  3. _Phương án C (Đã chọn):_ Kết hợp **nhãn cảnh báo trạng thái cụ thể** (`Nguồn có điểm cần xác minh` dùng cả chữ, biểu tượng và màu vàng) + **hộp trích dẫn nguyên văn `§3.3` tô sáng (`<mark>`) đúng câu cần xem lại** + **hộp phép tính phản ví dụ (`√0,25 = 0,5 → 0,5 lớn hơn 0,25`)**.
- **Chọn phương án nào:** Phương án C.
- **Vì sao chọn:** Học viên học muộn lúc 23:00 cần biết _chính xác câu nào trong tài liệu đang có vấn đề_ và _vì sao nó mâu thuẫn_ để làm tiếp Bài tập 3 mà không bị hoang mang. Đặt câu trích dẫn nguyên văn ở `§3.3` ngay trên hộp phép tính `√0,25 = 0,5` giúp học viên tự kiểm chứng bằng mắt trong vài giây thay vì phải tin mù quáng vào AI.
- **Vì sao loại các phương án kia:**
  - _Loại A (`% độ tin cậy`):_ Không có mô hình đo confidence thực tế; một con số phần trăm vô nghĩa với người học và không chỉ ra lỗi nằm ở suy luận của AI hay nằm ở câu chữ trong giáo trình `§3.3`.
  - _Loại B (chỉ viết chữ xuôi):_ Trộn lẫn lời giải thích của AI với văn bản giáo trình khiến học viên không phân biệt được đâu là nguyên văn tài liệu của giảng viên, đâu là phân tích của AI.

#### Quyết định 2: Cách điều khiển mức tự chủ đối với `dang_FAQ` và `chuyen_TA` (Ca 6 & Ca 4)

- **Đã cân nhắc các phương án:**
  1. _Phương án A:_ Cho AI đăng thẳng lên `FAQ của lớp` nhưng gắn nhãn cảnh báo _"Do AI tạo — Chưa được TA kiểm chứng"_, kèm nút để TA vào gỡ sau.
  2. _Phương án B:_ Cho AI tự động đẩy phiếu sang TA mỗi khi gặp câu hỏi khó và hiện câu chữ _"Mình đã báo TA, TA sẽ phản hồi sau 08:00"_.
  3. _Phương án C (Đã chọn):_ **Tách bước trên giao diện** — ở phía học viên chỉ có thẻ **Bản nháp (`Chưa công khai · Chỉ bạn thấy`)** và hộp thoại **Xem trước khi gửi TA** (kèm nút **Thu hồi / Hủy phiếu** sau khi gửi); còn nút thực thi **Duyệt & đăng FAQ** bị khóa sau checkbox kiểm tra ở màn hình **Góc TA**, đồng thời trạng thái giờ trực ghi rõ _"Ca tiếp theo từ 08:00 · Chưa xác định giờ trả lời"_.
- **Chọn phương án nào:** Phương án C.
- **Vì sao chọn:** Khớp với phân tích cost-of-error ở §4: một câu trả lời sai từ `§3.3` hoặc lộ đáp số Bài tập 3 một khi đã lên FAQ thì cả lớp đã đọc trước khi TA kịp gỡ vào sáng hôm sau. Việc bắt buộc đi qua thẻ nháp + màn hình Góc TA có checkbox chặn triệt để rủi ro phát tán sai lệch, trong khi học viên vẫn có sẵn nội dung nháp để chỉnh sửa ngay lúc 23:00.
- **Vì sao loại các phương án kia:**
  - _Loại A (đăng ngay kèm nhãn cảnh báo):_ Nhãn cảnh báo không thu hồi được kiến thức sai hoặc đáp số đã lộ cho những người đã đọc.
  - _Loại B (tự động gửi TA và hẹn phản hồi sau 08:00):_ Làm tràn hàng chờ của TA bằng các câu hỏi nháp học viên chưa muốn gửi, và cụm từ _"phản hồi sau 08:00"_ dễ làm học viên hiểu lầm là đúng 08:00 sẽ có câu trả lời ngay (vi phạm nguyên tắc không hứa điều hệ thống không kiểm soát được ở Ca 4).

---

### 5.4 Đường đi của Prototype khi gặp "ca lạ" trong lúc Demo

Khi người chấm hoặc nhóm bạn nhập một câu hỏi bất kỳ ngoài các kịch bản có sẵn vào ô chat (`#message`):

1. **Bộ phân loại tình huống (`app.js` dòng 41):** Kiểm tra nội dung theo các nhóm rủi ro cốt lõi (nếu hỏi đáp số/bài 3 → vào luồng khóa đáp số `exercise`; nếu đòi đăng FAQ → vào luồng bản nháp `faq`; nếu hỏi slide/nguồn ngoài → báo chỉ có `§3.1–§3.5`; nếu hỏi bài buổi sau → báo chỉ mở buổi 1–3).
2. **Nếu câu hỏi hoàn toàn nằm ngoài dữ liệu (`scenario = 'unknown'`, `app.js` dòng 30):**
   - AI **không đoán mò và không bịa nguồn**, trả lời rõ giới hạn: _"Mình chưa xác định được yêu cầu này trong các tình huống giả lập. Bạn có thể chọn một ca demo bên dưới hoặc gửi câu hỏi vào hàng chờ TA."_
   - Hiện nút **"Gửi câu hỏi cho TA"** (mức tự chủ: **Cần người duyệt** — học viên bấm mở hộp thoại xác nhận, xem rõ trạng thái TA ngoài giờ trực `08:00–22:00` rồi mới gửi vào hàng chờ).

## §6. Tốt là gì (chặng 6 — nhẹ, bỏ được nếu thiếu giờ)

### 6.1 Các câu hỏi phải tự trả lời

**1. Ba điều gì, nếu AI làm đúng, thì nhóm dám đưa cho người dùng thật?**

| # | Điều kiện phát hành | Pass khi | Cách chấm cố định | Bằng chứng |
| --- | --- | --- | --- | --- |
| 1 | Nguồn có thật | 7 ca nội dung (`source`, `faq`, `exercise`, `ambiguous`, `normal`, `missing`, `outlier`) chỉ nêu mã mục có trong modal "Tài liệu buổi 3"; ca `future` nói rõ chưa có tài liệu buổi 7; ca `time` chỉ nói giờ trực; ca lạ không nhắc nguồn nào. Fail nếu AI bịa nội dung "slide 12" hoặc giảng nội dung buổi 4–10. | Mở modal "Tài liệu buổi 3" để đối chiếu §3.1–§3.5; nhập lần lượt 9 câu trong `questions` (4 câu có chip, 5 câu gõ) rồi 2 câu tự nghĩ; đếm câu trả lời nêu mục không có. | Ảnh 1 điểm 3; `app.js` dòng 8 và 21–30 |
| 2 | Không lộ đáp số bài đang mở | Trong bong bóng trả lời của AI ở `exercise` và `outlier`: không có 15,25, không nhắc lại 11,5, không có "đúng / sai / chính xác" gán cho đáp số; không có nút mời xin đáp số. Số 11,5 do học viên gõ vẫn nằm trong bong bóng của họ, không tính là AI lộ. | Bấm chip "Kiểm tra bài 3"; gõ "trung bình bài 3 là 15,25 đúng không" và "cho em đáp số đi"; đọc bong bóng AI. | `app.js` dòng 23, 28; §4.1 dòng `goi_y_dap_so` = Cấm |
| 3 | Nói đúng giờ và đúng quyền duyệt | Modal "Xem trước khi gửi TA" và modal gửi duyệt FAQ hiện `08:00–22:00`; thẻ "Đang chờ TA" hiện "Ca trực tiếp theo từ 08:00; chưa xác định giờ trả lời". Không có câu hứa TA trả lời ngay hoặc đúng 08:00. Ô "FAQ công khai" chỉ tăng sau khi TA tích checkbox và bấm "Duyệt & đăng FAQ". | Gửi 1 phiếu ở Ca 1, đọc dòng trạng thái; gửi 1 đề xuất FAQ, đọc "FAQ công khai" = 0; sang Góc TA bấm duyệt khi chưa tích (bị chặn), rồi tích, duyệt, đếm lại. | Ảnh 1 điểm 4; Ảnh 2 điểm 5–7; `app.js` dòng 56, 58, 63 |

**2. Một người ngoài nhóm đọc tiêu chí có chấm ra cùng kết quả không?**

Có. Mỗi tiêu chí có cùng một tập đầu vào, cùng một phép đếm và cùng ngưỡng, không phụ thuộc người chấm:
- Cùng 9 câu mẫu trong `questions` + 2 câu tự nghĩ, không đổi giữa các lần.
- Đếm số câu trả lời nêu mục không có trong modal tài liệu; đếm số lần `15,25` hoặc `11,5` xuất hiện trong bong bóng AI; đếm số FAQ công khai trước và sau khi duyệt.
- Ngưỡng: 0 câu sai nguồn, 0 lần lộ đáp số trong câu AI, FAQ chỉ tăng sau thao tác duyệt. Ai bấm đúng các bước cũng ra cùng Pass/Fail.

**3. Thiết kế của nhóm (chặng 3–4 và prototype) đạt bao nhiêu tiêu chí trên 2 kịch bản đắt nhất? Còn lỗi nào chưa sửa được?**

| Tiêu chí | Ca 1: tài liệu §3.3 có câu sai | Ca 6: đăng FAQ chưa kiểm tra |
| --- | --- | --- |
| 1 | Pass. Hộp `BUỔI 3 · §3.3` kèm mã mục; modal tài liệu có đúng §3.3; không nhắc nguồn ngoài. | Pass. Bản nháp nhắc §3.3; phiếu chờ ghi nguồn `Buổi 3 · §3.3`; không nhắc nguồn ngoài. |
| 2 | Pass. Phản ví dụ dùng 0,25; không lấy số từ dãy §3.5 (9, 10, 10, 11, 12, 12, 13, 45); không có nút xin đáp số. | Pass. Bản nháp cũng dùng 0,25; cảnh báo "Không đưa đáp số bài 3 đang mở vào FAQ" hiện trên thẻ nháp và màn hình TA. |
| 3 | Pass. Dòng "TA ngoài giờ trực · Ca tiếp theo từ 08:00 · Chưa xác định giờ trả lời"; AI không tự gửi. | Pass. `0 FAQ công khai`, thẻ "Đang chờ TA"; bấm duyệt khi chưa tích bị chặn kèm thông báo. |

Kết quả: 3/3 tiêu chí đạt ở cả hai ca. Ca 1 và Ca 6 không có đáp số để lộ; phép thử đầy đủ cho tiêu chí 2 ở Ca 5 (học viên đưa 11,5) cũng Pass: AI không nhắc 11,5 và không xác nhận.

| Lỗi còn lại | Vì sao chưa sửa | Đã giảm thế nào |
| --- | --- | --- |
| Học viên ghép nhiều lượt gợi ý bước đầu thành lời giải | Mỗi lượt đều hợp lệ; chặn hết thì mất phần "gợi ý từng bước" của lát cắt | Mỗi lượt một bước; hỏi lại đáp số nhận cùng câu từ chối kèm nút chuyển TA |
| Câu sai trong §3.3 vẫn nằm trong tài liệu | AI không có quyền sửa giáo trình | Nhãn vàng, hộp trích dẫn, phản ví dụ và phiếu báo TA; ai bỏ qua cảnh báo vẫn đọc phải câu sai |
| TA duyệt vội một bản nháp có câu sai | Checkbox chỉ là tự cam kết của TA, không kiểm nội dung thay TA | Đoạn trích §3.3 tô vàng và cảnh báo Bài tập 3 hiện ngay trên màn hình duyệt |
| Prototype là mock: chưa có model thật, chưa dựng ca "Bài tập 2 đã hết hạn", mỗi lượt chỉ hiện một ca | Nhóm chọn bản giả lập để giữ dữ liệu dựng, không cần API key; luật Bài tập 2 ở §4.5 chưa có màn hình tương ứng | Ba tiêu chí chấm trên luồng giả lập; gõ "Bài tập 2" rơi vào ca lạ, mời gửi TA, không lộ đáp số; demo nói rõ đây là mock |

## §7. Demo

- **Ca lạ nhận được ở demo:** _(điền sau buổi demo)_
- **Prototype đã làm gì với ca đó:** _(điền sau buổi demo)_
- **Nhóm có đổi ý gì sau ca đó không:** _(điền sau buổi demo)_
