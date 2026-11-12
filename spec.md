# Bài nộp LAB5 — T2 Giáo dục · Nhóm DKH

**Lớp:** L3A · **Bàn / zone:** ____ · **Track:** T2 — Giáo dục (trợ lý học bài tối muộn, khi không còn ai để hỏi)

| Họ và Tên | Mã Học Viên | Việc đã làm |
|---|---|---|
|  |  |  |
|  |  |  |
|  |  |  |

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

## §3. Khi AI sai  (chặng 3)

### 3.1 Các câu hỏi phải tự trả lời

#### Ca 1: Tài liệu có câu sai ("Độ lệch chuẩn luôn nhỏ hơn phương sai. Đúng không?")

1. **Lúc AI không chắc, nó nên làm gì và vì sao không chọn hai cách kia?**
   AI chọn trả lời kèm giới hạn: trích nguyên văn câu trong §3.3, chỉ ra phản ví dụ khi phương sai nằm trong khoảng từ 0 đến 1, nói rõ AI không được tự sửa giáo trình và hướng dẫn học viên báo giảng viên.
   - Không chọn hỏi lại một câu (ví dụ "Bạn thử tính với phương sai bằng 0,25 xem sao?") vì học viên hỏi lúc tối muộn thường tin vào tài liệu của trường hơn phép tính của mình; hỏi vòng vo dễ làm họ nghĩ mình hiểu sai.
   - Không chọn dừng hẳn và chỉ chuyển người vì giờ trực của TA là 08:00 đến 22:00. Lúc 23:00 không còn TA trực, nếu AI từ chối giải thích và bắt chờ đến 08:00 sáng mai thì học viên bị kẹt, không làm tiếp được Bài tập 3 (hạn 13/11/2026 23:59).

2. **AI nói câu gì, nguyên văn? Câu đó có hứa điều AI không làm được không?**
   > "Mục §3.3 trong tài liệu Buổi 3 có ghi: 'Vì là căn bậc hai, độ lệch chuẩn luôn nhỏ hơn phương sai.' Câu này trong tài liệu cần xem lại về điều kiện toán học: khi phương sai nằm trong khoảng từ 0 đến 1 (ví dụ phương sai bằng 0,25 thì độ lệch chuẩn là căn bậc hai của 0,25, bằng 0,5), độ lệch chuẩn lớn hơn phương sai. Mình là trợ lý AI nên không có quyền kết luận thay giảng viên hay tự sửa tài liệu. Bạn có thể bấm nút 'Gửi báo cáo mục §3.3 cho TA' bên dưới để TA kiểm tra vào ca trực 08:00 sáng mai nhé."
   
   Câu này không hứa việc AI không làm được: AI nói thẳng mình không sửa được tài liệu, chưa tự gọi `chuyen_TA` khi học viên chưa bấm, và báo trước mốc 08:00 sáng mai theo giờ trực 08:00 đến 22:00 trên trang khoá học.

3. **Người dùng thấy gì ngoài câu chữ?**
   - Nhãn trạng thái màu vàng phía trên câu trả lời: "Độ chắc chắn thấp do tài liệu gốc (§3.3) có điểm cần giảng viên xác nhận".
   - Hộp bằng chứng trích từ `tra_cuu_tai_lieu` hiển thị nguyên văn mục §3.3, trong đó câu "Vì là căn bậc hai, độ lệch chuẩn luôn nhỏ hơn phương sai" được tô nền vàng.
   - Hai nút bấm bên dưới: nút chính "Gửi báo cáo mục §3.3 cho TA (phản hồi sau 08:00)" và nút phụ "Bỏ qua, tiếp tục làm bài với công thức gốc".

4. **Người dùng làm gì tiếp được? Nếu họ không làm gì thì chuyện gì xảy ra?**
   Học viên bấm "Gửi báo cáo mục §3.3 cho TA" để mở thẻ xác nhận gửi phiếu (có ô sửa ghi chú trước khi gửi và nút "Hoàn tác / Huỷ phiếu" sau khi gửi), hoặc bấm "Bỏ qua" để đóng cảnh báo và làm bài tiếp. Nếu học viên đóng trình duyệt mà không bấm gì, cuộc hội thoại được lưu lại trong lịch sử cá nhân và hệ thống không tự gọi `chuyen_TA`.

5. **Ai được báo, sau bao lâu? Người đó thấy gì?**
   Ngay khi học viên bấm xác nhận gửi, `chuyen_TA` đẩy phiếu vào hàng chờ của TA. Vì học viên hỏi lúc 23:00 (ngoài khung 08:00 đến 22:00), TA nhận thông báo vào lúc 08:00 sáng hôm sau. Trên màn hình TA hiện: mã mục §3.3, câu hỏi của học viên, câu trả lời của AI, đoạn trích §3.3 bị đánh dấu và nút "Xác nhận đính chính / Phản hồi học viên".

6. **Lỗi này là lỗi hệ thống, lỗi người dùng, hay lỗi ngữ cảnh? Cách xin lỗi và cách sửa đổi thế nào?**
   Đây là lỗi ngữ cảnh (context error) đi kèm lỗi dữ liệu nguồn: `tra_cuu_tai_lieu` hoạt động đúng thiết kế là trích đúng mục §3.3, nhưng câu chữ trong §3.3 thiếu điều kiện phương sai lớn hơn 1 nên nếu AI trả lời rập khuôn theo tài liệu sẽ làm học viên hiểu sai. Câu trả lời của AI tách rõ đoạn trích nguyên văn trong §3.3 và phép tính căn bậc hai với số 0,25 để học viên nắm đúng bản chất thay vì nhận lỗi tra cứu nhầm chung chung, đồng thời mở luồng báo cáo để giảng viên sửa lại mục §3.3.

7. **Có lỗi nào mà sửa câu chữ không cứu được, chỉ thiết kế mới cứu được?**
   Nếu AI tự gọi `chuyen_TA` ngầm rồi nói "Mình đã báo TA cho bạn" hoặc hứa hẹn giờ trả lời không bám vào dữ liệu `Giờ TA: 08:00-22:00`, học viên sẽ thức chờ phản hồi trong đêm. Sửa câu chữ trong prompt không ngăn được model đôi lúc hứa quá lời; phải sửa bằng thiết kế giao diện: khoá việc tự gọi `chuyen_TA` (bắt buộc qua thẻ xác nhận của học viên) và lấy thẳng trường `Giờ TA: 08:00-22:00` từ trang khoá học gắn cứng lên nút bấm ("TA ngoại tuyến, phản hồi sau 08:00 sáng mai").

#### Ca 6: Đăng FAQ chưa kiểm tra ("Đăng câu trả lời này lên FAQ cho cả lớp đi.")

1. **Lúc AI không chắc, nó nên làm gì và vì sao không chọn hai cách kia?**
   AI chọn dừng việc đăng trực tiếp và chuyển sang luồng chờ người duyệt: chỉ tạo bản nháp câu hỏi kèm câu trả lời, rồi đề xuất gửi cho TA duyệt trước khi đăng lên FAQ chung.
   - Không chọn trả lời kèm giới hạn rồi vẫn cho đăng (ví dụ đăng ngay lên FAQ kèm nhãn "Do AI tạo, chưa kiểm chứng") vì bảng FAQ là nơi cả lớp đọc nhanh trước giờ nộp bài; một câu trả lời dính lỗi từ §3.3 hoặc lộ gợi ý Bài tập 3 một khi đã hiện lên thì nhiều học viên đã đọc trước khi TA kịp gỡ.
   - Không chọn hỏi lại một câu ("Bạn có chắc chắn muốn đăng lên cho cả lớp không?") vì học viên là người đi hỏi bài, không có thẩm quyền và chuyên môn để duyệt kiến thức cho cả khoá học.

2. **AI nói câu gì, nguyên văn? Câu đó có hứa điều AI không làm được không?**
   > "Mình không có quyền đăng thẳng câu trả lời lên FAQ cả lớp. Mọi mục trên FAQ chung cần TA hoặc giảng viên kiểm tra trước để tránh lan truyền thông tin chưa chuẩn hoặc làm lộ gợi ý của Bài tập 3 đang mở (hạn 13/11/2026 23:59). Mình đã soạn sẵn bản nháp cho câu hỏi này; bạn bấm 'Gửi TA duyệt đăng FAQ' bên dưới để TA xem xét vào ca trực 08:00 sáng mai nhé."
   
   Câu nói không hứa quá quyền: nói rõ AI không tự đăng được, chỉ tạo bản nháp và hẹn đúng ca trực 08:00 sáng mai của TA.

3. **Người dùng thấy gì ngoài câu chữ?**
   - Thẻ "Bản nháp đề xuất FAQ" hiển thị câu hỏi, câu trả lời dự kiến và mã mục tài liệu liên quan (§3.1 đến §3.5).
   - Nhãn trạng thái màu xám gắn trên thẻ: "Chưa công khai (Chỉ mình bạn thấy)".
   - Hai nút bấm: "Gửi TA duyệt đăng FAQ (ca trực 08:00-22:00)" và "Huỷ bản nháp". Giao diện của học viên hoàn toàn không có nút gọi thẳng `dang_FAQ`.

4. **Người dùng làm gì tiếp được? Nếu họ không làm gì thì chuyện gì xảy ra?**
   Học viên có thể sửa lại câu hỏi trong bản nháp, bấm "Gửi TA duyệt đăng FAQ" (sau khi bấm gửi sẽ có nút "Hoàn tác / Thu hồi đề xuất" nếu đổi ý), hoặc bấm "Huỷ bản nháp". Nếu học viên không bấm gì, bản nháp chỉ nằm trong khung chat riêng của học viên đó, bảng FAQ của lớp không thay đổi.

5. **Ai được báo, sau bao lâu? Người đó thấy gì?**
   Khi học viên bấm gửi duyệt, đề xuất vào hàng chờ của TA ngay lập tức và báo cho TA lúc 08:00 sáng hôm sau (nếu gửi sau 22:00). TA nhìn thấy bản nháp gồm câu hỏi, câu trả lời của AI, mã mục tài liệu trích dẫn, cảnh báo nếu nội dung chạm vào Bài tập 3 đang mở, cùng hai nút "Duyệt và gọi `dang_FAQ`" hoặc "Sửa / Từ chối".

6. **Lỗi này là lỗi hệ thống, lỗi người dùng, hay lỗi ngữ cảnh? Cách xin lỗi và cách sửa đổi thế nào?**
   Đây là lỗi người dùng yêu cầu vượt thẩm quyền kết hợp với lỗi ngữ cảnh về phạm vi phát tán: cùng một câu trả lời của AI, gửi cho 1 học viên trong khung chat riêng có rủi ro thấp hơn nhiều so với đăng lên FAQ cho cả lớp đọc. AI giải thích rõ quy tắc kiểm duyệt FAQ của khoá học thay vì nhận lỗi hệ thống, rồi chuyển thao tác thành bước gửi bản nháp cho TA.

7. **Có lỗi nào mà sửa câu chữ không cứu được, chỉ thiết kế mới cứu được?**
   Lỗi AI tự động gọi tool `dang_FAQ` khi học viên thúc giục ("Cứ đăng lên đi, mình chịu trách nhiệm") hoặc AI nói dối là "Mình đã đăng lên FAQ cho cả lớp rồi" trong khi chưa đăng. Sửa câu chữ không chặn triệt để được việc model gọi nhầm tool; thiết kế phải tách tool `dang_FAQ` ra khỏi danh sách quyền của AI ở phía học viên, chỉ giữ quyền tạo bản nháp, còn nút thực thi `dang_FAQ` chỉ nằm trên màn hình quản trị của TA.

### 3.2 Bốn đường đi của trải nghiệm

1. **Happy path (Đủ căn cứ, trong phạm vi):** Học viên hỏi "Trung vị khác trung bình cộng chỗ nào ạ?". AI gọi `tra_cuu_tai_lieu`, giải thích sự khác nhau kèm trích dẫn rõ mục §3.1 và §3.2, sau đó hỏi ngược một câu ngắn để học viên tự liên hệ mà không đưa đáp số Bài tập 3.
2. **Low-confidence (② Mơ hồ / thiếu thông tin):** Học viên hỏi "Cái độ lệch ấy là gì? Em đọc không hiểu" (Ca 3). AI nhận diện từ "độ lệch" có thể chỉ "độ lệch chuẩn" ở §3.3 hoặc "dữ liệu lệch" ở §3.2, nên hiện hai nút gợi ý ("Tìm hiểu Độ lệch chuẩn ở §3.3" và "Tìm hiểu Dữ liệu lệch ở §3.2") để học viên chọn đúng ý trước khi giảng chi tiết.
3. **Failure / không căn cứ hoặc nguồn mâu thuẫn (① & ③):** Học viên hỏi "Slide 12 giải thích trung vị thế nào?" (Ca 2). AI báo rõ tài liệu Buổi 3 không có slide đánh số, chỉ có các mục §3.1 đến §3.5 và gợi ý mở §3.2. Khi gặp câu cần xem lại trong §3.3 (Ca 1) hoặc yêu cầu đăng thẳng lên FAQ (Ca 6), AI chặn hành động vượt quyền, hiện bằng chứng gốc và mở nút chuyển TA xử lý.
4. **Correction (Người dùng sửa AI):** Học viên phản hồi "Ý em không phải độ lệch chuẩn ở §3.3 đâu, em hỏi chỗ dữ liệu lương bị lệch về một phía cơ" hoặc bấm sửa lại nội dung trong thẻ "Bản nháp đề xuất FAQ" trước khi gửi TA. AI bỏ ngữ cảnh §3.3, chuyển sang trích mục §3.2 về dữ liệu lệch (thu nhập, giá nhà) và cập nhật lại hộp trích dẫn tương ứng.

### 3.3 Nguyên tắc HAX/PAIR

- **G2** → câu AI nói và nhãn trên màn hình ở Ca 1: hiển thị nhãn cố định "Trợ lý học tập AI (chỉ dựa trên tài liệu Buổi 1-3)" trên đầu khung chat (theo Điều 11 khoản 1 Luật Trí tuệ nhân tạo 134/2025/QH15) và nhãn vàng "Độ chắc chắn thấp do tài liệu gốc (§3.3) có điểm cần giảng viên xác nhận", kèm câu nói rõ AI không có quyền tự sửa giáo trình hay kết luận thay giảng viên.
- **G10** → câu AI nói và nút hành động ở Ca 1 và Ca 6: ở Ca 1, khi phát hiện câu trong §3.3 mâu thuẫn với trường hợp phương sai bằng 0,25, AI thu hẹp phạm vi về công thức gốc và đề xuất gửi phiếu cho TA thay vì khẳng định tài liệu đúng hay tự sửa tài liệu; ở Ca 6, AI thu hẹp yêu cầu "đăng FAQ cả lớp" thành "soạn bản nháp chờ TA duyệt".
- **PAIR Explainability + Trust** → hộp trích dẫn bên cạnh câu trả lời ở Ca 1 và thẻ xem trước ở Ca 6: hiển thị nguyên văn đoạn trích mục §3.3 từ `tra_cuu_tai_lieu` (tô sáng câu cần xem lại) để học viên tự đối chiếu với phép tính căn bậc hai, và hiển thị thẻ "Bản nháp đề xuất FAQ" kèm nhãn "Chưa công khai (Chỉ mình bạn thấy)" cùng mốc giờ trực `08:00-22:00` trước khi học viên bấm gửi.

## §4. Mức tự chủ  (chặng 4)

### 4.1 Bảng mức tự chủ của nhóm

Thang mức: **tự làm** / **cần người duyệt** / **cấm**. Hai tool được tách bước (lý do ở 4.5) nên bảng có 6 dòng thay vì 4. Trang khoá học (hạn nộp, giờ TA, đề cương) được nạp làm ngữ cảnh chỉ đọc cho AI, nhóm không tính là một tool riêng.

| Tool | Mức | Ai duyệt | Đảo lại thế nào |
|---|---|---|---|
| `tra_cuu_tai_lieu` | **Tự làm** | — | Chỉ đọc, không có gì để đảo |
| `goi_y_buoc_dau` *(tách từ `goi_y_bai_tap`)* | **Tự làm, khoá nội dung** | — | Không đảo được, nên chặn từ trước bằng khoá nội dung (xem 4.2) |
| `goi_y_dap_so` *(phần còn lại của `goi_y_bai_tap`: đưa hoặc xác nhận đáp số bài đang mở, viết nhận xét hộ)* | **Cấm** | — | Không có nút, AI không được cấp quyền |
| `chuyen_TA` | **Cần người duyệt** | Học viên bấm xác nhận trên thẻ | Có nút "Hoàn tác / Huỷ phiếu" sau khi gửi |
| `soan_nhap_FAQ` *(tách từ `dang_FAQ`)* | **Tự làm** | — | Nút "Huỷ bản nháp", chưa ai khác thấy |
| `dang_FAQ` | **Cần người duyệt** | TA (hoặc giảng viên) bấm "Duyệt và gọi `dang_FAQ`" trên màn hình quản trị | Gỡ được, nhưng người đã đọc thì không thu hồi được, nên chặn từ trước bằng bước duyệt |

### 4.2 Lý do từng tool theo cost-of-error

#### `tra_cuu_tai_lieu` → tự làm

- **Sai thì ai chịu gì:** tra nhầm mục hoặc trả đoạn lạc đề thì học viên đọc một đoạn không liên quan; không có gì bị ghi, bị gửi hay bị công khai. Hộp bằng chứng luôn hiện mã mục và nguyên văn (nguyên tắc PAIR Explainability ở §3) nên học viên tự thấy đoạn lạc đề.
- **Đảo lại được không:** không có gì để đảo, bảng tool ghi "Chỉ đọc".
- **Chờ người thì mất gì:** mất cả lát cắt. TA chỉ trực 08:00–22:00, học viên hỏi từ 22:00 trở đi không có ai duyệt, đúng nỗi đau trong lời học viên: "kẹt một chữ trong tài liệu là coi như bỏ".
- **Phương án đã loại:** *cần người duyệt* vì duyệt một thao tác chỉ đọc không chặn được rủi ro nào mà làm chậm mọi câu hỏi; *cấm* vì mất căn cứ trong khi giảng viên muốn trợ lý "nói rõ tài liệu buổi mấy, mục nào".
- **Giới hạn đi kèm:** chỉ tìm trong tài liệu các buổi đã mở (buổi 1–3), lọc ngay ở tool. Hỏi buổi 7 (Ca 8) thì tool trả "không có" và AI chỉ được nói tên buổi từ đề cương trên trang khoá học.

#### `goi_y_buoc_dau` → tự làm, khoá nội dung

- **Sai thì ai chịu gì:** gợi ý quá tay thì học viên chép sớm, mất cơ hội tự nghĩ, đúng thứ lát cắt muốn tránh; giảng viên không biết ai đã chép. Sai kiểu âm thầm, không ai báo.
- **Đảo lại được không:** không, bảng tool ghi "Gợi ý quá tay thì học viên đã chép". Vì không đảo được nên nhóm không dựa vào "sửa sau" mà khoá nội dung từ trước: mỗi gợi ý chỉ gồm *mã mục tài liệu liên quan + một câu hỏi dẫn* (ví dụ: "Bạn đã sắp xếp các giá trị tăng dần chưa? Với số giá trị chẵn, §3.2 nói trung vị lấy từ đâu?"). Bộ kiểm đầu ra chặn mọi con số kết quả tính từ dãy số ở §3.5 và mọi chữ "đúng / sai / chính xác" gán cho đáp số của học viên, rồi thay bằng câu mẫu an toàn. Luật này nằm ở tầng hiển thị, không nằm trong lời nhắc cho model, vì sửa câu chữ không chặn triệt để được (xem Ca 1 mục 7 ở §3). Nếu vẫn lọt, cái lộ ra nhiều nhất là một bước phương pháp đã có sẵn trong §3.1–§3.2, không phải đáp số.
- **Chờ người thì mất gì:** học viên hỏi lúc 23:00 phải chờ tới 08:00 sáng mai, trong khi Bài tập 3 hết hạn 13/11/2026 23:59 (Ca 4).
- **Phương án đã loại:** *tự làm không khoá nội dung* (Ca 5, Ca 7); *cần TA duyệt* (chờ vô ích); *học viên bấm xác nhận trước khi nhận gợi ý* vì người bấm chính là người muốn đáp số, một cú bấm chặn ý định chứ không chặn được nội dung quá tay; *cấm* (xem 4.3).

#### `goi_y_dap_so` → cấm

- **Sai thì ai chịu gì:** học viên chép đáp số hoặc được xác nhận đáp số rồi nộp, học sai mà không biết. Chấm bài và nhận xét bài làm là việc của giảng viên, không thuộc thẩm quyền của AI.
- **Đảo lại được không:** không, đáp số đã tới học viên thì không lấy lại được.
- **Chờ người thì mất gì:** không áp dụng. Cho TA duyệt cũng không giải quyết được: đáp số vẫn tới học viên trước hạn, trái mục tiêu "không chép đáp án" của lát cắt.
- **Phương án đã loại:** *cần TA duyệt* (TA ngoại tuyến sau 22:00, và dù duyệt thì đáp số vẫn lộ); *cần học viên xác nhận* vì người bấm chính là người muốn đáp số nên bước xác nhận không chặn được gì.
- **Trên màn hình:** không có nút hay câu gợi ý kiểu "Cho em đáp án" hoặc "Em làm đúng chưa?". Bài đã hết hạn và đã có đáp án công bố (Bài tập 2) không thuộc diện cấm (luật 3 ở 4.5).

#### `chuyen_TA` → cần người duyệt (học viên bấm xác nhận)

- **Ai duyệt · thấy gì:** học viên. Thẻ xác nhận hiện câu hỏi, ô ghi chú sửa được, mã mục và đoạn trích liên quan, và dòng trạng thái lấy thẳng từ trường Giờ TA ("TA ngoại tuyến, phản hồi sau 08:00 sáng mai" nếu ngoài 08:00–22:00).
- **Quá hạn thì sao:** học viên không bấm thì không có phiếu nào được tạo, thẻ vẫn nằm trong khung chat, cuộc hội thoại lưu lịch sử; AI không tự gửi và không nói "đã báo TA". Phiếu đã gửi nằm trong hàng chờ cho tới khi TA xử lý; học viên thấy trạng thái "Đang chờ TA" chứ không phải một giờ trả lời được hứa.
- **Sai thì ai chịu gì:** gửi thừa thì TA mất công đọc phiếu không cần thiết và hàng chờ của người duy nhất có thể "chuyển" bị loãng; gửi khi học viên chưa đồng ý thì nội dung bài làm dở bị TA thấy ngoài ý học viên; nặng nhất là học viên nghe "đã báo TA" rồi ngừng tìm cách khác, thức chờ qua đêm (Ca 4).
- **Đảo lại được không:** được (huỷ phiếu), nhưng TA có thể đã đọc.
- **Chờ người thì mất gì:** một cú bấm của chính học viên, vài giây. Bước xác nhận rất rẻ nên chặn được rủi ro mà không làm chậm.
- **Phương án đã loại:** *tự làm* (AI tự chuyển mỗi khi không chắc) vì hàng chờ TA sẽ tràn khi cả lớp cùng hỏi tối muộn, và AI dễ nói "đã báo TA" khi chưa có xác nhận; *cấm* vì bỏ mất đường lui duy nhất khi tài liệu có câu sai (Ca 1), trong khi sản phẩm thật hôm nay không có ai để chuyển.
- **Người nhận:** TA là người nhận duy nhất AI chạm tới, bảng tool không có tool nào gửi thẳng giảng viên; TA xác nhận lỗi tài liệu rồi tự chuyển giảng viên sửa, ngoài hệ thống trợ lý.

#### `soan_nhap_FAQ` → tự làm

- **Sai thì ai chịu gì:** bản nháp sai chỉ nằm trong khung chat riêng, nhãn "Chưa công khai (Chỉ mình bạn thấy)"; người nhìn thấy và chịu là chính học viên đó.
- **Đảo lại được không:** được, nút "Huỷ bản nháp", chưa ai khác đọc.
- **Chờ người thì mất gì:** nếu bắt duyệt thì TA phải duyệt cả những bản nháp chưa ai gửi, tăng việc cho người ít thời gian nhất.
- **Phương án đã loại:** *cần người duyệt* vì bản nháp chưa tác động tới ai; *cấm* vì mất đường cho học viên có sẵn bản soạn để TA xem, TA phải viết lại từ đầu.

#### `dang_FAQ` → cần người duyệt (TA)

- **Ai duyệt · thấy gì:** TA (hoặc giảng viên) trên màn hình quản trị: câu hỏi, câu trả lời của AI, mã mục tài liệu trích dẫn, đoạn trích có đánh dấu câu cần xem lại (nếu có), cảnh báo nếu nội dung chạm Bài tập 3 đang mở, và hai nút "Duyệt và gọi `dang_FAQ`" / "Sửa / Từ chối".
- **Quá hạn thì sao:** không ai duyệt thì không đăng. Gửi sau 22:00 thì TA thấy phiếu từ 08:00 sáng hôm sau. Mặc định an toàn là FAQ giữ nguyên; bản nháp hiện "Đang chờ TA duyệt" và không bao giờ tự đăng khi hết chờ. Học viên không bị kẹt vì câu trả lời riêng của họ vẫn nằm trong khung chat.
- **Sai thì ai chịu gì:** cả lớp, không chỉ người hỏi, đọc một câu sai hoặc lộ gợi ý Bài tập 3 trước giờ nộp. Đây là kiểu sai âm thầm nhân lên theo số người đọc.
- **Đảo lại được không:** gỡ bài được, nhưng bảng tool ghi "nhiều người đã đọc": thu hồi cái đã đọc thì không.
- **Chờ người thì mất gì:** FAQ chậm vài giờ; một số học viên khác chưa thấy câu trả lời nhưng vẫn hỏi riêng được trợ lý. Rẻ hơn nhiều so với một câu sai tới cả lớp.
- **Phương án đã loại:** *tự làm kèm nhãn "do AI tạo, chưa kiểm chứng"* vì nhãn không rút lại được cái đã đọc và người đọc FAQ trước giờ nộp thường lướt qua (Ca 6 mục 1 ở §3); *học viên tự duyệt* vì học viên không có thẩm quyền duyệt kiến thức cho cả khoá; *cấm* vì FAQ có giá trị thật, câu hỏi kiểu Ca 3 sẽ bị hỏi lại nhiều lần.

### 4.3 Tool khó xếp nhất: `goi_y_bai_tap`

Mức nào cũng có giá. Ba cách xếp ban đầu, mỗi người xếp riêng trước khi bàn:

| Cách xếp | Ai chọn | Cái giá | Kịch bản ở §2 cho thấy giá |
|---|---|---|---|
| **A.** Tự làm, không giới hạn nội dung | *(điền tên)* | AI xác nhận đáp số hoặc nhận xét hộ, học viên chép; không lấy lại được, âm thầm | Ca 5 ("ra 11,5, đúng không ạ?"); Ca 7 (khuyên bỏ số 45 là quyết định thay học viên) |
| **B.** Cần TA duyệt từng gợi ý | *(điền tên)* | Học viên chờ vô ích: TA chỉ trực 08:00–22:00, hỏi 23:00 thì đợi tới 08:00 sáng mai, trong khi Bài tập 3 hết hạn 13/11 23:59 | Ca 4 (23:00); lời học viên "sáng mai hỏi thì đã quá hạn" |
| **C.** Cấm mọi gợi ý bài đang mở | *(điền tên)* | Bỏ đúng thứ lát cắt hứa ("gợi ý từng bước"); học viên không có gì để làm tiếp và quay sang chép nguồn khác | Ca 5 và Ca 7: cách xử lý đúng ở §2 ("gợi ý kiểm tra thứ tự và hai vị trí giữa", "xem đó là lỗi nhập liệu hay dữ liệu thật") bản thân đã là gợi ý bước đầu; cấm hết thì cả hai ca mất cách xử lý tốt |

**Nhóm chốt D: tách đôi.** `goi_y_buoc_dau` tự làm có khoá nội dung, `goi_y_dap_so` cấm. Lý do: cái hại nằm ở *nội dung* của gợi ý (đáp số, xác nhận), không nằm ở *việc gợi ý*. Tách ra thì giữ được phần giá trị (bước đầu, không phải chờ ai) và cấm đúng phần gây hại. Cách chốt này trùng cột "Nên làm" của Ca 5 và Ca 7 ở §2.

**Giá còn lại của D:** học viên hỏi dồn nhiều lượt "bước đầu" để ghép thành lời giải. Nhóm chưa chặn triệt để việc này: mỗi lượt chỉ một bước đầu, xin đáp số lần hai thì nhận cùng giới hạn kèm nút `chuyen_TA` (học viên tự bấm). Phần ghép gợi ý được ghi vào lỗi còn lại ở §6.

### 4.4 Thử mức đã đặt trên ba kịch bản

Ba câu hỏi cho mỗi kịch bản: (1) cái sai có bị chặn không; (2) còn việc nào AI làm khi lẽ ra phải hỏi; (3) người dùng bình thường có phải chờ vô ích không. Hai kịch bản đắt nhất là Ca 1 và Ca 6 (§2); kịch bản bình thường là Ca 3 (nhãn "Nhẹ").

**Ca 1: Tài liệu có câu sai**

1. **Chặn một nửa.** Hành động sai bị chặn: AI không có tool sửa tài liệu và không tự gọi `chuyen_TA` (cần học viên bấm), nên không thể nói "đã báo TA" khi chưa gửi. Nhưng *lời nói* sai ("tài liệu đúng") thì mức tự chủ không chặn được: `tra_cuu_tai_lieu` tự làm vẫn trả nguyên văn câu sai ở §3.3. Phần này do nhãn vàng, hộp bằng chứng và luật "không khẳng định tài liệu đúng khi chưa kiểm" gánh (§3); được kiểm lại ở §6.
2. **Không còn việc nào làm khi lẽ ra phải hỏi:** việc duy nhất tự chạy là tra cứu chỉ đọc.
3. **Không chờ vô ích:** học viên nhận câu trả lời kèm phản ví dụ ngay lúc 23:00; chỉ chờ TA nếu tự chọn gửi phiếu, và được nói trước "phản hồi sau 08:00".

**Ca 6: Đăng FAQ chưa kiểm tra**

1. **Chặn.** Học viên không có nút `dang_FAQ`, AI chỉ có `soan_nhap_FAQ`. Học viên thúc giục ("cứ đăng đi, mình chịu trách nhiệm") cũng không đổi được mức, vì quyền nằm ở tầng tool chứ không ở lời nói.
2. **Còn một việc tự làm là soạn nháp.** Chấp nhận được vì nháp chỉ mình học viên thấy; nháp chạm Bài tập 3 mang cảnh báo cho TA. Rủi ro còn lại: TA duyệt vội và đăng câu sai. Nhóm giảm bằng đoạn trích và cảnh báo trên màn hình TA, không loại bỏ hoàn toàn được.
3. **Không chờ vô ích:** người hỏi bình thường không bị ảnh hưởng vì không đòi đăng FAQ. Người đòi đăng thì chờ TA, nhưng không mất gì gấp vì họ vẫn nhận câu trả lời riêng ngay trong chat.

**Ca 3: "Cái độ lệch ấy là gì? Em đọc không hiểu." (bình thường)**

1. **Không có hành động rủi ro để chặn:** chỉ có `tra_cuu_tai_lieu`, chỉ đọc.
2. **Không làm khi lẽ ra phải hỏi:** AI hiện hai nút ("Độ lệch chuẩn ở §3.3" / "Dữ liệu lệch ở §3.2") trước khi giảng (đường low-confidence ở phần 3.2); tra cứu chỉ để tìm hai ứng viên.
3. **Không chờ vô ích:** một lần bấm chọn, không cần người nào duyệt.

**Kết luận thử:** mức tự chủ chặn tốt các *hành động* (đăng, chuyển, đưa đáp số), nhưng chưa chặn được lỗi *nội dung nguồn* ở Ca 1. Điểm này ghi vào lỗi còn lại ở §6.

### 4.5 Luật thêm và tool tách bước

1. **Tách `dang_FAQ`** thành `soan_nhap_FAQ` (tự làm) và `dang_FAQ` (TA duyệt). Nhờ đó Ca 6 bị chặn mà học viên vẫn có bản soạn sẵn nên không phải chờ vô ích.
2. **Tách `goi_y_bai_tap`** thành `goi_y_buoc_dau` (tự làm, khoá nội dung) và `goi_y_dap_so` (cấm). Nhờ đó Ca 5 (xác nhận 11,5) và Ca 7 (khuyên bỏ số 45) bị chặn mà người hỏi vẫn nhận được bước đầu hữu ích.
3. **Luật trạng thái bài, lấy từ trang khoá học:** bài "đang mở" (Bài tập 3, hạn 13/11/2026 23:59) thì chỉ bước đầu; bài "đã hết hạn và đã có đáp án công bố" (Bài tập 2, hạn 06/11, đáp án 07/11) thì được giải thích đầy đủ. Trạng thái lấy từ trang khoá học, không lấy từ lời học viên ("bài đó hết hạn rồi mà"), để học viên không nói sai trạng thái nhằm moi đáp số.
4. **Luật câu xác nhận hành động do hệ thống phát:** các câu "Đã gửi cho TA", "Đã gửi duyệt", "Đã đăng" chỉ hiện từ kết quả tool trả về (kèm giờ), model không tự viết. Luật này chặn kiểu lỗi "AI nói đã làm việc nó chưa làm" (Ca 4: hứa TA trả lời ngay; Ca 6: "mình đã đăng rồi") mà sửa câu chữ không cứu được (Ca 6 mục 7 ở §3).

### 4.6 Mức tự chủ đã đổi lời hứa với người dùng

`dang_FAQ` là ví dụ rõ nhất. Nếu để tự làm, lời hứa với học viên là *"Mình đăng giúp bạn lên FAQ cho cả lớp"*. Ở mức cần TA duyệt, lời hứa thành *"Mình soạn sẵn, TA duyệt rồi mới lên FAQ"*. Lời hứa đổi từ **kết quả** (đã đăng) sang **quy trình** (đã gửi duyệt, đang chờ). Học viên mất tốc độ (FAQ không lên ngay) và đổi lại có một bảo đảm: câu trả lời chưa ai kiểm không bao giờ tới cả lớp.

Tương tự, `goi_y_bai_tap` hạ từ "Mình giúp bạn giải bài" xuống "Mình chỉ ra bước đầu, không xác nhận đáp số"; `chuyen_TA` đổi từ "Mình sẽ báo TA cho bạn" thành "Bạn bấm gửi, TA xem sau 08:00 sáng mai".

## §5. Prototype  (chặng 5)

> *Chưa làm.*

## §6. Tốt là gì  (chặng 6 — nhẹ, bỏ được nếu thiếu giờ)

> *Chưa làm.*

## §7. Demo

> *Chưa làm.*
