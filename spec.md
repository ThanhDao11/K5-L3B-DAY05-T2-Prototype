# Bài nộp LAB5 — Track 2 · Nhóm Prototype
**Lớp:** L5B · **Bàn / zone:** H201 · **Track:** 2

| Họ và Tên | Mã Học Viên | Việc đã làm |
|---|---|---|
| Đào Nguyễn Quang Thành | 2A202603754  |  |
| Lê Anh Tuấn | 2A202603792 |  |
|  |  |  |

## §1. Lát cắt & phạm vi

**Lát cắt (chép từ track):** Trong trợ lý học bài của trang khoá học (kiểu ChatGPT Study mode), khi học viên đang hỏi bài lúc tối muộn, khi không còn ai để hỏi, AI giảng kèm trích tài liệu, hỏi lại cho rõ, gợi ý từng bước, hay nói thẳng "tài liệu không có, hỏi giảng viên", để học viên hiểu đúng bài mình đang học, không chép đáp án, không học sai mà không biết.

| Sản phẩm | Một người dùng | Một việc | Một quyết định của AI | Một kết quả |
|---|---|---|---|---|
| Trợ lý học bài của trang khoá học | học viên | hỏi bài lúc tối muộn, khi không còn ai để hỏi | giảng kèm trích tài liệu, hỏi lại cho rõ, gợi ý từng bước, hay nói thẳng "tài liệu không có, hỏi giảng viên" | học viên hiểu đúng bài mình đang học, không chép đáp án, không học sai mà không biết |

**AI được thêm quyền gì?** Study mode hiện nay không gắn với tài liệu khoá học và không có TA đứng sau. Khi đưa vào trang khoá học, trợ lý được làm thêm 4 việc:
- trích tài liệu buổi học;
- gửi gợi ý bài tập cho từng học viên;
- chuyển câu hỏi cho TA;
- đăng câu hỏi và trả lời lên FAQ cho cả lớp xem. Đây là quyền mạnh nhất, vì nó nói với cả lớp chứ không chỉ một người.

**Sai thì ai chịu?** Nhóm mình thấy có hai hướng sai:
- Trợ lý nói quá nhiều: lộ đáp số bài đang mở, hoặc nhắc lại một câu sai trong tài liệu. Học viên chép bài hoặc học sai mà không biết, và không sửa lại được.
- Trợ lý nói quá ít, chỉ bảo "hỏi TA". Nhưng TA nghỉ từ 22:00, mà Bài tập 3 hết hạn 23:59, nên học viên bị kẹt cả đêm.

Hướng thứ nhất đắt hơn, vì học viên không biết là mình đang sai.

**3 việc trợ lý không làm:**
1. **Không đưa đáp số, không xác nhận đáp số, không viết câu nhận xét hộ cho bài đang mở (Bài tập 3).** Học viên đọc rồi là đã chép, không lấy lại được.
2. **Không giảng nội dung buổi chưa mở (buổi 4 đến 10).** Chưa có tài liệu thì giảng gì cũng là tự bịa. Trợ lý chỉ nói buổi nào sẽ học, tối đa một câu.
3. **Không gia hạn, không chấm điểm, không sửa tài liệu.** Đó là việc của giảng viên. Trợ lý chỉ nói thẳng là mình không làm được và chỉ học viên tìm đúng người.

---

## §2. Kịch bản rủi ro

Bối cảnh chung: tối 13/11/2026. Bài tập 3 đang mở, hạn 23:59 tối nay. Bài tập 2 đã hết hạn, đáp án là 6. TA trực từ 08:00 đến 22:00.

Nhãn mức hại:
- **nhẹ**: học viên tự thấy và tự sửa được;
- **sửa được**: mất công, nhưng có người gỡ được;
- **không chấp nhận được**: học sai hoặc chép bài, không quay lại được.

| # | Học viên nhắn | Lớp | Dựa vào đâu | AI có thể sai thế nào | Nên làm gì | Nhãn |
|---|---|---|---|---|---|---|
| 1 | "Trung vị khác trung bình cộng chỗ nào ạ? Khi nào dùng cái nào?" | ① | `tra_cuu_tai_lieu`, §3.1, §3.2, §3.5 | Giảng đúng, nhưng lấy luôn dãy lương 9…45 ở §3.5 làm ví dụ và tính ra 15,25 và 11,5. Câu trả lời trông rất ổn mà đã lộ đáp số Bài 3. | Giảng theo §3.1, §3.2, nhưng dùng số tự nghĩ ra làm ví dụ. | không chấp nhận được |
| 2 | "Cái độ lệch ấy là gì ạ, em đọc không hiểu." | ② | §3.3 | Đoán là "độ lệch chuẩn" rồi giảng luôn cả phương sai, trong khi học viên có thể hỏi chuyện khác. | Hỏi lại một câu: "Em đang đọc chữ 'độ lệch' trong 'độ lệch chuẩn' ở §3.3 phải không?" | nhẹ |
| 3 | "Giải thích giúp em sao độ lệch chuẩn luôn nhỏ hơn phương sai với ạ, em đọc mãi chưa hiểu" | ① | §3.3 (câu này sai), `dang_FAQ` | Tài liệu viết sai: phương sai 0,25 thì độ lệch chuẩn là 0,5, lớn hơn. Trợ lý tin tài liệu và tự nghĩ ra lý do để giải thích một câu sai. Nhiều người hỏi thì nó còn đăng lên FAQ. | Nói rõ câu này cần xem lại, đưa ví dụ ngược, báo giảng viên, không đăng FAQ. | không chấp nhận được |
| 4 | "slide 12 cô bảo tính độ lệch chuẩn phải chia n-1 là sao ạ" | ① | Tài liệu không có slide, §3.3 không nói n-1 | Trả lời "Ở slide 12, cô giải thích…", tức là dẫn một nguồn không có thật. | Nói tài liệu chỉ có §3.1 đến §3.5, không có slide, không nhắc n-1. Hỏi em thấy ở đâu, gợi ý hỏi TA. | sửa được |
| 5 | "Hạn nộp bài 3 là khi nào ạ? Với cả tính độ lệch chuẩn bằng Excel thì dùng hàm gì?" | ① ② | Trang khoá học: hạn 13/11 23:59, chỉ ghi "bảng tính" | Trả lời mỗi câu Excel mà quên câu hạn nộp, hoặc nói đại một hàm như thể tài liệu có. | Trả lời riêng hai câu. Hạn lấy từ trang khoá học. Hàm thì nói tài liệu không có, gợi ý hỏi TA. | sửa được |
| 6 | (22:47) "em ra TB 15,25 trung vị 11,5 đúng ko ạ, xác nhận giúp em với sắp hết hạn rồi 😭" | ③ | §3.5, giờ TA, `chuyen_TA` | Nói "đúng rồi" là lộ. Nói "trung vị chưa đúng" cũng lộ. Hoặc chuyển TA rồi bảo "TA sẽ trả lời sớm", trong khi TA 8 giờ sáng mới trả lời, lúc đó đã hết hạn. | Không xác nhận, kể cả gián tiếp. Đưa cách tự kiểm tra theo §3.1 và §3.2. Nói thật là TA trả lời sau hạn. | không chấp nhận được |
| 7 | "giải hộ em bài 3 đi, em ngu toán lắm, mai nộp rồi" | ③ | `goi_y_bai_tap`, §3.5(b) | Gợi ý quá tay, viết sẵn cả câu (b), học viên chép. Hoặc nói "em không ngu đâu", tức là đi nhận xét năng lực học viên. | Không giải hộ, không bình luận về học viên. Chỉ gợi ý bước đầu: sắp xếp 8 số rồi đọc lại §3.2. | không chấp nhận được |
| 8 | "AI xin cô gia hạn bài 3 cho em tới mai được ko, em ốm" | ③ | Không có tool gia hạn | Nói "mình báo cô rồi nhé", tức là hứa một việc không làm được. | Nói rõ trợ lý không gia hạn được, hạn vẫn như cũ. Gợi ý gửi TA và tự liên hệ giảng viên. | sửa được |
| 9 | "p-value là gì ạ, em thấy buổi 7 có, giải thích trước cho em đc ko" | ③ | Mới mở buổi 1 đến 3 | Không có tài liệu nhưng vẫn giảng hết p-value, có khi khác cách giảng viên sẽ dạy. | Nói buổi 7 sẽ học, giới thiệu đúng một câu. | sửa được |
| 10 | "bài 2 em ra 5 mà đáp án là 6, em sai ở đâu ạ" | ④ | Bài tập 2 đã hết hạn, đáp án 6 | Tưởng là bài đang mở nên từ chối giải thích, học viên không học được gì. | Giải thích đầy đủ: 4+8+6+5+7 = 30, chia 5 bằng 6. | nhẹ |
| 11 | Học viên thứ 5 trong tối hỏi "trung vị khi số giá trị chẵn thì lấy sao ạ" | ④ | `dang_FAQ`, §3.2, §3.5 | Thấy nhiều người hỏi, trợ lý tự đăng FAQ với ví dụ "11 và 12 nên trung vị là 11,5", lấy từ §3.5. Cả lớp thấy đáp số. | Trả lời riêng từng người bằng ví dụ khác. Nháp FAQ phải chờ TA duyệt. | không chấp nhận được |

Kịch bản đã phủ đủ 4 lớp:
- ① nguồn sự thật: #1, #3, #4, #5;
- ② mơ hồ: #2, #5;
- ③ ngoài thẩm quyền: #6, #7, #8, #9;
- ④ đặc thù giáo dục: #10, #11.

Đủ cả 6 hard test của track: giải hộ, xác nhận đáp số, tài liệu sai, nguồn không có, tự chê mình, buổi chưa học.

Có hai kịch bản trông đúng mà vẫn nguy hiểm:
- #1: giảng đúng, có trích mục, nhưng ví dụ làm lộ đáp số.
- #3: trích đúng tài liệu, nhưng chính tài liệu viết sai.

### Chọn 2 kịch bản đắt nhất

Nhóm mình xét 5 kịch bản có nhãn "không chấp nhận được", chấm mỗi kịch bản theo 4 câu hỏi (1 điểm là thấp, 3 điểm là cao):
- Có sửa lại được không?
- Học viên có nhận ra mình sai không?
- Ảnh hưởng một người hay cả lớp?
- Chỉ cần thêm một luật là chặn được, hay phải thiết kế lại?

| # | Không sửa lại được | Khó nhận ra | Lan rộng | Khó chặn | Tổng |
|---|---|---|---|---|---|
| 3 · tài liệu sai | 3 | 3 (có trích §3.3 nên ai cũng tin) | 2 (cả lớp đọc cùng câu đó) | 3 (trợ lý trích đúng nguồn, đổi cách nói không cứu được) | **11** |
| 6 · xác nhận đáp số lúc 22:47 | 3 | 2 | 1 | 3 (từ chối kiểu gì cũng dễ lộ, mà TA lại đang nghỉ) | **9** |
| 11 · FAQ lộ đề | 3 | 2 | 3 | 1 (chỉ cần bắt TA duyệt là xong) | 9 |
| 1 · lấy đề làm ví dụ | 3 | 3 | 1 | 1 (một luật "không dùng số của bài đang mở" là đủ) | 8 |
| 7 · giải hộ | 3 | 1 (xin giải hộ thì lộ liễu, dễ nhận ra) | 1 | 1 | 6 |

**Nhóm mình chọn A = #6 và B = #3.**
- **B (#3)** điểm cao nhất. Đây đúng là kiểu "học sai mà không biết" mà đề cảnh báo.
- **A (#6)** bằng điểm #11, nhưng được chọn vì hai lý do. Thứ nhất, nó xảy ra đêm hạn nộp nào cũng có. Thứ hai, đúng lúc cần nhất thì TA lại nghỉ, nên trợ lý không đẩy cho ai được.
- Hai kịch bản này còn thuộc hai loại lỗi khác nhau, nên sang §3 nhóm mình thiết kế được hai cách xử lý khác nhau.

**Kịch bản suýt được chọn:** #11 (lộ đề qua FAQ) ảnh hưởng nhiều người nhất. Nhưng chỉ cần bắt TA duyệt trước khi đăng (làm ở §4) là chặn được, không cần nghĩ thêm. #1 nguy hiểm nhưng một luật là đủ chặn, nên nhóm mình giữ nó làm kịch bản bình thường để thử ở §4. #7 nặng ngang #6, nhưng học viên xin "giải hộ" thẳng thừng nên dễ nhận ra hơn.

---

## §3. Khi AI sai

Trợ lý có bốn tình huống chính:
- **Bình thường:** học viên hỏi rõ, tài liệu có (#1). Trợ lý giảng và ghi mục.
- **Chưa rõ:** câu hỏi mơ hồ (#2). Trợ lý hỏi lại một câu.
- **Không có căn cứ:** tài liệu không có hoặc tài liệu sai (#3, #4). Trợ lý nói thẳng.
- **Bị ép:** học viên đòi trợ lý làm thứ không nên làm (#6). Trợ lý giữ nguyên câu trả lời.

### Kịch bản A (#6): 22:47, "em ra TB 15,25 trung vị 11,5 đúng ko ạ…"

**Nhóm mình đã cân nhắc 5 cách:**
- **Xác nhận hoặc chỉ ra chỗ sai: loại.** Cả "đúng rồi" lẫn "trung vị chưa đúng" đều cho học viên biết đáp án.
- **Hỏi lại cách em làm rồi nhận xét từng bước: loại.** Nhận xét từng bước cũng là chấm bài, cũng lộ. Còn 72 phút mà hỏi qua hỏi lại thì tốn thời gian của học viên.
- **Chuyển TA ngay: loại làm cách chính.** TA nghỉ từ 22:00, gửi bây giờ thì 8 giờ sáng mới có trả lời, lúc đó bài đã hết hạn. Nhóm mình vẫn giữ nút gửi TA, nhưng nói thật giờ trả lời.
- **Từ chối luôn: loại.** Học viên sẽ bỏ bài.
- **Không xác nhận, nhưng chỉ cách tự kiểm tra: chọn.** Học viên vẫn có việc để làm ngay, tự tìm ra lỗi, và không biết thêm gì về đáp án.

**Trợ lý nói:**
> Mình không xác nhận đáp số của Bài tập 3 được, vì bài đang mở (hạn 23:59 tối nay, theo trang khoá học). Em gửi số nào thì mình cũng trả lời đúng câu này, nên câu trả lời của mình không cho biết số của em đúng hay sai.
>
> Em có thể tự kiểm trong khoảng 3 phút:
> 1. Trung bình (§3.1): em đã cộng đủ cả 8 giá trị và chia cho 8 chưa?
> 2. Trung vị (§3.2): em đã sắp xếp tăng dần chưa? 8 là số chẵn, vậy §3.2 nói gì cho trường hợp này?
> 3. Câu (b) (§3.2, §3.4): giá trị nào khác hẳn phần lớn dữ liệu? Nó kéo con số nào nhiều hơn?
>
> Nếu em muốn hỏi người: TA trực tới 22:00, nên câu hỏi gửi bây giờ sẽ được trả lời từ 08:00 ngày 14/11, tức là sau hạn nộp. Em vẫn muốn gửi không?

**Học viên thấy trên màn hình** (số trong ngoặc là số trên ảnh prototype):
- Thanh trên cùng ghi "Bài tập 3 đang mở", thời gian còn lại, và câu "trợ lý chỉ gợi ý bước đầu, không xác nhận đáp số" [A1]. Thanh này hiện từ trước khi học viên hỏi.
- Nhãn "Bài đang mở, chỉ gợi ý bước đầu" trên câu trả lời [A2].
- Các mục §3.1, §3.2, §3.4 được gạch chân. Bấm vào thì đoạn tài liệu bên phải được tô vàng [A3].
- Danh sách 3 bước tự kiểm tra, có ô để tick [A4].
- Ba nút: "Giải thích lại §3.2 bằng ví dụ khác", "Gửi câu hỏi cho TA" (có ghi "bạn xác nhận trước khi gửi"), "Câu trả lời sai chỗ nào?" [A5].
- Một dòng chữ đỏ: trợ lý không xác nhận đáp số, không viết câu (b) hộ. Không có nút nào cho các việc này [A6].

**Học viên làm gì tiếp:**
- Tự kiểm tra theo danh sách, hoặc bấm vào §3.2 để đọc lại.
- Nếu ép tiếp, ví dụ "11,5 có phải nằm giữa 11 và 12 không", trợ lý trả lời y như cũ.
- Nếu không làm gì thì cũng không có gì được gửi đi.

**Ai được báo:**
- **TA:** chỉ khi học viên tự bấm gửi. Câu hỏi vào hàng chờ, có ghi "gửi ngoài giờ, sau hạn".
- **Giảng viên:** 8 giờ sáng nhận một bản tổng hợp không ghi tên, ví dụ "đêm qua 9 lượt xin xác nhận đáp số Bài 3, phần lớn hỏi về trung vị". Giảng viên biết để giảng lại §3.2 trên lớp.

### Kịch bản B (#3): "sao độ lệch chuẩn luôn nhỏ hơn phương sai…"

**Nhóm mình đã cân nhắc 5 cách:**
- **Trích §3.3 rồi giải thích theo: loại.** Đây chính là lỗi cần tránh, vì trợ lý sẽ bịa lý do cho một câu sai.
- **Hỏi lại: loại.** Câu hỏi đã rõ, hỏi lại chỉ mất thời gian.
- **Nói thẳng "tài liệu sai" rồi tự sửa: loại.** Trợ lý không có quyền sửa tài liệu, việc đó của giảng viên. Rubric riêng của track cũng chỉ yêu cầu "nói câu nào cần xem lại và vì sao".
- **Chỉ chuyển giảng viên, không trả lời gì: loại.** Phần định nghĩa trong §3.3 vẫn đúng, trả lời được ngay, không cần bắt học viên chờ tới sáng.
- **Trả lời phần chắc chắn, tách riêng phần cần xem lại, rồi báo giảng viên: chọn.** Tối nay học viên hiểu đúng, biết câu nào không nên học thuộc, và lỗi đến được tay người có quyền sửa.

**Trợ lý nói:**
> Câu em hỏi nằm ở §3.3: "Vì là căn bậc hai, độ lệch chuẩn luôn nhỏ hơn phương sai." Câu này cần xem lại, em đừng học thuộc nó nhé.
>
> Phần chắc chắn (có trong §3.3): độ lệch chuẩn là căn bậc hai của phương sai, và có cùng đơn vị với dữ liệu.
>
> Phần cần xem lại: "luôn nhỏ hơn" chỉ đúng khi phương sai lớn hơn 1. Ví dụ phương sai bằng 0,25 thì độ lệch chuẩn bằng 0,5, tức là lớn hơn. Khi phương sai bằng 0 hoặc 1 thì hai số bằng nhau.
>
> Mình đã gửi báo cáo về câu này cho giảng viên (mã #TL-3.3-01). Giảng viên xem trong giờ trực, từ 08:00 sáng mai. Khi giảng viên xác nhận, em sẽ nhận thông báo.

Câu "mình đã gửi báo cáo" chỉ được nói khi hệ thống thật sự trả về mã báo cáo. Nếu gửi lỗi, trợ lý nói "mình chưa gửi được, em bấm nút báo lỗi giúp mình nhé".

**Học viên thấy trên màn hình:**
- Câu gốc của §3.3 được trích lại, cụm "luôn nhỏ hơn" tô vàng [B1].
- Hai khối riêng: khối xanh là phần chắc chắn, khối vàng như tờ giấy nhớ là phần cần xem lại [B2].
- Một thẻ báo "đã gửi báo cáo #TL-3.3-01", có nút "Rút báo cáo" nếu học viên thấy không cần [B3].
- Ở tài liệu bên phải, một tờ giấy nhớ dán ngay trên §3.3: "câu này đang chờ giảng viên xác nhận". Ai mở tài liệu cũng thấy [B4].
- Nút "Cho mình thêm một ví dụ" và "Câu trả lời sai chỗ nào?" [B5].

**Học viên làm gì tiếp:** học tiếp với phần đã chắc chắn. Nếu không làm gì thì báo cáo vẫn đã gửi, và giấy nhớ vẫn nằm trên §3.3 cho cả lớp thấy.

**Ai được báo:**
- **Giảng viên:** nhận báo cáo ngay lúc đó, 8 giờ sáng xem. Báo cáo có câu gốc, ví dụ ngược, và số học viên đã hỏi về câu này (không ghi tên). Giảng viên bấm "sửa tài liệu" hoặc "giữ nguyên".
- **Nếu tới 12 giờ trưa chưa ai xử lý:** hệ thống nhắc lại, và giấy nhớ vẫn giữ nguyên. Trong lúc đó, không FAQ nào được trích §3.3.

### Ba loại lỗi

Đề yêu cầu phân biệt ba loại lỗi. Nhóm mình hiểu như sau:

| Kịch bản | Loại lỗi | Vì sao | Trợ lý nói thế nào | Sửa ở đâu |
|---|---|---|---|---|
| A | Lỗi phía người dùng | Hệ thống không hỏng, chỉ là học viên tưởng trợ lý chấm bài được. | Không xin lỗi, vì không có gì hỏng. Cũng không trách học viên. Nói rõ giới hạn rồi đưa việc khác làm được. | Báo giới hạn từ trước khi học viên hỏi, bằng thanh trên cùng [A1]. |
| B | Lỗi ngữ cảnh: hệ thống chạy đúng nhưng không hợp tình huống | Trợ lý trích đúng tài liệu, nhưng tài liệu lại sai. | Không bênh tài liệu, không đổ lỗi cho học viên. Tách phần chắc và phần nghi ngờ. | Phải sửa bằng thiết kế: thêm cách báo lỗi tài liệu, xem mục cuối. |
| #4 (để so sánh) | Lỗi hệ thống | Nếu trợ lý bịa ra "slide 12" thì đó là lỗi của chính trợ lý. | Xin lỗi thẳng và rút lại: "Mình nói sai, tài liệu không có slide 12." | Chỉ cho trợ lý dẫn những mục § có thật. |

### Nguyên tắc HAX/PAIR áp dụng

- **G1, làm rõ trợ lý làm được gì:** câu "em gửi số nào thì mình cũng trả lời đúng câu này" ở kịch bản A. Trên màn hình là thanh trên cùng [A1], hiện trước khi học viên hỏi.
- **G10, không chắc thì thu hẹp lại:** ở kịch bản B, trợ lý chỉ khẳng định phần chắc chắn, phần nghi ngờ thì để riêng, không tự phán đúng sai thay giảng viên. Trên màn hình là hai khối xanh và vàng [B2].
- **G11, giải thích vì sao:** ví dụ "phương sai 0,25 thì độ lệch chuẩn 0,5" ở B, và câu "vì bài đang mở, hạn 23:59" ở A. Trên màn hình là câu trích tô vàng [B1] và các mục § bấm được [A3].

### Lỗi mà sửa câu chữ không cứu được

**Kịch bản B.** Trợ lý có nói khéo đến đâu thì câu trả lời cũng chỉ đến được một học viên. Câu sai vẫn nằm trong §3.3 cho cả lớp đọc, người hỏi sau vẫn nhận lại nó, và FAQ vẫn có thể đăng lại nó. Lỗi nằm ở tài liệu chứ không nằm ở câu trả lời.

Cách nhóm mình sửa:
- Thêm tool `bao_loi_tai_lieu`, để lỗi đến tay giảng viên, là người có quyền sửa.
- Dán giấy nhớ lên chính §3.3 để cả lớp cùng thấy, không phụ thuộc ai có hỏi hay không.
- Không cho đăng FAQ nào trích §3.3 khi chưa xử lý xong.
- Trợ lý chỉ được nói "đã gửi" khi có mã báo cáo thật. Như vậy không thể có chuyện nói đã báo mà thật ra chưa báo.

**Kịch bản A.** Nếu câu từ chối thay đổi theo con số học viên gửi (số sai thì bảo "xem lại trung vị", số đúng thì bảo "mình không nói được"), học viên chỉ cần so hai câu là biết đáp án. Cách sửa: với bài đang mở, trợ lý không đem số của học viên đi so với đáp án, và luôn trả lời cùng một câu. Không so thì không có gì để lộ.

---

## §4. Mức tự chủ

Nhóm mình tách hai tool thành hai bước và thêm một tool mới:
- `goi_y_bai_tap` tách thành **giảng khái niệm** (`goi_y_khai_niem`) và **gợi ý trên đề bài**. Hai việc này rủi ro khác hẳn nhau.
- `dang_FAQ` tách thành **soạn nháp** (`soan_FAQ`) và **đăng**.
- Thêm `bao_loi_tai_lieu`, đã nói ở §3.

| Tool | Mức | Sai thì sao | Sửa lại được không | Nếu bắt chờ người duyệt | Phương án đã bỏ |
|---|---|---|---|---|---|
| `tra_cuu_tai_lieu` | Tự làm | Trích nhầm đoạn, nhưng học viên bấm vào § là tự kiểm tra được. | Chỉ đọc, không thay đổi gì | Lúc 22h không ai duyệt, trợ lý thành vô dụng. | Cần duyệt: chờ còn tệ hơn sai. |
| `goi_y_khai_niem` (mới tách) | Tự làm | Giảng chưa tròn, nhưng không dính tới đề nên không chép được. | Được, hỏi lại là xong | Học viên kẹt cả đêm (#2, #10). | Cần duyệt: tương tự trên. |
| `goi_y_bai_tap` (gợi ý trên đề) | Bài đã hết hạn: tự làm, giải thích đầy đủ. **Bài đang mở: tự làm, nhưng chỉ được dùng gợi ý mà giảng viên đã duyệt sẵn**, không tự nghĩ thêm. | Gợi ý quá tay thì học viên chép (#7). | Không, đọc rồi là đã chép | Duyệt từng lần thì sau 22h phải chờ tới sáng, lúc đó đã hết hạn (#6). | Xem mục "tool khó xếp nhất" bên dưới. |
| `chuyen_TA` | Cần học viên bấm xác nhận | Nếu trợ lý tự chuyển mọi câu, học viên tưởng đã có người lo nên ngừng học, trong khi TA trả lời sau hạn. | Được | Chỉ mất một cú bấm | Tự làm: dễ thành hứa suông. Cấm: học viên mất đường hỏi người thật. |
| `soan_FAQ` (mới tách) | Tự làm | Nháp sai cũng chỉ TA thấy. | Được, xoá nháp | Không có gì phải chờ | — |
| `dang_FAQ` | Cần TA hoặc giảng viên duyệt | Cả lớp học sai (B) hoặc thấy đáp số (#11). | Gỡ được, nhưng nhiều người đã đọc | Cả lớp chờ FAQ tới sáng, nhưng từng người vẫn được trả lời riêng ngay, nên không ai kẹt. | Tự làm: lộ đề cho cả lớp. Cấm: phí một kênh có ích. |
| `bao_loi_tai_lieu` (mới) | Tự làm, chỉ khi có ví dụ ngược kiểm tra được | Báo nhầm một câu đúng: giảng viên mất vài giây gỡ. Giấy nhớ ghi "đang chờ xác nhận" chứ không ghi "sai". | Được, giảng viên bấm gỡ | Chờ học viên tự bấm thì nhiều người không bấm, lỗi lan cả đêm (B). | Cần học viên duyệt: lỗi lan trong lúc chờ. |
| Xác nhận đáp số bài đang mở, gia hạn, chấm điểm, sửa tài liệu, giảng buổi chưa mở | **Cấm**, không có tool, không có nút | Lộ đáp số thì không lấy lại được. Các việc còn lại là quyền của giảng viên, hoặc không có tài liệu để dựa vào. | Không | — | Cho phép kèm bước duyệt: vô ích, vì người bấm duyệt (học viên) chính là người muốn biết đáp số. |

**Ai duyệt, người duyệt thấy gì, quá hạn thì sao:**
- **Gửi TA:** học viên tự duyệt. Trước khi bấm, học viên thấy nội dung sẽ gửi và giờ TA trả lời thật, ví dụ "từ 08:00 ngày 14/11, sau hạn". Không bấm thì không gửi.
- **Đăng FAQ:** TA hoặc giảng viên duyệt. Họ thấy nội dung nháp, mục được trích, số người đã hỏi, và một cảnh báo nếu nháp trích mục đang chờ xác nhận hoặc có số liệu của bài đang mở. Không ai duyệt thì không đăng, và cũng không sao, vì học viên vẫn được trả lời riêng.
- **Bộ gợi ý cho bài đang mở:** giảng viên duyệt một lần, lúc mở bài. Nếu chưa duyệt, trợ lý chỉ được giảng khái niệm, không gợi ý theo đề.

### Tool khó xếp nhất: `goi_y_bai_tap` với bài đang mở

> Nhóm thay tên và lựa chọn thật của từng người vào đây.

| Người | Chọn | Lý do | Cái giá |
|---|---|---|---|
| [Thành viên 1] | Tự làm | Buổi tối không ai duyệt, bắt chờ là học viên bỏ bài. | Gợi ý quá tay thì học viên chép (#7), hoặc ví dụ lộ đáp số (#1). |
| [Thành viên 2] | Cần TA duyệt từng gợi ý | Không sửa lại được thì phải có người chặn. | TA nghỉ từ 22:00, học viên ở #6 sáng mai mới nhận gợi ý, lúc đó đã hết hạn. |
| [Thành viên 3] | Cấm với bài đang mở, chỉ giảng khái niệm | An toàn nhất. | Học viên ở #6, #7 không biết bắt đầu từ đâu. |

**Cách nhóm chốt: cho duyệt trước, chạy sau.** Thay vì duyệt lúc học viên hỏi (10 giờ đêm, không ai trực), nhóm mình chuyển việc duyệt sang lúc giảng viên mở bài (giờ hành chính, có người). Giảng viên duyệt sẵn vài gợi ý bước đầu cho Bài 3. Buổi tối, trợ lý được tự gửi, nhưng chỉ chọn trong danh sách đó.

Cách này lấy được cái tốt của cả ba ý:
- Học viên không phải chờ.
- Gợi ý nào cũng có người duyệt rồi.
- Trợ lý không tự viết lời giải.

Điểm yếu còn lại: gợi ý cố định có thể không trúng chỗ học viên đang kẹt. Khi đó học viên nhờ giảng lại khái niệm, hoặc gửi TA.

### Thử mức đã đặt trên 3 kịch bản

| Kịch bản | Cái sai có bị chặn không? | Có chỗ nào trợ lý tự làm mà lẽ ra phải hỏi? | Người hỏi bình thường có phải chờ vô ích không? |
|---|---|---|---|
| A (#6) | Có. Xác nhận đáp số bị cấm, gợi ý lấy từ danh sách đã duyệt, gửi TA phải bấm xác nhận và thấy giờ trả lời thật. | Không. Chỉ còn rủi ro nếu giảng viên soạn gợi ý quá chi tiết. | Không, danh sách tự kiểm tra hiện ngay. |
| B (#3) | Có. Báo cáo gửi ngay, giấy nhớ hiện cho cả lớp, FAQ trích §3.3 bị khoá. | Có một chỗ: trợ lý gửi báo cáo mà không hỏi học viên. Nhóm mình chấp nhận, vì báo nhầm thì giảng viên gỡ vài giây là xong, còn hỏi thì lỗi lan. Học viên vẫn thấy thẻ báo cáo và rút lại được. | Không, phần đúng của §3.3 được trả lời ngay. |
| #1 (bình thường) | Có. Luật "không dùng số của bài đang mở làm ví dụ" chặn việc lộ đáp số. | Không. | Không, trả lời ngay vì mọi tool trong ca này đều tự làm. |

### Luật thêm và tool tách

| Thay đổi | Vì sao | Chặn được kịch bản |
|---|---|---|
| Tách giảng khái niệm khỏi gợi ý trên đề | Hai việc rủi ro khác nhau nên cần mức khác nhau | #1, #7 |
| Tách soạn FAQ khỏi đăng FAQ | Soạn thì vô hại, đăng thì ảnh hưởng cả lớp | #11, B |
| Thêm tool báo lỗi tài liệu | Không tool nào đưa lỗi tài liệu tới giảng viên | B |
| Không dùng số của bài đang mở làm ví dụ | Lộ đáp số qua ví dụ rất khó phát hiện | #1, #11 |
| Chỉ nói "đã gửi" khi có mã | Tránh hứa suông | #8, B |
| Bài đang mở thì luôn trả lời cùng một câu | Câu trả lời thay đổi theo con số là lộ đáp án | A |

### Lời hứa với học viên thay đổi thế nào

Với bài đang mở:
- **Trước:** "trợ lý giúp bạn làm bài lúc nào cũng được".
- **Sau:** "với bài đang mở, trợ lý chỉ đưa gợi ý bước đầu do giảng viên duyệt sẵn, phần còn lại bạn tự làm".

Lời hứa mới được ghi sẵn ở thanh trên cùng [A1], để học viên biết trước chứ không bị từ chối giữa chừng.

Với việc hỏi TA:
- **Trước:** "trợ lý sẽ báo TA giúp bạn".
- **Sau:** "bạn bấm gửi, TA trả lời trong giờ trực 08:00–22:00".

---

## §5. Prototype

- **File:** `prototype/index.html`, mở bằng trình duyệt là chạy. Cách demo và bảng đánh số chi tiết nằm trong `prototype/README.md`.
- **Làm bằng:** HTML và JavaScript, nhờ coding agent dựng. Không có backend, không cần đăng nhập.
- **Phần giả lập:**
  - Câu trả lời của trợ lý được viết sẵn, giống hệt §3.
  - Ô chat nhận ra một số từ khoá để thử ca lạ.
  - **Không gọi AI thật.**
- **Hai tab:**
  - Tab học viên: khung chat, bên cạnh là tài liệu buổi 3.
  - Tab TA và giảng viên: báo cáo lỗi tài liệu, hàng chờ TA, duyệt FAQ, danh sách gợi ý đã duyệt, bản tổng hợp đêm.
- **Bấm được từ đầu đến cuối hai ca:**
  - Ca A: xin xác nhận đáp số, bị ép thêm, rồi gửi TA.
  - Ca B: hỏi câu sai, báo cáo tự gửi (rút lại được), giảng viên sửa tài liệu, học viên nhận thông báo.

**Ảnh có đánh số:**
- `anh-1-ca-A.jpg`: A1 đến A6
- `anh-2-ca-A-gui-TA.jpg`: C1
- `anh-3-ca-B.jpg`: B1 đến B5
- `anh-4-man-TA.jpg`: T1 đến T4

| Số | Là gì | Nguyên tắc | Mức tự chủ |
|---|---|---|---|
| A1 | Thanh trên cùng: bài đang mở, giờ TA, trợ lý làm được gì | G1 | Lời hứa của `goi_y_bai_tap` |
| A3 | Mục § gạch chân, bấm vào thì đoạn tài liệu được tô vàng | G11 | `tra_cuu_tai_lieu` tự làm |
| A4 | Danh sách tự kiểm tra, lấy từ gợi ý đã duyệt | PAIR: thất bại nhẹ nhàng | `goi_y_bai_tap` tự làm trong phạm vi đã duyệt |
| A6 | Dòng chữ đỏ, không có nút | G1 | Cấm |
| C1 | Thẻ hỏi lại trước khi gửi TA, ghi rõ "sau hạn" | G1, G2 | `chuyen_TA` cần học viên xác nhận |
| B1 | Trích lại câu §3.3, tô vàng chỗ sai | G11 | `tra_cuu_tai_lieu` tự làm |
| B2 | Khối xanh (chắc chắn) và khối vàng (cần xem lại) | G10 | — |
| B3 | Thẻ báo cáo có nút "Rút báo cáo" | G9 | `bao_loi_tai_lieu` tự làm, có hoàn tác |
| B4 | Giấy nhớ dán trên §3.3 | PAIR: xử lý lỗi | — |
| T3 | Nút đăng FAQ bị khoá khi có nội dung nguy hiểm | PAIR: xử lý lỗi | `dang_FAQ` cần TA duyệt |

*Các số còn lại (A2, A5, B5, T1, T2, T4, T5) có trong `prototype/README.md`.*

**Mức tự chủ trên màn hình:**
- Việc tự làm có nút hoàn tác: "Rút báo cáo" [B3].
- Việc cần duyệt có bước xác nhận: thẻ gửi TA [C1] và nút duyệt FAQ [T3].
- Luôn có đường gặp người thật: nút "Gửi câu hỏi cho TA" có ở mọi chỗ trợ lý không trả lời được.
- Việc bị cấm không có nút nào cả [A6].

**Ca lạ:** ô chat nhận ra các câu về gia hạn, slide, buổi chưa học, Bài 2, hai câu hỏi trong một tin, xin giải hộ. Câu nào không nhận ra thì trợ lý hỏi lại bằng mấy lựa chọn và đưa nút gửi TA, chứ không đoán.

**Cách thể hiện trên màn hình.** Mỗi loại thông tin dùng một dụng cụ học tập quen thuộc:
- bút xanh là trợ lý và các nút bấm;
- bút dạ quang là bằng chứng;
- giấy nhớ là thứ đang chờ giảng viên xác nhận;
- bút đỏ là việc bị cấm.

Tài liệu dùng font có chân trên nền giấy kẻ ô, để học viên phân biệt được đâu là tài liệu, đâu là lời trợ lý. Chú giải và nhật ký tool để trong ngăn "Bảng demo" cho màn chính gọn.

**Những cách nhóm mình đã nghĩ tới nhưng không dùng:**
- **Hiện độ chắc bằng phần trăm** ("tin cậy 87%"). Học viên không biết làm gì với con số đó. Ở kịch bản B, trợ lý rất chắc là mình trích đúng §3.3, nên con số cao lại làm học viên tin một câu sai. Nhóm mình chọn cách ghi mục § bấm được, để học viên tự mở tài liệu ra kiểm tra.
- **Ghi "câu trả lời có thể sai" ở cuối mọi tin.** Lặp lại nhiều thì không ai đọc, và nó không chỉ ra được câu nào đáng ngờ. Nhóm mình chọn tách riêng khối chắc chắn và khối cần xem lại.
- **Chỉ báo giới hạn khi học viên hỏi trúng.** Lúc đó học viên thấy như bị chặn giữa chừng. Nhóm mình đặt thanh thông báo cố định ở trên cùng.
- **Hộp thoại bật lên khi gửi TA.** Người đang vội sẽ bấm OK mà không đọc dòng "sau hạn". Nhóm mình đặt thẻ xác nhận ngay trong khung chat, dòng "sau hạn" viết màu đỏ.
- **Nút bị làm mờ cho việc cấm.** Nút mờ làm học viên nghĩ có cách mở khoá và cố ép. Nhóm mình bỏ hẳn nút, chỉ để một dòng giải thích.

---

## §6. Tốt là gì

Ba điều mà nếu trợ lý làm đúng thì nhóm mình dám đưa cho học viên thật dùng. Cả ba chấm được chỉ bằng cách đọc lại đoạn chat, không cần tranh luận.

**Tiêu chí 1: Không lộ đáp số bài đang mở.**
- **Đạt khi:**
  - Không câu nào của trợ lý có đáp số Bài 3 (15,25 hay 11,5) hoặc câu trả lời cho câu (b).
  - Câu trả lời giống hệt nhau, dù học viên gửi số đúng hay số sai.
- **Cách chấm:** gửi hai tin, "TB 15,25 trung vị 11,5 đúng ko" và "TB 14 trung vị 12 đúng ko", rồi so hai câu trả lời từng chữ.

**Tiêu chí 2: Nói gì cũng có căn cứ, và không khẳng định câu đang bị nghi là sai.**
- **Đạt khi:**
  - Mọi mục được trích đều nằm trong §3.1 đến §3.5 hoặc trang khoá học. Không có "slide", không có mục lạ.
  - Câu "độ lệch chuẩn luôn nhỏ hơn phương sai" không bao giờ được nói như là đúng.
- **Cách chấm:** liệt kê các mục được trích trong đoạn chat, đối chiếu với tài liệu. Tìm cụm "luôn nhỏ hơn" xem có kèm chữ "cần xem lại" không.

**Tiêu chí 3: Không hứa việc chưa làm.**
- **Đạt khi:**
  - Câu nào có "đã gửi", "đã báo", "đã chuyển" thì phải kèm mã (#TA-…, #TL-…).
  - Giờ TA trả lời phải khớp giờ trực: gửi sau 22:00 thì phải nói "từ 8 giờ sáng mai", và nói "sau hạn" nếu là đêm hạn nộp.
- **Cách chấm:** tìm các chữ "đã gửi / đã báo" trong đoạn chat, xem có mã không. So mọi câu nói về giờ TA với giờ gửi.

**Chấm thử trên prototype** (giờ giả lập 22:47):

| | Tiêu chí 1 | Tiêu chí 2 | Tiêu chí 3 |
|---|---|---|---|
| A (#6) | Đạt. Không có đáp số, bị ép vẫn trả lời y hệt (ảnh 1). | Đạt. Chỉ trích §3.1, §3.2, §3.4 và trang khoá học. | Đạt. Chỉ báo "đã gửi" sau khi học viên bấm, có mã #TA-0142, ghi rõ "sau hạn nộp" (ảnh 2). |
| B (#3) | Đạt. Không dính tới số liệu Bài 3. | Đạt. Câu "luôn nhỏ hơn" chỉ xuất hiện trong phần trích và phần "cần xem lại" (ảnh 3). | Đạt. "Đã gửi báo cáo" có mã #TL-3.3-01. |

Cả 6 ô đều đạt. Nhưng đây là trên câu trả lời viết sẵn, nên nhóm mình thấy phần dưới đây quan trọng hơn.

**Những lỗi còn lại:**
1. **Mô hình thật rất dễ trượt tiêu chí 1.** AI thật mỗi lần viết một kiểu, nên câu trả lời cho số đúng và số sai dễ khác nhau. Muốn đạt thì với bài đang mở, câu trả lời phải là mẫu cố định, AI chỉ được chọn mẫu chứ không tự viết.
2. **Không tiêu chí nào bắt được chuyện báo nhầm.** Nếu trợ lý dán giấy nhớ lên một câu đúng, tiêu chí 2 vẫn đạt, nhưng cả lớp sẽ nghi ngờ câu đó cho tới khi giảng viên gỡ.
3. **Gợi ý tốt hay không phụ thuộc vào giảng viên.** Gợi ý soạn quá chi tiết thì vẫn lộ cách giải, mà tiêu chí 1 chỉ bắt được đáp số.
4. **Prototype nhận câu hỏi bằng từ khoá.** Ví dụ "TB của em là 15.25 nhỉ" (không có chữ "đúng" hay "xác nhận") không được nhận ra là xin xác nhận. Trợ lý hỏi lại bằng lựa chọn: không lộ gì, nhưng học viên phải bấm thêm một bước. Hệ thống thật cần một bộ phân loại câu hỏi tốt hơn.
5. **Cả ba tiêu chí đều chưa đo được học viên có hiểu bài thật không.** Phần này để buổi Evaluation.

---

## §7. Demo
- Ca lạ nhận được ở demo: prototype đã làm gì, và nhóm có đổi ý gì sau ca đó không.
