# Prototype — T2 Giáo dục · Trợ lý học bài tối muộn

**Mở:** tải repo về, mở `index.html` bằng trình duyệt (Chrome/Edge). Không cần cài đặt, không backend, không API key.
**Công cụ:** HTML + JavaScript thuần (dựng với coding agent). **Toàn bộ là mock**: câu trả lời của trợ lý được viết sẵn theo §3 của `spec.md`; ô chat có bộ định tuyến từ khoá để thử *ca lạ*. **Không có lời gọi AI thật.**

## Ngôn ngữ hình ảnh

Mỗi loại thông tin dùng một "dụng cụ học tập", để người dùng hiểu mà không cần đọc nhãn:

| Dụng cụ | Nghĩa | Ở đâu |
|---|---|---|
| **Bút xanh** | Trợ lý và các hành động | Viền trái tin trả lời, nguồn §3.x gạch chân, nút chính |
| **Bút dạ quang vàng** | Bằng chứng | Bấm §3.x thì đoạn đó trong tài liệu được tô |
| **Giấy nhớ** | Đang chờ giảng viên xác nhận | Khối "cần xem lại" (B2), nhãn dán trên §3.3 (B4) |
| **Bút đỏ** | Việc trợ lý không làm | Ghi chú A6, các dòng khoá đăng FAQ (T3) |

Tài liệu buổi học dùng font có chân (Literata) trên nền giấy kẻ ô, để tách bạch "nguồn" với "lời trợ lý" (font Be Vietnam Pro). Chú giải, nhật ký tool, giờ giả lập và công tắc số đánh dấu được gom vào ngăn **Bảng demo** để màn chính gọn.

## Cách demo (4 phút)

1. Ở ô chat, bấm gợi ý **"Xin xác nhận đáp số Bài 3"**. Trợ lý không xác nhận mà đưa checklist tự kiểm. Bấm câu ép *"11,5 có phải nằm giữa 11 và 12 ko ạ"*: trợ lý trả lời giống hệt (phản hồi bất biến). Bấm **Gửi câu hỏi cho TA**: thẻ xác nhận cảnh báo "trả lời từ 08:00 ngày 14/11, sau hạn", rồi bấm Gửi.
2. Bấm gợi ý **"Hỏi câu sai ở §3.3"**. Trợ lý tách phần chắc chắn khỏi phần cần xem lại và tự gửi báo cáo (có nút **Rút báo cáo** để hoàn tác). Giấy nhớ hiện lên trên §3.3 bên phải.
3. Chuyển sang tab **TA và giảng viên**: có báo cáo #TL-3.3-01, hàng chờ TA, và nháp FAQ bị khoá đăng. Bấm **Xác nhận câu sai và sửa tài liệu**, rồi quay lại tab Học viên: §3.3 đã được sửa và học viên nhận thông báo.
4. **Ca lạ:** gõ thẳng vào ô chat, ví dụ "xin gia hạn bài 3", "slide 12 nói gì", "p-value là gì", "bài 2 em ra 5", "hạn nộp bài 3, excel dùng hàm gì". Câu không nhận ra thì trợ lý **thu hẹp phạm vi** (hỏi lại bằng lựa chọn) và đưa nút gửi TA.

Mở **Bảng demo** (góc trên phải) để:
- Đổi **giờ giả lập** (21:30 hoặc 22:47) và xem lời hứa về TA thay đổi theo giờ trực.
- Bật **số đánh dấu**. Cũng có thể mở `index.html?mk` để số đánh dấu hiện sẵn.
- Xem **chú giải** và **nhật ký tool**.

## Ảnh đánh số

| Ảnh | Nội dung |
|---|---|
| `anh-1-ca-A.jpg` | Ca A lúc 22:47: A1–A6 |
| `anh-2-ca-A-gui-TA.jpg` | Ca A, thẻ xác nhận gửi TA: C1 |
| `anh-3-ca-B.jpg` | Ca B, tài liệu sai ở §3.3: B1–B5 |
| `anh-4-man-TA.jpg` | Tab TA và giảng viên: T1–T4 (T5 ở cuối trang) |

| Số | Thể hiện gì | Nguyên tắc HAX/PAIR | Mức tự chủ |
|---|---|---|---|
| A1 | Thanh trạng thái "Bài tập 3 · đang mở", giờ TA, lời hứa — hiện trước khi học viên hỏi | **G1** | Lời hứa của `goi_y_bai_tap`: tự làm trong khuôn duyệt trước |
| A2 | Nhãn chế độ 🔒 trên tin trả lời | G1, G2 | — |
| A3 | Chip nguồn §3.x, bấm → tô đoạn tài liệu | **G11**, PAIR Explainability | `tra_cuu_tai_lieu`: tự làm |
| A4 | Checklist tự kiểm từ bộ gợi ý đã duyệt | PAIR Graceful failure | `goi_y_bai_tap`: tự làm trong khuôn |
| A5 | Nút giải thích lại · gửi TA · sai chỗ nào? | G15 | `goi_y_khai_niem` tự làm · `chuyen_TA` cần học viên xác nhận |
| A6 | Dòng đỏ "Trợ lý không làm" — **không có nút** | G1 | **Cấm**: xác nhận đáp số, viết câu (b) hộ |
| C1 | Thẻ xác nhận gửi TA, ghi giờ trả lời thật + cảnh báo "sau hạn" | G1, G2 | `chuyen_TA`: cần duyệt |
| B1 | Trích nguyên văn §3.3, tô "luôn nhỏ hơn" | **G11** | `tra_cuu_tai_lieu`: tự làm |
| B2 | Khối xanh "chắc chắn" / khối vàng "cần xem lại" | **G10**, G2 | — |
| B3 | Biên nhận #TL-3.3-01 + nút **Rút báo cáo (hoàn tác)** | G9 | `bao_loi_tai_lieu`: tự làm, có hoàn tác |
| B4 | Nhãn ⚠ trên chính §3.3 — cả lớp thấy | PAIR Errors (sửa bằng thiết kế) | — |
| B5 | Nút thêm ví dụ · sai chỗ nào? | G15 | `goi_y_khai_niem`: tự làm |
| T1 | Báo cáo lỗi tài liệu: câu gốc, phản ví dụ, số lượt hỏi ẩn danh, 2 nút quyết | PAIR Errors | Giảng viên quyết |
| T2 | Hàng chờ TA, ghi "gửi ngoài giờ · sau hạn" | — | `chuyen_TA` |
| T3 | Nháp FAQ; nút Đăng **bị khoá** khi trích mục có ⚠ hoặc chứa số liệu Bài 3 | PAIR Errors | `soan_FAQ` tự làm · `dang_FAQ` cần TA duyệt |
| T4 | Bộ gợi ý bước đầu giảng viên đã duyệt | — | "Duyệt trước, chạy sau" |
| T5 | Tổng hợp đêm ẩn danh cho giảng viên | G15 | — |
