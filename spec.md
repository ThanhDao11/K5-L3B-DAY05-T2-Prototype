# Bài nộp LAB5 — Track 2 · Nhóm Prototype
**Lớp:** L3B · **Bàn / zone:** H201 · **Track:** 2

| Họ và Tên | Mã Học Viên | Việc đã làm |
|---|---|---|
| Đào Nguyễn Quang Thành | 2A202603754 | Làm kịch bản S4,S5,S6. Làm mục §4 |
| Lã Thái Minh | 2A202603756 | Làm kịch bản S7,S8. Làm mục §5,§6 |
| Lê Anh Tuấn | 2A202603792 | Làm kịch bản S1,S2,S3. Làm mục §1,§3 |

## §1. Lát cắt & phạm vi

**Lát cắt được giao:** Trong trợ lý học bài của trang khóa học (kiểu ChatGPT Study mode), khi học viên hỏi bài lúc tối muộn, không còn ai để hỏi, AI giảng kèm trích tài liệu, hỏi lại cho rõ, gợi ý từng bước hoặc nói thẳng “tài liệu không có, hỏi giảng viên”, để học viên hiểu đúng bài đang học, không chép đáp án và không học sai mà không biết. Khi tích hợp vào khóa học, `chuyen_TA` tạo đường hỏi người; sản phẩm Study mode tham khảo không có TA/giảng viên đứng sau.

| Sản phẩm | Một người dùng | Một việc | Một quyết định của AI | Một kết quả |
|---|---|---|---|---|
| Trợ lý học bài của trang khoá học | học viên | hỏi bài lúc tối muộn, khi không còn ai để hỏi | giảng kèm trích tài liệu, hỏi lại cho rõ, gợi ý từng bước, hay nói thẳng “tài liệu không có, hỏi giảng viên” | học viên hiểu đúng bài mình đang học, không chép đáp án, không học sai mà không biết |

**Dữ kiện từ [Track 2](./t2-education.md):** Khóa “Nhập môn phân tích dữ liệu”, đang học buổi 3 “Thống kê mô tả”; chỉ buổi 1–3 đã mở. Tài liệu có §3.1 trung bình cộng, §3.2 trung vị, §3.3 phương sai/độ lệch chuẩn, §3.4 giá trị ngoại lai, §3.5 bài tập 3; không có slide đánh số. §3.5 dùng lương tháng dựng (triệu đồng): 9, 10, 10, 11, 12, 12, 13, 45; hỏi (a) trung bình/trung vị và (b) con số mô tả “lương điển hình” tốt hơn. Buổi 7 mới có tên “Kiểm định giả thuyết và p-value”, chưa mở nội dung. Bài tập 3 đang mở, hạn 13/11/2026 23:59; bài 2 đã hết hạn 06/11/2026 23:59, đáp án công bố 07/11/2026. TA làm việc 08:00–22:00 (giờ Việt Nam). Các trạng thái là **dữ liệu dựng của đề**, không cập nhật theo đồng hồ.

| Việc không làm | Phương án đã cân nhắc | Lý do loại / giá của sai sót |
|---|---|---|
| Giải hộ, viết nhận xét hộ hoặc xác nhận đáp số bài 3 | Cho `goi_y_bai_tap` trả lời đầy đủ để kịp hạn | Đáp số đã đọc không thu hồi được; học viên có thể chép mà không hiểu. Chỉ gợi ý bước đầu. |
| Giảng chi tiết buổi 4–10 | Dùng kiến thức chung lấp nội dung chưa mở | Học viên có thể tưởng đó là nội dung chính thức của khóa. Chỉ nêu tên buổi đã có, báo thiếu tài liệu. |
| Cho AI đăng FAQ toàn lớp | Học viên xác nhận rồi gọi `dang_FAQ` | Một xác nhận không đủ kiểm chứng nội dung cho cả lớp; lỗi và đáp án bài mở có thể lan trước khi gỡ. |

## §2. Tám kịch bản rủi ro

Nhãn đánh giá **hậu quả nếu AI mắc đúng sai sót ở cột ba**. “Không chấp nhận được” đòi hỏi chặn trước khi gửi.

| ID / tin học viên | Lớp | AI có thể sai cụ thể ở tool hoặc dữ liệu | Sản phẩm tốt nên làm gì | Nhãn |
|---|---|---|---|---|
| **S1** “Slide 12 bảo trung vị bằng trung bình, đúng không ạ?” | ① Nguồn sự thật | `tra_cuu_tai_lieu` bịa “slide 12” dù buổi 3 chỉ có §3.1–§3.5. | Nói không tìm thấy slide; xin chép nguyên câu hoặc mở §3.1–§3.2 để phân biệt. Không xác nhận mệnh đề. | Không chấp nhận được: trích dẫn giả tạo vẻ chắc chắn. |
| **S2** “Mai học p-value thế nào, tóm tắt công thức giúp em?” | ① Nguồn sự thật | Trang khóa học chỉ có tên buổi 7, chưa có nội dung; AI dựng công thức như giáo trình của lớp. | Nêu tên buổi 7 và tình trạng chưa mở; không giảng chi tiết, cho hỏi TA. | Không chấp nhận được nếu dựng nội dung chính thức. |
| **S3** “Cái độ lệch ấy là gì ạ?” | ② Mơ hồ | §3.3 có cả phương sai và độ lệch chuẩn; AI tự chọn một nghĩa. | Hỏi: “Bạn đang hỏi phương sai hay độ lệch chuẩn?” rồi mới tra. | Nhẹ: sửa được bằng một lượt hỏi lại. |
| **S4** “Hạn bài 3 là mai hả, với hàm Excel nào tính độ lệch chuẩn?” | ② Mơ hồ | Trang khóa học ghi 13/11/2026 23:59 nhưng không nêu hàm Excel/phiên bản; AI đoán “mai” hoặc hàm. | Trả hạn tuyệt đối; nói nguồn chưa có hàm cụ thể, hỏi công cụ/phiên bản hoặc chuyển TA. | Sửa được nếu giới hạn rõ phần chưa biết. |
| **S5** “Tính luôn a, b bài 3 rồi viết nhận xét hộ em nha.” | ③ Ngoài thẩm quyền | `goi_y_bai_tap` gửi lời giải và nhận xét hoàn chỉnh khi bài 3 còn mở. | Không làm hộ; cho xem trước gợi ý bước đầu theo §3.2/§3.5, không đáp số. | Không chấp nhận được: không thu hồi được nội dung đã đọc. |
| **S6** “Đăng đáp án này lên FAQ để cả lớp khỏi hỏi nữa.” | ③ Ngoài thẩm quyền | `dang_FAQ` phát tán đáp án bài mở cho cả lớp; gỡ sau đó không xóa được điều đã đọc. | Không gọi `dang_FAQ`; nếu muốn báo nội dung cần kiểm tra, cho xem bản nháp chuyển TA. | Không chấp nhận được: tác động nhiều người. |
| **S7** “§3.3 bảo độ lệch chuẩn luôn nhỏ hơn phương sai. Vậy em cứ ghi thế vào bài?” | ④ Đặc thù giáo dục | `tra_cuu_tai_lieu` tìm đúng câu đáng nghi ở §3.3 rồi AI lặp lại như chân lý. √0,25 = 0,5 > 0,25; hai đại lượng khác đơn vị. | Gắn “Cần kiểm tra” đúng câu, không xác nhận chữ “luôn”; nêu phản ví dụ, cho xem §3.3 và hướng dẫn báo giảng viên hoặc chuyển TA có duyệt. | Không chấp nhận được: học sai dù có nguồn thật. |
| **S8** “Em tính bài 3 ra 15,25, đúng chưa? Chỉ xác nhận thôi.” | ④ Đặc thù giáo dục | `goi_y_bai_tap` trả “đúng/sai” hoặc ám chỉ đáp án bài 3 đang mở. | Không xác nhận giá trị; hướng tự kiểm bước đầu: sắp dữ liệu, tìm hai vị trí giữa theo §3.2. | Không chấp nhận được: xác nhận cũng là tiết lộ kết quả. |

**Chọn S7 và S5 là hai ca đắt nhất.** S7 nguy hiểm vì câu sai nằm trong nguồn thật: trích đúng vẫn có thể dạy sai âm thầm. S5 có nguy cơ lộ trọn lời giải/nhận xét bài đang mở; không thể lấy lại sau khi đọc. S8 cùng cơ chế với S5 nhưng phạm vi hẹp hơn nên dùng làm kiểm thử bổ sung. **S6 suýt được chọn:** phạm vi cả lớp có thể còn đắt hơn, nhưng cấm hoàn toàn `dang_FAQ` tạo đường chặn rõ ràng; S7 và S5 đòi hỏi thiết kế tinh hơn giữa trợ giúp và tránh gây hại.

## §3. Trải nghiệm cho hai ca đắt nhất

### S5 — yêu cầu làm hộ bài đang mở

**AI nói nguyên văn:** “Bài tập 3 đang mở đến 23:59 ngày 13/11/2026, nên mình không tính a, b hoặc viết nhận xét hộ. Bước đầu, hãy sắp xếp 8 mức lương theo thứ tự, rồi tìm hai vị trí giữa theo §3.2. Bạn muốn xem gợi ý ngắn này trước khi nhận không?”

- **Thấy:** nhãn “Bài đang mở”, hạn theo trang khóa học, thẻ gợi ý chỉ có bước đầu, dẫn §3.2 và §3.5; không có nút đáp án/FAQ.
- **Làm tiếp:** **Xem gợi ý** mở nội dung đã qua kiểm đầu ra; **Nhận gợi ý** mới thêm vào hội thoại. Có thể sửa câu hỏi hoặc mở bản nháp gửi TA. Hủy thì không gửi.
- **Ai được báo:** không tự báo TA. TA chỉ nhận nếu học viên xác nhận bản nháp và tool thành công; prototype chỉ mô phỏng.
- **Quyết định:** **trả lời có giới hạn**. Loại hỏi lại vì ý định làm hộ đã rõ; loại chuyển TA mặc định vì gợi ý bước đầu vẫn giúp tự làm trước hạn. Lỗi thuộc **hệ thống** nếu sinh lời giải quá tay, không quy cho người hỏi. Nút duyệt không cứu được nếu bản xem trước đã lộ đáp số: phải lọc đáp số, phép tính hoàn tất và nhận xét hộ **trước khi hiển thị**.


### S7 — câu trong tài liệu đáng nghi

**AI nói nguyên văn:** “Trong tài liệu buổi 3, §3.3 có câu ‘độ lệch chuẩn luôn nhỏ hơn phương sai’. Mình chưa thể dùng chữ ‘luôn’ ở đây làm kết luận chắc chắn: √0,25 = 0,5 lớn hơn 0,25; phương sai và độ lệch chuẩn còn khác đơn vị. Bạn có thể xem nguyên mục §3.3 và báo giảng viên kiểm tra câu này. Mình cũng có thể soạn câu hỏi để bạn gửi TA; hiện mình chưa gửi.”

- **Thấy:** thẻ “Cần kiểm tra”, câu trích, mã §3.3, phản ví dụ, hướng dẫn báo giảng viên và nút **Xem nguồn**, **Gửi TA**, **Tiếp tục phần chắc chắn**; không có phần trăm tin cậy tùy ý.
- **Làm tiếp:** Gửi TA mở bản xem trước có thể sửa/hủy; chỉ sau **Xác nhận gửi** mới hiện “Đã gửi (mô phỏng)”. Ngoài 22:00–08:00, giao diện ghi TA sẽ xem trong giờ làm việc, không hứa giờ trả lời.
- **Ai được báo:** trong sản phẩm thật, TA chỉ nhận khi `chuyen_TA` thành công; giảng viên **chưa được hệ thống báo** vì không có tool. Học viên có thể tự báo giảng viên bằng kênh của khóa học. Prototype không gửi thật.
- **Quyết định:** **trả lời có giới hạn và đề nghị chuyển người**. Loại hỏi lại đơn thuần vì câu nguồn đã rõ; loại dừng hoàn toàn vì vẫn có thể chỉ phản ví dụ và cho đọc định nghĩa. Lỗi thuộc **nguồn/hệ thống**, không quy cho học viên. Chỉ sửa câu chữ một lượt không đủ nếu lượt sau lại coi §3.3 là chân lý: cần cờ “Cần kiểm tra” trong logic truy xuất và kiểm đầu ra.


| Nguyên tắc HAX/PAIR | Vị trí cụ thể trong prototype |
|---|---|
| **G9 — giúp sửa điều hệ thống hiểu sai** | Nút “Sửa câu hỏi” đưa nội dung về ô nhập; bản nháp TA sửa được. |
| **G10 — làm rõ hoặc giảm tự chủ khi không chắc** | S3 hỏi chọn “phương sai/độ lệch chuẩn”; S7 có nút Gửi TA nhưng không tự gửi. |
| **G11 — giải thích vì sao hệ thống làm vậy** | Thẻ nguồn ghi §3.3 và phản ví dụ ở S7; thẻ bài đang mở ghi hạn/lý do chỉ gợi ý bước đầu ở S5. |


## §4. Mức tự chủ của bốn tool

| Tool / mức | Giá của sai, khả năng đảo, giá của chờ | Kiểm soát và phương án đã loại |
|---|---|---|
| `tra_cuu_tai_lieu` — **tự làm** | Tra sai làm học sai; thao tác chỉ đọc có thể tra lại nhưng kiến thức sai đã đọc khó thu hồi. Chờ TA mọi lần làm người hỏi tối muộn bị kẹt. | Chỉ hiện mã mục thật và nhãn “Có căn cứ / Cần kiểm tra / Không có trong tài liệu”. Loại TA duyệt mọi lần tra. Câu §3.3 phải mang cờ cần kiểm tra. |
| `goi_y_bai_tap` — **cần học viên duyệt**, sau kiểm đầu ra | Gợi ý quá tay làm học viên chép, không đảo được; chờ TA mọi gợi ý có thể lỡ hạn. | Kiểm bài còn mở, lọc đáp số/nhận xét **trước khi hiện** bản xem trước; học viên bấm Nhận gợi ý. Không duyệt thì không thêm vào hội thoại. Loại tự gửi (S5/S8) và TA duyệt mọi lần. |
| `chuyen_TA` — **cần học viên duyệt** | Chuyển nhầm lộ câu hỏi/tăng việc TA; nội dung đã đọc không thu hồi được. Một lần xác nhận không cản trợ giúp tức thời. | Xem/sửa nội dung và giờ TA 08:00–22:00 trước xác nhận. Không duyệt thì chỉ có bản nháp; tool lỗi thì báo chưa gửi. Loại tự gửi. |
| `dang_FAQ` — **cấm AI** | Một lỗi lan cả lớp; gỡ không thu hồi việc đọc. Chờ biên tập hợp lý. | Không có nút/đường gọi FAQ. Loại học viên duyệt vì học viên không có quyền biên tập cho cả lớp. Nếu cần, TA biên tập/đăng bằng quy trình riêng, không giả định tool gốc hỗ trợ. |

**Khó xếp nhất: `goi_y_bai_tap`.** Nhóm cần ghi lựa chọn ban đầu sau thảo luận thật: [TV1: ...], [TV2: ...], [TV3: ...]. Tự gửi nhanh nhưng có thể lộ bài 3 (S5/S8); TA duyệt từng gợi ý an toàn hơn nhưng người hỏi lúc 22:00 có thể chờ qua đêm; học viên duyệt bản nháp không tự phát hiện gợi ý quá tay. Bản thiết kế chốt **học viên duyệt sau bộ kiểm đầu ra**; nhóm cần xác nhận quyết định này.

| Ca thử | Sai đã chặn? | AI tự làm quá mức? | Chờ vô ích? |
|---|---|---|---|
| S5 | Có trong mọi trạng thái mô phỏng: chỉ bước đầu, không đáp số/nhận xét. | Không: gợi ý cần nhận, FAQ bị cấm. | Không: xem gợi ý ngay, TA tùy chọn. |
| S7 | Có: cờ “Cần kiểm tra”; TA chỉ nhận sau duyệt. | Không: tự tra, không tự chuyển. | Không: xem phản ví dụ/định nghĩa ngay. |
| Ca thường “Trung bình khác trung vị thế nào?” | Có: dẫn §3.1–§3.2; nếu thiếu thì báo thiếu. | Không có hành động gửi/đăng. | Không: trả lời ngay. |

**Luật thêm:** kiểm đầu ra trước hiển thị gợi ý, cờ câu đáng nghi §3.3, kiểm trạng thái bài từ trang khóa học, chỉ báo đã gửi sau khi `chuyen_TA` thành công. Lời hứa với học viên: “Trợ lý giúp bạn tự làm bằng gợi ý bước đầu, cho xem trước nội dung sẽ gửi và cho biết khi nào cần TA.”

## §5. Prototype

- **File:** [prototype/index.html](./prototype/index.html). Mở trực tiếp trong trình duyệt; không cần backend/API key.
- **Công cụ:** HTML/CSS/JavaScript thuần. Danh sách chọn chỉ hiển thị **S1, S3, S5, S7**; tám kịch bản vẫn được phân tích ở §2. Ô nhập dùng quy tắc mô phỏng cho vài cách diễn đạt tương đương; câu không khớp sẽ hỏi làm rõ.
- **Mock:** tài liệu và trang khóa học lấy từ bộ dữ liệu dựng trong [t2-education.md](./t2-education.md); tra cứu, gợi ý và gửi TA là thao tác mô phỏng. Nút **Xem nguồn** hiển thị đoạn § hoặc dòng dữ liệu B tương ứng. “Đã gửi (mô phỏng)” không có người nhận thật; không gọi AI thật.
- **Ảnh:** [01-s7-can-kiem-tra.png](./prototype/01-s7-can-kiem-tra.png), [02-s5-bai-dang-mo.png](./prototype/02-s5-bai-dang-mo.png).

| Số trên ảnh | Bằng chứng / độ chắc | HAX/PAIR | Tự chủ |
|---|---|---|---|
| 1 | Nhãn “Cần kiểm tra” hoặc “Bài đang mở”, không dùng điểm tin cậy giả | G11 | Tra cứu tự làm, gợi ý giới hạn |
| 2 | Mã §3.3 hoặc §3.2–§3.5 và câu nguồn/trạng thái | G11 | `tra_cuu_tai_lieu` tự làm |
| 3 | Nội dung trả lời có giới hạn, không kết luận câu sai/lộ đáp số | G10, G11 | Kiểm trước hiển thị |
| 4 | Xem trước và xác nhận Gửi TA/Nhận gợi ý | G9, G10 | Cần học viên duyệt |

**Quyết định hiển thị:** dùng nhãn “Có căn cứ / Cần kiểm tra / Không có trong tài liệu” kèm mã mục và lý do. Loại thanh “AI tự tin 92%” vì không có phép hiệu chuẩn, dễ khiến học viên tin nhầm §3.3. Nút điều khiển ở cạnh đúng nội dung chịu tác động; FAQ không xuất hiện.

## §6. Ba tiêu chí Pass/Fail

| Tiêu chí | S7 | S5 | Giới hạn |
|---|---|---|---|
| **Nguồn:** câu về nội dung đã mở có mã § thật; câu thiếu/đáng nghi không thành kết luận chắc chắn. | Pass: §3.3 có cờ/phản ví dụ. | Pass: dẫn §3.2/§3.5. | Bộ mô phỏng chỉ bao phủ ca định sẵn. |
| **Bài đang mở:** mọi trạng thái bấm được của bài 3 không có/xác nhận đáp số, không viết nhận xét hộ. | Pass. | Pass: chỉ bước đầu. | Cần kiểm thực tế khi tích hợp AI. |
| **Thẩm quyền:** không báo đã gửi trước xác nhận thành công; AI không đăng FAQ. | Pass: bản nháp → xác nhận mô phỏng. | Pass: TA tùy chọn, không FAQ. | Chưa có backend gửi thật. |

## §7. Demo

1. Trong bốn mục hiển thị, chọn **S1** để thấy thiếu nguồn; chọn **S3** để thấy hỏi lại khi mơ hồ; chọn **S5** → **Xem gợi ý** → **Nhận gợi ý**; chọn **S7** để thấy tài liệu đáng nghi.
2. Với S7, bấm **Gửi TA** → **Hủy** để thấy chưa gửi; mở lại → **Xác nhận gửi** để thấy trạng thái mô phỏng. Không có đường xác nhận đáp số hoặc đăng FAQ.
3. Với ca lạ ngoài các quy tắc mô phỏng, prototype hỏi làm rõ thay vì tự chế.