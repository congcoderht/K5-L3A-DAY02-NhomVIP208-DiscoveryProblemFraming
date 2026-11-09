# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Trường Duy
- MSSV: 2A202603589
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: NhomVIP208
- Link repo nhóm: https://github.com/congcoderht/K5-L3A-DAY02-NhomVIP208-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi tiếp nhận hồ sơ vay vốn mới, tôi muốn tự động tổng hợp thông tin khách hàng từ Core Banking, để không phải tra cứu và nhập lại những dữ liệu đã có trên hệ thống. | Credit Officer, bộ phận vận hành tín dụng | Mỗi hồ sơ mất khoảng 10–15 phút để tra cứu và nhập lại thông tin. |
| 2 | Tốn thời gian | Khi nhận bộ hồ sơ vay gồm CCCD, sao kê lương, hợp đồng lao động và giấy tờ tài sản, tôi muốn nhanh chóng kiểm tra tính đầy đủ và hợp lệ của tài liệu, để giảm thời gian rà soát thủ công. | Credit Officer, khách hàng | Mất khoảng 20–30 phút/hồ sơ để mở từng file, kiểm tra và đối chiếu danh mục giấy tờ. |
| 3 | Cần đọc, tổng hợp nhiều thông tin | Khi đối chiếu thông tin khách hàng giữa đơn đề nghị vay, giấy tờ tùy thân và Core Banking, tôi muốn tự động phát hiện những thông tin không nhất quán, để tránh đưa dữ liệu sai vào báo cáo thẩm định. | Credit Officer, bộ phận quản lý rủi ro, cấp phê duyệt | Có nguy cơ bỏ sót sai lệch về họ tên, số CCCD, thu nhập hoặc thông tin khoản vay khi kiểm tra thủ công. |
| 4 | Cần đọc, tổng hợp nhiều thông tin | Khi đánh giá khả năng trả nợ của khách hàng, tôi muốn tập hợp thông tin về thu nhập, lịch sử tín dụng, dư nợ hiện tại và nghĩa vụ tài chính từ các nguồn liên quan, để có đủ cơ sở đánh giá rủi ro khoản vay. | Credit Officer, bộ phận quản lý rủi ro, cấp phê duyệt | Phải chuyển đổi giữa Core Banking, hệ thống quản lý tài liệu và các nguồn thông tin nội bộ; mất khoảng 30–45 phút/hồ sơ để tổng hợp. |
| 5 | Tốn thời gian | Khi hoàn tất thẩm định hồ sơ vay vốn, tôi muốn tự động tạo bản dự thảo báo cáo thẩm định theo cấu trúc chuẩn từ dữ liệu đã thu thập, để rút ngắn thời gian lập báo cáo và chuyển cấp có thẩm quyền phê duyệt đúng hạn. | Credit Officer, cấp phê duyệt, khách hàng | Mất khoảng 30–60 phút để tổng hợp dữ liệu, viết nhận xét, đánh giá rủi ro và định dạng báo cáo. |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

-

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Kiểm tra tính đầy đủ và hợp lệ của hồ sơ vay | Quy trình rõ ràng, lặp lại với hầu hết hồ sơ, tốn thời gian kiểm tra thủ công. Có thể ứng dụng AI/OCR để trích xuất và đối chiếu tài liệu. | AI nhận diện tài liệu không chính xác đến mức nào? Làm thế nào xử lý tài liệu mờ, thiếu hoặc sai định dạng? |
| 2 | Phát hiện thông tin không nhất quán | Sai lệch thông tin giữa CCCD, đơn vay, sao kê và Core Banking có thể ảnh hưởng trực tiếp đến độ chính xác của báo cáo thẩm định. Có thể xây dựng quy tắc đối chiếu và AI hỗ trợ phát hiện bất thường. | Tỷ lệ phát hiện sai lệch và tỷ lệ cảnh báo nhầm là bao nhiêu? Cần xác định những trường dữ liệu nào được ưu tiên đối chiếu. |
| 3 | Tự động tạo báo cáo thẩm định | Báo cáo có cấu trúc tương đối chuẩn, yêu cầu tổng hợp nhiều nguồn dữ liệu và viết nhận xét. Có tiềm năng tiết kiệm thời gian, giảm thao tác lặp lại và tăng tính nhất quán. | Nội dung do AI tạo ra có chính xác, đầy đủ và tuân thủ biểu mẫu ngân hàng không? Ai chịu trách nhiệm kiểm tra và phê duyệt nội dung? |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi tiếp nhận một bộ hồ sơ vay vốn cá nhân, tôi muốn nhanh chóng kiểm tra tính đầy đủ và hợp lệ của các tài liệu, để đảm bảo hồ sơ đáp ứng yêu cầu trước khi tiến hành thẩm định. |
| Actor | Credit Officer trực tiếp tiếp nhận và kiểm tra hồ sơ vay vốn cá nhân. |
| Thời điểm / bối cảnh | Khi khách hàng nộp hồ sơ vay vốn trực tiếp hoặc khi nhân viên tiếp nhận hồ sơ được chuyển đến từ bộ phận kinh doanh. |
| Quy trình hiện tại (3–7 bước) | 1. Tiếp nhận bộ hồ sơ từ khách hàng · 2. Truy cập hệ thống quản lý tài liệu · 3. Mở từng tài liệu như CCCD, sao kê lương, hợp đồng lao động · 4. Kiểm tra danh mục giấy tờ theo yêu cầu khoản vay · 5. Kiểm tra chất lượng và tính hợp lệ của từng tài liệu · 6. Ghi nhận giấy tờ còn thiếu hoặc không hợp lệ · 7. Gửi yêu cầu bổ sung hồ sơ nếu cần. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3–5: Phải mở và kiểm tra từng tài liệu riêng lẻ, mất thời gian khi hồ sơ có nhiều giấy tờ hoặc tài liệu không được sắp xếp thống nhất. |
| Impact (nếu không giải thì sao) | Giả định mất 20–30 phút/hồ sơ. Với 8 hồ sơ/ngày, Phương có thể dành khoảng 160–240 phút/ngày cho việc kiểm tra tài liệu. |
| Success metric (baseline → target) | Thời gian kiểm tra hồ sơ giảm ít nhất 50%; tỷ lệ phát hiện chính xác giấy tờ thiếu hoặc không hợp lệ đạt từ 95%; không làm tăng tỷ lệ bỏ sót tài liệu. |
| Phương án không dùng AI | Xây dựng checklist hồ sơ theo từng loại khoản vay, chuẩn hóa tên file và sử dụng biểu mẫu kiểm tra tài liệu. |
| Giả thuyết về AI (nếu có) | AI kết hợp OCR và xử lý tài liệu để tự động nhận diện loại giấy tờ, trích xuất thông tin cơ bản, kiểm tra danh mục hồ sơ và cảnh báo tài liệu thiếu, mờ hoặc hết hạn. Credit Officer xác nhận kết quả trước khi chuyển bước tiếp theo. |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 75 phút

[1 Tiếp nhận hồ sơ: 5'] → [2 Truy cập hệ thống: 5'] → [3 Mở từng tài liệu: 10']
→ [4 Kiểm tra danh mục: 10'] → [5 Kiểm tra tính hợp lệ: 30'] ← BOTTLENECK
→ [6 Ghi nhận thiếu/lỗi: 10'] → [7 Yêu cầu bổ sung: 5']
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi thẩm định hồ sơ vay vốn, tôi muốn nhanh chóng phát hiện những thông tin không nhất quán giữa các tài liệu và dữ liệu Core Banking, để hạn chế sai sót trong quá trình đánh giá khách hàng và khoản vay. |
| Actor | Credit Officer chịu trách nhiệm kiểm tra, đối chiếu và xác minh thông tin khách hàng. |
| Thời điểm / bối cảnh | Sau khi hồ sơ đã được kiểm tra tính đầy đủ, trước khi nhân viên thực hiện đánh giá tài chính và lập báo cáo thẩm định. |
| Quy trình hiện tại (3–7 bước) | 1. Mở đơn đề nghị vay vốn · 2. Kiểm tra thông tin CCCD · 3. Mở sao kê lương và hợp đồng lao động · 4. Truy cập Core Banking để kiểm tra thông tin khách hàng · 5. Đối chiếu họ tên, số CCCD, ngày sinh, thu nhập và thông tin khoản vay · 6. Ghi nhận các điểm không khớp · 7. Xác minh lại thông tin với khách hàng hoặc bộ phận liên quan. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 5: Phải đối chiếu thủ công giữa nhiều tài liệu và hệ thống khác nhau. Những sai lệch nhỏ có thể bị bỏ sót khi số lượng hồ sơ lớn. |
| Impact (nếu không giải thì sao) | Giả định mất 15–25 phút/hồ sơ để đối chiếu. Sai lệch không được phát hiện có thể dẫn đến đánh giá sai khả năng trả nợ hoặc phải thực hiện lại quy trình thẩm định. |
| Success metric (baseline → target) | Thời gian đối chiếu giảm ít nhất 50%; tỷ lệ phát hiện sai lệch quan trọng đạt từ 95%; tỷ lệ cảnh báo sai dưới 5%. |
| Phương án không dùng AI | Sử dụng biểu mẫu đối chiếu thông tin thống nhất, quy tắc kiểm tra dữ liệu và checklist xác minh giữa các nguồn. |
| Giả thuyết về AI (nếu có) | AI kết hợp OCR và cơ chế đối chiếu dữ liệu để tự động trích xuất thông tin từ tài liệu, so sánh với Core Banking, phát hiện trường dữ liệu không khớp và đưa ra cảnh báo kèm nguồn tham chiếu. |
| Cảm nhận nhanh | Rule |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 60 phút

[1 Mở đơn đề nghị vay: 2'] → [2 Kiểm tra CCCD: 3'] → [3 Mở sao kê & HĐLĐ: 5']
→ [4 Truy cập Core Banking: 5'] → [5 Đối chiếu thông tin: 20'] ← BOTTLENECK
→ [6 Ghi nhận sai lệch: 10'] → [7 Xác minh lại: 15']

```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi hoàn tất quá trình thẩm định hồ sơ vay vốn, tôi muốn tự động tổng hợp thông tin và tạo bản dự thảo báo cáo thẩm định theo biểu mẫu chuẩn, để tiết kiệm thời gian lập báo cáo và chuyển cấp có thẩm quyền phê duyệt. |
| Actor | Credit Officer chịu trách nhiệm phân tích hồ sơ, đưa ra nhận xét và lập báo cáo thẩm định trình cấp phê duyệt. |
| Thời điểm / bối cảnh | Sau khi hoàn tất kiểm tra hồ sơ, đối chiếu thông tin khách hàng và đánh giá tình hình tài chính, trước khi chuyển hồ sơ lên cấp có thẩm quyền phê duyệt. |
| Quy trình hiện tại (3–7 bước) | 1. Truy cập Core Banking để lấy thông tin khoản vay · 2. Mở hệ thống quản lý tài liệu để xem lại hồ sơ khách hàng · 3. Tổng hợp thông tin cá nhân, thu nhập và nghĩa vụ tài chính · 4. Đánh giá khả năng trả nợ và mức độ rủi ro · 5. Mở biểu mẫu báo cáo thẩm định · 6. Nhập thông tin và viết nhận xét đánh giá · 7. Kiểm tra nội dung, định dạng báo cáo. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 5–6: Phải tổng hợp thông tin từ nhiều nguồn và tự viết nội dung nhận xét, đánh giá theo biểu mẫu. Đây là công đoạn tốn thời gian và đòi hỏi khả năng phân tích nghiệp vụ. |
| Impact (nếu không giải thì sao) | Giả định mất 30–60 phút/hồ sơ để tổng hợp dữ liệu và lập báo cáo. Với 8 hồ sơ/ngày, thời gian có thể lên đến 4–8 giờ/ngày. |
| Success metric (baseline → target) | Thời gian lập báo cáo giảm ít nhất 50%; 100% trường thông tin bắt buộc được điền đầy đủ; không xuất hiện thông tin sai lệch so với dữ liệu nguồn; báo cáo được Credit Officer kiểm tra trước khi trình phê duyệt. |
| Phương án không dùng AI | Sử dụng biểu mẫu báo cáo chuẩn, tích hợp dữ liệu từ Core Banking vào mẫu báo cáo và xây dựng thư viện nhận xét theo từng trường hợp thẩm định. |
| Giả thuyết về AI (nếu có) | AI thu thập và tổng hợp dữ liệu từ các nguồn được cấp quyền, phân tích thông tin tài chính theo tiêu chí nghiệp vụ, tạo bản dự thảo báo cáo thẩm định và đề xuất nhận xét. Credit Officer kiểm tra, chỉnh sửa và xác nhận trước khi trình cấp phê duyệt. |
| Cảm nhận nhanh | Agent |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 90 phút

[1 Lấy TT Core Banking: 5'] → [2 Xem lại hồ sơ: 10'] → [3 Tổng hợp thông tin: 15']
→ [4 Đánh giá rủi ro: 20'] → [5 Mở biểu mẫu báo cáo: 5'] 
→ [6 Viết nhận xét đánh giá: 25'] ← BOTTLENECK
→ [7 Review & định dạng: 10']

```

### Card muốn pitch nhất

- Card số: 1
- Vì sao: 
  - Quy trình rõ ràng, lặp lại với hầu hết hồ sơ, tốn thời gian kiểm tra thủ công.
  - Có thể ứng dụng AI/OCR để trích xuất và đối chiếu tài liệu.
  - Nếu giải quyết được vấn đề này, sẽ giảm đáng kể thời gian kiểm tra hồ sơ, tăng hiệu quả công việc và giảm sai sót.
- Câu hỏi muốn nhóm phản biện: 
  - AI có thể nhận diện và trích xuất thông tin từ các loại giấy tờ khác nhau với độ chính xác cao không?
  - Làm thế nào để xử lý các trường hợp tài liệu mờ, thiếu hoặc sai định dạng?
  - Có cần xây dựng cơ chế kiểm tra và xác nhận kết quả của AI trước khi chuyển bước tiếp theo không?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Problem đang gộp nhiều phạm vi như nhận diện tài liệu, kiểm tra tính đầy đủ, xác minh tính hợp lệ và phát hiện giấy tờ giả. | Đồng ý | Thu hẹp MVP vào nhận diện loại giấy tờ, kiểm tra danh mục bắt buộc và cảnh báo tài liệu thiếu hoặc không đọc được. Không đặt mục tiêu xác minh giấy tờ thật hay giả. |
| Tối ưu tốc độ không được làm giảm tính chính xác và các bước kiểm soát trong quy trình tín dụng. | Đồng ý | Giới hạn AI ở vai trò hỗ trợ kiểm tra và cảnh báo; không tự quyết định hồ sơ đạt yêu cầu, không thay thế kiểm soát nghiệp vụ và quyết định tín dụng của ngân hàng. |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Trình bày Problem Card về kiểm tra tính đầy đủ và hợp lệ của hồ sơ vay, giải thích bottleneck là bước mở và kiểm tra thủ công nhiều tài liệu | Giúp nhóm thấy đây là vấn đề có quy trình rõ, lặp lại và có thể đo thời gian xử lý. |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: Nếu khách hàng nộp đủ nhưng ảnh mờ, cắt góc, hoặc sai định dạng thì sao? Việc cảnh báo thiếu có thực sự giải quyết được việc "bổ sung nhiều lần" nếu chất lượng giấy tờ không được kiểm soát ngay từ đầu? | Nhóm bổ sung bước kiểm tra chất lượng tài liệu ngay khi tiếp nhận. Hồ sơ bị mờ, cắt góc hoặc không đọc được phải được cảnh báo và yêu cầu xử lý trước khi chuyển sang bước thẩm định. |
| Nhận phản biện | Câu hỏi tôi nhận được: Phần nào trong việc lập báo cáo hiện mất nhiều thời gian nhất, và có mẫu hoặc quy tắc sẵn có nào giúp giảm công việc mà vẫn bảo đảm người có thẩm quyền kiểm tra được? | Tôi đã sửa gì: |
| Gom cluster / cây OST | Đề xuất gom các vấn đề liên quan đến kiểm tra hồ sơ, đối chiếu dữ liệu và tổng hợp báo cáo thành các nhóm nhu cầu riêng. | Giúp nhóm nhìn được mối quan hệ giữa opportunity, bottleneck và outcome. |
| Chọn candidate problem | Tham gia so sánh các candidate theo mức độ ảnh hưởng, tần suất, khả năng đo lường và tính phù hợp với phạm vi bài. | mức độ ảnh hưởng, tần suất, khả năng đo lường và tính phù hợp với phạm vi bài.	Nhóm thống nhất ưu tiên vấn đề kiểm tra tính đầy đủ và hợp lệ của hồ sơ vay. |
| Kiểm chứng / research | Làm việc với Linh và Công xây dựng, rà soát bộ câu hỏi theo phương pháp Mom Test; đồng thời khảo sát khả năng trích xuất văn bản của FPT.AI Reader và Azure Document Intelligence. | Nhóm nhận thấy các công cụ này chủ yếu hỗ trợ đọc và bóc tách dữ liệu từ từng tài liệu riêng lẻ, trong khi bài toán của nhóm còn cần đối chiếu chéo thông tin giữa nhiều giấy tờ trong cùng một bộ hồ sơ. |
| Quy trình nhóm | Góp ý làm rõ quy trình từ tiếp nhận hồ sơ, kiểm tra từng tài liệu, đối chiếu với Core Banking, yêu cầu bổ sung đến chuyển thẩm định | Nhóm xác định bottleneck chính là mở nhiều file, nhập và đối chiếu thủ công, khiến hồ sơ phải bổ sung nhiều lần; thời gian hiện tại ước tính 35–45 phút/hồ sơ. |
| Problem Statement | Góp phần làm rõ acotr là nhân viên tiếp nhận/Credit Officer, bottleneck là kiểm tra và đối chiểu thủ công, cùng tác động đến thời gian và rủi ro bỏ sót. | Problem Statement được cụ thể hóa bằng baseline 35–45 phút/hồ sơ, mục tiêu còn tối đa 20–25 phút, số lần bổ sung không quá một lần và có bước HITL bắt buộc. |
| Mức can thiệp AI | Xác định cùng các thành viên và quyết định bài toàn vào mức Độ mơ hồ Thấp và đặt Độ phức tạp Cao | Nhóm chọn mức Workflow để triển khai |
| Quyết định | Định hướng nhóm không để AI tự duyệt, tự từ chối hoặc tự duyệt hồ sơ vay mà phải chuyển sự quyết định sang con người | Nhóm xác định rõ boundary và cơ chế HITL: AI chỉ hỗ trợ một bước trong Workflow, còn quyết định nghiệp vụ vẫn thuộc về con người. Điều này giúp giảm rủi ro bỏ sót, automation bias và vi phạm tuân thủ. |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Gợi ý thêm vấn đề theo các kênh lặp lại, tốn thời gian và cần tổng hợp nhiều thông tin. | Giúp mở rộng góc nhìn và chuyển ý tưởng thành Job Story có actor, bối cảnh và kết quả mong muốn. | Một số gợi ý còn chung chung, dễ chuyển sang giải pháp như “dùng AI để tự động hóa”. | Em giữ các vấn đề gắn với quy trình hồ sơ vay và bổ sung thời gian xử lý dựa trên bối cảnh thực tế. |
| CP2 Problem Card | Nhờ AI phản biện actor, bottleneck, impact, metric và khả năng giải quyết bằng No AI/Rule/Workflow/Agent. | Giúp phát hiện phạm vi quá rộng và các câu hỏi cần làm rõ, đặc biệt về chất lượng tài liệu và trách nhiệm khi AI sai. | AI có xu hướng mặc định OCR hoặc AI là giải pháp, chưa phân biệt rõ kiểm tra tính đầy đủ với xác minh giấy tờ thật. | Tôi thu hẹp bài toán về kiểm tra tính đầy đủ, chất lượng và tính nhất quán của hồ sơ; không đưa xác minh giả mạo vào MVP. |
| CP4 Research | Hỗ trợ lập câu hỏi Mom Test và gợi ý các công cụ OCR/document intelligence để nghiên cứu. | Giúp nhóm có khung câu hỏi và nhanh chóng so sánh các khả năng như đọc văn bản, nhận diện trường dữ liệu và xử lý biểu mẫu. | AI có thể mô tả tính năng công cụ quá chung hoặc suy diễn rằng OCR có thể xác nhận hồ sơ hợp lệ. | Tôi rà soát lại nguồn chính thức và kết luận rằng OCR chỉ hỗ trợ trích xuất; việc đối chiếu chéo và quyết định nghiệp vụ vẫn cần Rule và con người. |
| CP5 Quy trình | Chuyển mô tả quy trình hiện tại thành các bước có actor, input, output, thời gian và bottleneck. | Giúp trình bày rõ quy trình trước/sau và nhận diện các điểm có thể dùng Rule, AI hoặc HITL. | AI dễ gộp các bước kiểm tra khác nhau thành một bước hoặc bỏ qua vòng lặp yêu cầu bổ sung. | Tôi tách riêng bước kiểm tra chất lượng tài liệu, đối chiếu Core Banking, yêu cầu bổ sung và xác nhận chuyển thẩm định. |
| CP5–6 Problem Statement | Nhờ AI rà soát actor, bottleneck, impact, metric và boundary của Problem Statement. | Giúp phát hiện chỗ còn mơ hồ và gợi ý cách viết baseline, target, guardrail metric rõ hơn. | AI thường đề xuất mục tiêu lý tưởng hoặc viết như thể giải pháp đã chắc chắn khả thi. | Tôi giữ các số liệu ở mức ước tính, ghi rõ cách đo bằng hồ sơ giả lập và bổ sung boundary: AI không tự duyệt, từ chối hay sửa dữ liệu. |
| CP6 Mức can thiệp / quyết định | Dùng AI để so sánh No AI, Rule, Workflow và Agent, đồng thời phân tích rủi ro của từng mức. | Giúp nhóm thấy quy trình có thể bắt đầu bằng Checklist + Rule, sau đó mới thêm OCR nếu cần. | AI dễ đề xuất Agent hoặc tự động hóa quá nhiều, chưa đủ chú ý đến bảo mật và trách nhiệm trong nghiệp vụ tín dụng. | Tôi thống nhất hướng Workflow có HITL: AI chỉ OCR/trích xuất ở một bước, Rule xử lý đối chiếu, Credit Officer kiểm tra và quyết định; quyết định triển khai cần chờ kiểm chứng thêm. |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**
Em học được rằng cùng một pain có thể xuất hiện nhiều góc nhìn khác nhau. Các bạn giúp em thấy cần kiểm tra actor, bottleneck và bằng chứng trước khi nghĩ đến giải pháp.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**
Có. Nhón từng nhanh chóng nghĩ đến OCR, AI Agent và chatbot. Sau khi lập cây OST và so sánh No AI/Rule/Workflow/Agent, nhóm quay lại xác định pain trước và nhận ra Checklist + Rule có thể giải quyết một phần vấn đề.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**
Có. Khi được hỏi phần nào trong báo cáo tốn nhiều thời gian nhất và liệu mẫu/quy tắc sẵn có đã đủ hay chưa, em nhận ra không nên mặc định dùng AI để viết toàn bộ báo cáo. Cần ưu tiên chuẩn hóa biểu mẫu, Rule và giữ bước kiểm tra của người có thẩm quyền.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**
Điều bất ngờ nhất là khoảng cách giữa việc AI trích xuất đúng chữ và việc giải quyết bài toán nghiệp vụ. Azure Document Intelligence hay AWS Textract có thể đọc CCCD, hợp đồng hoặc sao kê, nhưng không thể tự xác minh giấy tờ giả, tính hợp pháp của con dấu hay điều kiện vay. AI chỉ nên hỗ trợ đọc dữ liệu; trách nhiệm pháp lý, kiểm soát rủi ro và quyết định tín dụng vẫn thuộc về con người. Ngoài ra, yêu cầu bảo mật dữ liệu ngân hàng khiến việc sử dụng dịch vụ đám mây công cộng bị giới hạn nghiêm ngặt.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**
Khó nhất là viết vấn đề đủ cụ thể nhưng không lẫn vào giải pháp. Em phải phân biệt rõ bottleneck hiện tại, tác động đo được và boundary của bài toán.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**
Nếu làm lại, em sẽ kiểm chúng với người dùng sớm và phản biện mạnh hơn về số liệu thời gian, tấn suất hồ sơ thiếu và khả năng dugnf Checklist/Rule trước khi nghĩ đến AI.

**6.7. Hiểu bài: giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.**
Quy trình hiện tại yêu cầu nhân viên mở từng tài liệu, kiểm tra checklist, đối chiếu với Core Banking và yêu cầu bổ sung khi phát hiện thiếu sót. Quy trình này mất khoảng 35–45 phút mỗi hồ sơ và có thể khiến khách hàng phải bổ sung nhiều lần. AI không được tự duyệt, từ chối khoản vay, sửa dữ liệu hay gửi yêu cầu cho khách hàng. Nhóm chọn Workflow, trong đó Rule xử lý checklist và đối chiếu, còn AI chỉ hỗ trợ OCR/trích xuất dữ liệu từ ảnh hoặc bản scan. Credit Officer vẫn phải kiểm tra và xác nhận kết quả trước khi chuyển hồ sơ sang thẩm định. Quyết định hiện tại nên là Not Yet cho đến khi nhóm hoàn tất kiểm chứng với người dùng và đánh giá bốn rủi ro chính.

---

## 7. Tài liệu tham khảo
- Hướng dẫn thực hành và bài mẫu môn học (docs/01-worksheet.md, docs/02-deliverable-example.md).
- Báo cáo tổng hợp nhóm NhomVIP208 (report/group_report.md).
- Tài liệu kỹ thuật: Microsoft Azure Document Intelligence, Google Document AI, AWS Textract.
- Khung phương pháp: Google PAIR Guidebook (Thiết kế AI lấy con người làm trung tâm) và Opportunity Solution Tree (Teresa Torres).
-
