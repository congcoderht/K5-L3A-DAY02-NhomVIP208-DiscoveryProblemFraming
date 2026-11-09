# Báo cáo cá nhân — 2A202603583_LeQuangLinh

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Lê Quang Linh
- MSSV: 2A202603583
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: NhomVIP208
- Link repo nhóm: https://github.com/congcoderht/K5-L3A-DAY02-NhomVIP208-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi tổng kết tuần làm việc, tôi muốn tổng hợp các đầu việc hoàn thành, việc tồn đọng và blocker từ Jira/Slack/Trello, để xuất báo cáo tiến độ (weekly status report) cho ban quản lý. | Bản thân, Project Manager, 4 thành viên trong dự án | Mất 60 phút mỗi chiều thứ Sáu; thao tác thủ công mở từng board Jira và copy-paste vào Confluence; lịch sử commit báo cáo đều đặn 12 tuần liên tiếp. |
| 2 | Tốn thời gian | Khi đối soát danh sách khách hàng và dữ liệu xuất từ CRM/database nội bộ, tôi muốn rà soát và làm sạch các trường dữ liệu bị trùng lặp, sai định dạng số điện thoại/email, để nạp vào hệ thống marketing mà không bị lỗi bounce. | Chuyên viên vận hành dữ liệu, Sales Ops | Mất 90 phút cho mỗi đợt 500 bản ghi; tần suất 2 lần/tháng; tháng trước ghi nhận 2 lần chiến dịch email bị tạm dừng do dữ liệu chứa ký tự lạ gây lỗi parser. |
| 3 | Cần đọc, tổng hợp nhiều thông tin | Khi thẩm định tài liệu kỹ thuật hoặc báo cáo phân tích đối thủ cạnh tranh (15–20 trang), tôi muốn bóc tách nhanh các tính năng chính, bảng giá và công nghệ sử dụng, để lập bảng so sánh đối chuẩn (benchmarking) phục vụ họp chiến lược. | Product Owner, Business Analyst, Tech Lead | Mất 3–4 tiếng đọc lướt và ghi chép tay sang bảng tính; mỗi quý làm 2 đợt; có tài liệu nháp 4 trang bảng so sánh bị lệch thông tin giữa các phiên bản. |
| 4 | Pain từ người khác | Khi nhân sự mới gia nhập công ty, HR/IT Admin muốn đối chiếu thông tin cá nhân với checklist tài khoản nội bộ (email, Slack, GitHub, VPN), để cấp quyền truy cập đúng tiến độ mà không bị sót quyền. | IT Support / HR Operations | IT Support mất 45 phút cho mỗi nhân sự mới; trung bình onboarding 5–7 người/tháng; có 3 ticket phàn nàn trong tháng qua vì nhân sự mới phải đợi nửa ngày mới đủ quyền truy cập. |
| 5 | Lặp lại | Khi kết thúc cuộc họp nội bộ với các bên liên quan (stakeholders), tôi muốn trích xuất các quyết định và đầu việc được giao (action items) kèm deadline cụ thể, để gửi email xác nhận biên bản họp (meeting recap). | Người chủ trì cuộc họp, các bên liên quan (6–8 người) | Mất 30–40 phút nghe lại bản ghi hoặc rà soát ghi chú sau cuộc họp kéo dài 1 tiếng; tần suất 3 cuộc họp/tuần; từng có 2 sự việc chậm tiến độ do hiểu nhầm người chịu trách nhiệm chính. |
| 6 | Cần đọc, tổng hợp nhiều thông tin | Khi nhận tài liệu yêu cầu thay đổi (Change Request) hoặc phản hồi từ đối tác/khách hàng qua nhiều chuỗi email và file đính kèm, tôi muốn phân loại các mục ảnh hưởng đến hợp đồng hoặc tiến độ, để chuyển tiếp chính xác cho bộ phận pháp chế/kỹ thuật. | Quản lý dự án (PM), Account Manager | Mất trung bình 2 tiếng đọc rà soát chuỗi email dài 20–30 phản hồi; phát sinh khoảng 1–2 lần/tháng; từng bị đối tác nhắc nhở do bỏ sót một yêu cầu chỉnh sửa ở giữa chuỗi thư. |
| 7 | Tốn thời gian | Khi nhận các file ghi âm cuộc họp khách hàng kéo dài 60–90 phút, tôi muốn định vị nhanh các mốc thời gian khách hàng chốt yêu cầu kỹ thuật hoặc phản hồi về chi phí, để cập nhật vào hồ sơ dự án mà không phải nghe lại toàn bộ file. | Tech Lead, Account Executive | Mất 50–60 phút tua lại file ghi âm sau mỗi buổi làm việc; tần suất 1 lần/tuần; tuần trước mất gần 1.5 tiếng chỉ để xác minh lại 1 mốc cam kết tiến độ với khách hàng. |
| 8 | Pain từ người khác | Khi gửi yêu cầu hoàn ứng hoặc thanh toán hóa đơn công tác, nhân viên các phòng ban muốn tra cứu nhanh chính sách và định mức chi phí hợp lệ, để không bị bộ phận kế toán trả lại hồ sơ yêu cầu làm lại. | Nhân viên toàn công ty, Phòng Kế toán | Kế toán mất trung bình 3 tiếng mỗi kỳ quyết toán cuối tháng để giải thích lại quy định; tỷ lệ hồ sơ bị trả về lần đầu chiếm khoảng 25% tổng số yêu cầu nộp lên. |

- **Ý AI gợi ý mà tôi giữ lại:** AI gợi ý lăng kính *"Cần đọc, tổng hợp nhiều thông tin"* về việc phân tích tài liệu thị trường. Tôi đã điều chỉnh lại theo đúng thực tế vận hành doanh nghiệp: *"Khi thẩm định tài liệu kỹ thuật hoặc báo cáo phân tích đối thủ cạnh tranh (15–20 trang), tôi muốn bóc tách nhanh các tính năng chính, bảng giá và công nghệ sử dụng, để lập bảng so sánh đối chuẩn"* (dòng #3). Bổ sung các thông số đo lường thật: tốn 3–4 tiếng đọc lướt, tần suất 2 đợt/quý và bằng chứng tài liệu nháp bị lệch số liệu.
- **Ý AI gợi ý mà tôi bỏ qua:** AI gợi ý *"Khi quản lý chi tiêu cá nhân hoặc nhân sự nghỉ phép, nhân viên muốn có chatbot tự động phê duyệt đơn"*. Tôi loại bỏ vì:
  1. Gợi ý này vi phạm nguyên tắc "Problem first" khi cố đưa giải pháp "chatbot tự động duyệt" vào.
  2. Về mặt vận hành doanh nghiệp, quy trình phê duyệt nghỉ phép hay chi tiêu đòi hỏi thẩm quyền quản lý và chính sách tuân thủ (compliance) chặt chẽ, không thể tự tiện ủy quyền hoàn toàn cho bot mà không qua quy trình kiểm soát.
---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Bóc tách và lập bảng so sánh đối chuẩn (benchmarking) tính năng/chi phí từ tài liệu kỹ thuật của đối thủ hoặc nhà cung cấp. | Tốn nhiều thời gian nhất (3–4 tiếng/lần), ảnh hưởng trực tiếp đến chất lượng ra quyết định của ban lãnh đạo và định hướng phát triển sản phẩm. | Định dạng tài liệu của các nhà cung cấp/đối thủ rất đa dạng (file PDF, brochure, bảng thông số kỹ thuật) nên việc chuẩn hóa trường dữ liệu có thể gặp trở ngại. |
| 2 | Rà soát và làm sạch dữ liệu khách hàng xuất từ CRM/database nội bộ trước khi nạp vào hệ thống chiến dịch. | Gây gián đoạn chiến dịch marketing, làm tăng tỷ lệ email bounce và có nguy cơ làm hỏng uy tín tên miền (domain reputation) của doanh nghiệp. | Chưa rõ bộ quy tắc lọc (Rule-based Regex) kết hợp script nội bộ đã đủ bao phủ các trường hợp lỗi chưa, hay bắt buộc phải cần phân tích ngữ cảnh. |
| 3 | Trích xuất các quyết định và đầu việc được giao (action items) kèm deadline từ biên bản/bản ghi cuộc họp điều hành với các bên liên quan. | Diễn ra thường xuyên (3 lần/tuần), nếu bỏ sót việc sẽ dẫn đến chậm tiến độ cam kết giữa các phòng ban hoặc với khách hàng. | Văn phong trao đổi trong cuộc họp nhiều khi không theo cấu trúc chuẩn, các cam kết thường được chốt ngầm hoặc sửa đổi qua lại nhiều lần. |



### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi thẩm định tài liệu kỹ thuật hoặc hồ sơ năng lực của nhà cung cấp/đối thủ (15–20 trang), tôi muốn bóc tách nhanh các thông số kỹ thuật, bảng giá và giới hạn hệ thống, để lập bảng so sánh đối chuẩn phục vụ cuộc họp đánh giá kỹ thuật. |
| Actor | Product Owner / Business Analyst / Kỹ sư giải pháp (Solution Engineer). |
| Thời điểm / bối cảnh | Giai đoạn đánh giá giải pháp công nghệ mới hoặc chuẩn bị hồ sơ đấu thầu/so sánh đối tác (khoảng 2 tuần/lần). |
| Quy trình hiện tại (3–7 bước) | 1. Tiếp nhận và mở 3–4 tài liệu giải pháp định dạng PDF (10 phút). Đọc lướt phần tổng quan cấu trúc kiến trúc và danh mục tính năng (45 phút). Tìm đến phần bảng giá, điều kiện cấp phép (license) và giới hạn tải/băng thông, chép thủ công các thông số vào Google Sheets (90 phút). Đối chiếu chéo các tiêu chí kỹ thuật tương đương giữa các bên (45 phút). Tổng hợp lại thành bảng so sánh hoàn chỉnh trình ban quản lý (20 phút). |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 & Bước 4: Mất tổng cộng 135 phút để đọc lướt, trích xuất thông số kỹ thuật và chuẩn hóa các tiêu chí so sánh giữa nhiều tài liệu không đồng nhất cấu trúc. |
| Impact (nếu không giải thì sao) | Tốn 3.5 – 4 tiếng cho mỗi lượt thẩm định; dễ ghi chép nhầm số liệu chi phí hoặc bỏ sót điều khoản ràng buộc kỹ thuật, dẫn đến việc chọn sai nhà cung cấp hoặc lập dự toán ngân sách sai lệch. |
| Success metric (baseline → target) | - Thời gian trích xuất và lập bảng so sánh sơ bộ: từ 210 phút giảm xuống dưới 45 phút. Độ chính xác của các thông số kỹ thuật trích xuất: đạt tối thiểu 90% (kiểm tra lại thủ công tối đa 2 điểm cần đính chính/bảng). |
| Phương án không dùng AI | Sử dụng một template bảng tính chuẩn hóa (RFP template) gửi cho nhà cung cấp tự điền trước; kết hợp tính năng tìm kiếm từ khóa nâng cao trên phần mềm đọc PDF chuyên dụng. |
| Giả thuyết về AI (nếu có) | AI (Workflow) nhận file tài liệu, nhận diện các bảng biểu/đoạn văn bản chứa thông số kỹ thuật theo schema định sẵn (Tên tính năng, Mức giá, SLA, Giới hạn hệ thống), sau đó xuất dữ liệu có cấu trúc ra bảng Markdown/Excel. |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
[Nhận và mở 3-4 tài liệu giải pháp] (10')
[Đọc lướt cấu trúc & tính năng] (45')
[BÓC TÁCH BẢNG GIÁ & THÔNG SỐ VÀO BẢNG TÍNH] (90') <--- [BOTTLENECK CHÍNH]
[ĐỐI CHIẾU CHÉO TIÊU CHÍ KỸ THUẬT TƯƠNG ĐƯƠNG] (45') <--- [BOTTLENECK PHỤ]
[Tổng hợp bảng so sánh hoàn chỉnh] (20')
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi đối soát danh sách khách hàng và dữ liệu xuất từ CRM/database nội bộ, tôi muốn rà soát và làm sạch các trường dữ liệu bị trùng lặp, sai định dạng số điện thoại/email, để nạp vào hệ thống marketing mà không bị lỗi bounce. |
| Actor | Chuyên viên vận hành dữ liệu (Data Ops) / Sales Operations. |
| Thời điểm / bối cảnh | Mỗi khi xuất file dữ liệu định kỳ chuẩn bị cho các đợt gửi thông báo hoặc chiến dịch tiếp cận khách hàng mới (khoảng 2 lần/tháng, mỗi đợt 500–1.000 dòng). |
| Quy trình hiện tại (3–7 bước) | 1. Xuất file thô từ CRM ra định dạng `.csv` hoặc `.xlsx` (10 phút). Chạy tính năng Remove Duplicates mặc định của Excel (10 phút). Mở file, rà soát bằng mắt các trường họ tên bị lỗi font, số điện thoại thiếu mã vùng hoặc email chứa khoảng trắng/ký tự lạ (60 phút). Sửa thủ công từng dòng phát hiện lỗi (30 phút). Chạy thử nghiệm gửi kiểm tra (test broadcast) để kiểm tra lỗi hệ thống (10 phút). |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 & Bước 4: Mất 90 phút rà soát thủ công bằng mắt và chỉnh sửa từng ô dữ liệu chứa lỗi sai định dạng tinh vi mà công cụ Excel cơ bản bỏ sót. |
| Impact (nếu không giải thì sao) | Tỷ lệ email gửi đi bị trả về (bounce rate) vượt ngưỡng an toàn (>5%), hệ thống gửi thư bị khóa tài khoản; dữ liệu khách hàng bị phân mảnh, gây phiền hà cho khách hàng và làm giảm uy tín doanh nghiệp. |
| Success metric (baseline → target) | - Thời gian làm sạch tập 500 bản ghi: từ 120 phút giảm xuống dưới 20 phút. Tỷ lệ bản ghi bị lỗi định dạng khi nạp vào hệ thống: giảm từ 8% xuống dưới 0.5%. |
| Phương án không dùng AI | Xây dựng pipeline kiểm tra chất lượng dữ liệu bằng script Python/SQL với các biểu thức chính quy (Regex) nghiêm ngặt; đồng thời cấu hình validation ngay tại form nhập liệu đầu vào của CRM. |
| Giả thuyết về AI (nếu có) | Sử dụng Rule-based kết hợp mô hình phân tích chuỗi văn bản nhỏ để tự động chuẩn hóa định dạng địa chỉ, nhận diện tên riêng và phát hiện các trường dữ liệu bị đảo lộn vị trí. |
| Cảm nhận nhanh | Rule |

Quy trình nháp hiện tại:

```text
[Xuất file CSV/Excel thô từ CRM] (10')
[Chạy lọc trùng cơ bản trong Excel] (10')
[RÀ SOÁT LỖI FONT, SỐ ĐT, EMAIL BẰNG MẮT] (60') <--- [BOTTLENECK CHÍNH]
[SỬA THỦ CÔNG TỪNG Ô LỖI TRONG FILE] (30') <--- [BOTTLENECK PHỤ]
[Chạy gửi kiểm tra thử nghiệm] (10')
Tổng thời gian: 120 phút
```

---

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi kết thúc cuộc họp điều hành hoặc thảo luận giải pháp với khách hàng/đối tác, tôi muốn trích xuất chính xác các quyết định đã thống nhất và đầu việc được giao kèm người chịu trách nhiệm, để gửi email xác nhận biên bản họp (meeting recap) trong ngày. |
| Actor | Quản lý dự án (Project Manager) / Thư ký cuộc họp. |
| Thời điểm / bối cảnh | Ngay sau các cuộc họp định kỳ tuần hoặc họp bàn giao giải pháp với khách hàng (2–3 lần/tuần). |
| Quy trình hiện tại (3–7 bước) | 1. Mở bản ghi chú nháp trong lúc họp và mở file ghi âm cuộc họp (5 phút). Nghe tua lại các đoạn thảo luận kéo dài để xác nhận lại chi tiết cam kết (40 phút). Tổng hợp danh sách đầu việc: mô tả việc, người phụ trách, thời hạn bàn giao (25 phút). Soạn thảo email biên bản cuộc họp theo mẫu chuẩn của công ty (15 phút). Gửi email cho các bên tham gia để xác nhận đồng thuận (5 phút). |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2 & Bước 3: Mất 65 phút nghe tua lại các đoạn thảo luận rối rắm để lọc ra đúng nội dung chốt cam kết và phân loại việc theo từng người. |
| Impact (nếu không giải thì sao) | Biên bản họp bị gửi trễ (sang ngày hôm sau); dễ bỏ sót các cam kết phát sinh trong trao đổi, dẫn đến xung đột trách nhiệm giữa các phòng ban khi dự án gặp sự cố. |
| Success metric (baseline → target) | - Thời gian hoàn thành và gửi biên bản họp: từ 90 phút giảm xuống dưới 20 phút sau khi cuộc họp kết thúc. Tỷ lệ phản hồi yêu cầu đính chính biên bản do ghi nhận sai người/việc: giảm từ 20% xuống dưới 5%. |
| Phương án không dùng AI | Áp dụng kỷ luật cuộc họp: yêu cầu người chủ trì dành 5 phút cuối buổi để chốt miệng và ghi trực tiếp các Action Items lên màn hình chia sẻ chung để mọi người cùng duyệt ngay tại chỗ. |
| Giả thuyết về AI (nếu có) | AI (Workflow) xử lý transcript cuộc họp, tự động bóc tách các câu mang tính cam kết hành động dựa trên cấu trúc nhận diện thực thể và ngữ cảnh, sinh bản nháp Action Items kèm người phụ trách để thư ký duyệt nhanh. |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
[Mở ghi chú nháp & file ghi âm] (5')
[NGHE TUA LẠI ĐOẠN CAM KẾT PHỨC TẠP] (40') <--- [BOTTLENECK CHÍNH]
[TỔNG HỢP DANH SÁCH VIỆC & DEADLINE] (25') <--- [BOTTLENECK PHỤ]
[Soạn thảo email biên bản họp] (15')
[Gửi email xác nhận cho các bên] (5')
Tổng thời gian: 90 phút
```

---

### Card muốn pitch nhất

- Card số: **Card #1** (Bóc tách và lập bảng so sánh đối chuẩn tính năng/chi phí từ tài liệu kỹ thuật của đối thủ hoặc nhà cung cấp).
- Vì sao: Đây là bài toán có thời gian lãng phí lớn nhất (hơn 3.5 tiếng mỗi lần), ảnh hưởng trực tiếp đến hiệu quả kinh doanh và chiến lược sản phẩm của công ty, đồng thời có ranh giới đầu vào/đầu ra rõ ràng rất phù hợp để chuẩn hóa quy trình Workflow.
- Câu hỏi muốn nhóm phản biện: *"Nếu các tài liệu kỹ thuật có cách dùng thuật ngữ chuyên môn khác nhau hoặc cấu trúc bảng giá phức tạp (ví dụ một bên tính giá theo lượt gọi API, một bên tính trọn gói theo người dùng), quy trình của chúng ta sẽ xử lý việc quy đổi này thế nào để bảng so sánh đảm bảo tính khách quan và chính xác?"*

---

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| AI nhận xét rằng ở Card #1, bottleneck "mất thời gian bóc tách" chưa nêu rõ mất bao nhiêu phút và chỉ số metric "giúp ra quyết định nhanh hơn" là cảm tính, không đo lường được. | Đồng ý | Đã bóc tách cụ thể thời gian bước bóc tách (90 phút) và đối chiếu chéo (45 phút). Sửa metric thành chỉ số định lượng rõ ràng: giảm thời gian từ 210 phút xuống dưới 45 phút và độ chính xác dữ liệu bóc tách đạt 90% |
| AI cho rằng ở Card #2, việc sử dụng AI để làm sạch dữ liệu bảng tính định dạng đơn giản là lãng phí tài nguyên vì SQL/Regex và cấu hình validation ở cổng CRM hoàn toàn xử lý được hầu hết lỗi. | Đồng ý | Đã bổ sung chi tiết phương án không dùng AI (tập luật Regex + form validation ở CRM) và hạ mức can thiệp nhận định nhanh xuống **Rule** thay vì Workflow hay Agent. |
| AI chỉ ra ở Card #3, việc bóc tách Action Items tự động rất dễ mắc lỗi ảo giác (hallucination) do văn phong nói chuyện trong cuộc họp thường không có cấu trúc cố định, tiềm ẩn rủi ro gán nhầm trách nhiệm. | Đồng ý | Đã xác định rõ phương án không dùng AI (áp dụng kỷ luật chốt việc 5 phút cuối buổi họp), đồng thời giới hạn ranh giới AI chỉ sinh bản nháp gợi ý và bắt buộc có con người (Human-in-the-loop) duyệt trước khi gửi. |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Pitch Card #1 (Bóc tách & benchmarking tài liệu kỹ thuật/báo cáo đối thủ) và giới thiệu 2 card còn lại. | Card #1 được đưa vào shortlist 3 bài toán chung cuộc của nhóm để chấm điểm. |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt cho Trương Việt Công: *"Nếu khách hàng chụp ảnh mờ, mất góc hoặc gửi file qua Zalo không đúng mẫu, hệ thống nhận diện thế nào để không báo sai?"* | Công và Duy nhận ra điểm nghẽn thực sự của việc khách phải bổ sung nhiều lần nằm ở chất lượng ảnh đầu vào, từ đó nhóm bổ sung bước tiền kiểm tra chất lượng file (Quality Pre-check). |
| Nhận phản biện | Câu hỏi tôi nhận được từ Đoàn Văn Tú: *"Nếu tài liệu dùng thuật ngữ khác nhau hoặc cấu trúc giá dị biệt (API call vs user/tháng), hệ thống chuẩn hóa thế nào để số liệu không bị méo?"* | Tôi sửa lại: nếu làm bài toán benchmarking này thì cần thêm bước chuẩn hóa quy đổi đơn vị đo lường trước khi đưa vào bảng so sánh. |
| Gom cluster / cây OST | Rà soát 15 candidate của cả nhóm, phân tích pattern chung và gom thành 4 Cluster (A, B, C, D); dựng cây OST rút gọn. | Nhóm có một cây OST chuẩn: xác định đúng 1 Outcome chung (giảm 50% thời gian sơ duyệt), tách bạch rõ 3 Opportunity cốt lõi và gạch bỏ triệt để 3 solution trá hình (Agent duyệt tự động, portal khách hàng, tool spam email). |
| Chọn candidate problem | Xây dựng bảng chấm điểm shortlist 7 tiêu chí (1–5) cho 3 bài toán; chủ trì phiên thảo luận và giải trình lý do loại 2 bài toán còn lại. | Nhóm thống nhất 100% chọn cụm bài toán Kiểm tra tính đầy đủ và nhất quán hồ sơ vay (#7 & #8) với 34 điểm; tôi chủ động nhường bài toán #1 của mình vì bài tín dụng có impact rộng hơn. |
| Kiểm chứng / research | Cùng Duy và Công thảo luận bảng câu hỏi Mom Test; rà soát tính năng bóc tách văn bản của FPT.AI Reader và Azure Document Intelligence. | Nhóm nhận ra công cụ thị trường chỉ đọc từng file rời rạc, chưa có tính năng đối chiếu chéo (Cross-matching) giữa các giấy tờ trong cùng một bộ hồ sơ. |
| Quy trình nhóm | Đóng góp ý kiến về việc thiết kế điểm nút Human-in-the-loop (HITL) tại bước 4 của quy trình tương lai. | Quy trình nhóm có chốt chặn an toàn: nhân viên bắt buộc phải duyệt trên màn hình đối chiếu trước khi phát hành danh sách giấy tờ thiếu cho khách. |
| Problem Statement | Phản biện bản v0 về việc thiếu Success Metric chất lượng bóc tách. | Nhóm bổ sung thêm chỉ số đo lường tỷ lệ nhân viên phải gõ sửa tay lại $\le 10\%$ vào bản v1. |
| Mức can thiệp AI | Thảo luận và thống nhất đặt bài toán vào ô Độ mơ hồ Thấp — Độ phức tạp Cao trong ma trận. | Nhóm không bị sa đà vào Agent mà chọn mức Workflow triển khai 2 giai đoạn (No AI/Rule trước, OCR sau). |
| Quyết định | Tham gia đánh giá 4 rủi ro và xác lập các ngưỡng dừng (Stop conditions) cho đợt pilot 2 tuần. | Nhóm có ngưỡng dừng định lượng: nếu tỷ lệ trích xuất sai trường quan trọng $> 20\%$ thì dừng pilot, quay về checklist cứng. |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Tìm thêm góc nhìn từ lăng kính "Cần đọc, tổng hợp nhiều thông tin". | Gợi ý ý tưởng phân tích tài liệu thị trường và đọc báo cáo doanh nghiệp dài. | Gợi ý bài toán chung chung kiểu "dùng AI tóm tắt tài liệu", không có ngữ cảnh công việc và dấu hiệu đo lường thật. | Tôi viết lại theo trải nghiệm thẩm định hồ sơ kỹ thuật/giải pháp thực tế: tài liệu 15–20 trang, tốn 3–4 tiếng, tần suất 2 đợt/quý. |
| CP2 Problem Card | Đóng vai PM hoài nghi để bóc tách lỗ hổng của 3 Problem Card. | Chỉ ra rất đúng việc metric "giúp ra quyết định nhanh hơn" ở Card #1 là định tính, không thể đo lường. | Gợi ý tôi làm Agent tự động crawl và tự động so sánh giá các bên (quá phức tạp và vi phạm tính khả thi). | Tôi giữ nguyên mức Workflow; sửa metric thành định lượng cụ thể: giảm từ 210' xuống dưới 45' và độ chính xác $\ge 90\%$. |
| CP4 Research | Tra cứu các giải pháp trích xuất dữ liệu tài liệu trên thị trường. | Liệt kê nhanh các dịch vụ OCR lớn như Google Document AI, Azure Form Recognizer, AWS Textract. | AI khẳng định các công cụ này có thể "tự động hóa toàn bộ quy trình thẩm định hồ sơ vay vốn". | Tôi vào trực tiếp trang tài liệu kỹ thuật của Azure/Google để kiểm chứng và đính chính: OCR chỉ bóc tách ký tự thô, không thể thay thế thẩm định nghiệp vụ tín dụng. |
| CP5 Quy trình | Nhờ AI chuyển đổi luồng quy trình hiện tại và tương lai sang mã Mermaid. | Sinh cấu trúc flowchart nhanh, hiển thị trực quan các nhánh rẽ và bước kiểm tra. | AI tự ý gộp bước "bóc tách OCR" và bước "đối chiếu chéo Rule" thành 1 khối AI duy nhất. | Tôi tách đôi 2 bước: AI chỉ phụ trách trích xuất thực thể ở bước 2, còn bước 3 so sánh dữ liệu với Core Banking hoàn toàn do Rule đảm nhiệm. |
| CP5–6 Problem Statement | Đặt prompt: "Chỉ ra 3 điểm mơ hồ nhất trong Problem Statement v0 của tôi, không viết lại thay". | Chỉ ra được v0 chưa có guardrail metric chống lỗi trích xuất sai và boundary chưa chặt. | Đề xuất thêm các tiêu chí mơ hồ như "người dùng cảm thấy hài lòng hơn". | Tôi tự viết tiêu chí eval định lượng: độ chính xác trường số đạt 100%, tỷ lệ sửa tay $\le 10\%$, cảnh báo sai lệch $\ge 95\%$. |
| CP6 Mức can thiệp / quyết định | So sánh sự khác biệt giữa Workflow và Agent trong xử lý tài liệu có cấu trúc. | Giúp làm rõ định nghĩa: Workflow là luồng định sẵn AI làm 1 bước, Agent là AI tự quyết bước tiếp theo. | Khuyên nhóm nên dùng Agentic Workflow để tự tương tác với khách hàng đòi nợ/bổ sung giấy tờ. | Tôi bác bỏ vì rủi ro pháp lý/tuân thủ quá lớn; kiên quyết cùng nhóm chốt mức Workflow bán tự động có con người duyệt (HITL). |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**  
Thấy nhân viên tín dụng tốn quá nhiều sức vào việc mở file ảnh và soi từng số CCCD.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**  
có nhưng đã loại bỏ

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**  
Có, Tú phản biện rằng bài toán benchmarking của tôi tần suất thấp và phạm vi hẹp. Nên tôi đã đổi ý.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**  
Bất ngờ: 100% người được hỏi từ chối để AI tự quyết.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**  
Khó nhất là Metric và Boundary.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**  

Nếu làm lại, tôi sẽ ưu tiên dùng OCR chuyên biệt để tối ưu tốc độ, chi phí và tránh bịa đặt thông tin.
**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.
1. **Problem:** Cán bộ tín dụng mất 35–45 phút mở file kiểm tra thủ công và đối chiếu Core Banking, khiến xử lý trễ và khách phải bổ sung nhiều đợt.
2. **Quy trình:** Tái cấu trúc thành 5 bước: tiếp nhận (Rule) - bóc tách trường - đối chiếu chéo (Rule)- cán bộ duyệt cảnh báo (HITL) - chuyển thẩm định.
3. **Metric:** Giảm thời gian từ 35–45 phút xuống 20–25 phút/hồ sơ, số lần bổ sung tối đa 1 lần, và 0% bỏ sót sai lệch.
4. **Boundary:** AI chỉ bóc tách và cảnh báo; không tự duyệt/từ chối vay, không tự nhắn khách và không sửa Core Banking.
5. **Mức can thiệp AI:** Chọn **Workflow bán tự động** (No AI + Rule ở giai đoạn 1, tích hợp AI OCR ở giai đoạn 2 có con người giám sát), từ chối Agent.
6. **Quyết định:** Chốt **Go, phạm vi nhỏ** thử nghiệm pilot 2 tuần trên 50 bộ hồ sơ ẩn danh; nếu lỗi trích xuất trường chính vượt 20% thì dừng ngay để quay về checklist chuẩn.

---

## 7. Tài liệu tham khảo

* Marty Cagan, *Inspired: How to Create Tech Products Customers Love* (Mô hình đánh giá 4 rủi ro sản phẩm).
* Teresa Torres, *Continuous Discovery Habits* (Phương pháp luận xây dựng Opportunity Solution Tree).
* Rob Fitzpatrick, *The Mom Test* (Kỹ thuật phỏng vấn kiểm chứng hành vi khách hàng trong quá khứ).
* Google PAIR (People + AI Research): *Human-AI Interaction Design Guidelines*.
* Tài liệu kỹ thuật Microsoft Azure AI Document Intelligence & FPT.AI Reader.
-
