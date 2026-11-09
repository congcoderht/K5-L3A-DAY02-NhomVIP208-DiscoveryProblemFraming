# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: NhomVIP208
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Nhân viên khó phát hiện sớm giấy tờ còn thiếu, tài liệu không đọc được hoặc sai lệch cần xác minh trước khi chuyển hồ sơ vay cá nhân sang thẩm định.
- Quyết định cuối: Not Yet — cần kiểm chứng nhu cầu, quy trình và điều kiện dữ liệu trước khi thử nghiệm OCR.

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
| -- | ----------- | -------------------------- | ----- | ---------- | ------------------------------------ |
| 1 | Trương Việt Công  | Khi tiếp nhận hồ sơ vay, tôi muốn nhận biết sớm giấy tờ/thông tin còn thiếu để giảm yêu cầu bổ sung nhiều lần. | Nhân viên tiếp nhận; khách hàng.| Kiểm tra tính đầy đủ, ước tính 10–20 phút/hồ sơ. | Nếu khách hàng nộp đủ nhưng ảnh mờ, cắt góc, hoặc sai định dạng thì sao? Việc cảnh báo thiếu có thực sự giải quyết được việc "bổ sung nhiều lần" nếu chất lượng giấy tờ không được kiểm soát ngay từ đầu? (Nguyễn Trường Duy)  |
| 2 | Trương Việt Công  | Khi hồ sơ đang được thẩm định/phê duyệt, tôi muốn biết hồ sơ đang chờ ở đâu và ai xử lý tiếp để theo dõi bàn giao. | Nhân viên xử lý hồ sơ; quản lý tiến độ. | Chờ giữa lúc bàn giao và lúc bước tiếp theo được nhận. | Việc biết chính xác "ai đang giữ hồ sơ" có thực sự đẩy nhanh được tốc độ xử lý không, hay chỉ giải quyết vấn đề tâm lý (an tâm) của người theo dõi. (Nguyễn Trường Duy) |
| 3 | Trương Việt Công  | Khi rà soát hồ sơ vay, tôi muốn biết thông tin nào đã được kiểm tra để tránh đối chiếu trùng mà vẫn giữ đủ control point. | Nhân viên thẩm định/kiểm soát. | Tìm hoặc đối chiếu lại kết quả trước, ước tính 10–20 phút. | Nếu người trước đánh dấu "đã kiểm tra" (verified) nhưng thực tế có sai sót, và người sau tin tưởng bỏ qua, thì khi phát sinh nợ xấu hoặc lỗi tuân thủ, trách nhiệm sẽ thuộc về ai? (Nguyễn Trường Duy) |
|   4 | Lê Quang Linh     | Khi thẩm định tài liệu kỹ thuật/báo cáo đối thủ (15–20 trang), tôi muốn bóc tách nhanh thông số và chi phí, để lập bảng so sánh đối chuẩn (benchmarking) phục vụ họp chiến lược.                                       | Product Owner / Business Analyst / Solution Engineer                                                           | Bước bóc tách bảng giá/thông số kỹ thuật vào bảng tính (90 phút) và đối chiếu chéo tiêu chí kỹ thuật tương đương (45 phút).                                          | "Nếu tài liệu của các bên dùng thuật ngữ chuyên môn khác nhau hoặc cấu trúc giá dị biệt (bên tính theo API call, bên tính theo user/tháng), hệ thống chuẩn hóa thế nào để số liệu không bị bóp méo?" (Đoàn Văn Tú) |
|   5 | Lê Quang Linh     | Khi đối soát dữ liệu xuất từ CRM/database, tôi muốn rà soát và làm sạch các trường trùng lặp, sai định dạng số ĐT/email, để nạp vào hệ thống marketing mà không bị lỗi bounce.                                         | Data Ops / Sales Operations                                                                                    | Bước rà soát bằng mắt các lỗi font, số ĐT, email (60 phút) và sửa thủ công từng ô lỗi (30 phút).                                                                     | "Tại sao không dùng bộ lọc Regex hoặc validation ngay tại form nhập liệu CRM để chặn lỗi từ đầu mà lại cần tới một quy trình can thiệp phức tạp?"(Đoàn Văn Tú)|
|   6 | Lê Quang Linh     | Khi kết thúc cuộc họp điều hành/khách hàng, tôi muốn trích xuất chính xác các quyết định và đầu việc được giao kèm người phụ trách, để gửi biên bản họp (meeting recap) trong ngày.                                    | Project Manager / Thư ký cuộc họp                                                                              | Bước nghe tua lại các đoạn thảo luận cam kết phức tạp (40 phút) và tổng hợp danh sách việc/deadline (25 phút).                                                       | "Văn phong nói chuyện lúc họp thường nhảy ý và không có cấu trúc cố định; nếu bóc tách tự động bị ảo giác (hallucination) rồi gán nhầm trách nhiệm/deadline cho người khác thì rủi ro xử lý ra sao?" (Đoàn Văn Tú) |
|   7 | Nguyễn Trường Duy | Khi tiếp nhận một bộ hồ sơ vay vốn cá nhân, tôi muốn nhanh chóng kiểm tra tính đầy đủ và hợp lệ của các tài liệu, để đảm bảo hồ sơ đáp ứng yêu cầu trước khi tiến hành thẩm định.                                      | Credit Officer trực tiếp tiếp nhận và kiểm tra hồ sơ vay vốn cá nhân.                                          | Phải mở và kiểm tra từng tài liệu riêng lẻ, mất thời gian khi hồ sơ có nhiều giấy tờ hoặc tài liệu không được sắp xếp thống nhất.                                    | “Lần gần nhất hồ sơ bị thiếu hoặc không hợp lệ là khi nào, và việc đó khiến hồ sơ bị chậm hoặc phải xử lý lại ra sao?” (Truong Viet Cong) |
|   8 | Nguyễn Trường Duy | Khi thẩm định hồ sơ vay vốn, tôi muốn nhanh chóng phát hiện những thông tin không nhất quán giữa các tài liệu và dữ liệu Core Banking, để hạn chế sai sót trong quá trình đánh giá khách hàng và khoản vay.            | Credit Officer chịu trách nhiệm kiểm tra, đối chiếu và xác minh thông tin khách hàng.                          | Phải đối chiếu thủ công giữa nhiều tài liệu và hệ thống khác nhau. Những sai lệch nhỏ có thể bị bỏ sót khi số lượng hồ sơ lớn.                                       | “Những loại sai lệch nào thường gặp, và hiện có bước kiểm tra nào để phát hiện chúng trước khi ảnh hưởng đến kết quả thẩm định?” (Truong Viet Cong) |
|   9 | Nguyễn Trường Duy | Khi hoàn tất quá trình thẩm định hồ sơ vay vốn, tôi muốn tự động tổng hợp thông tin và tạo bản dự thảo báo cáo thẩm định theo biểu mẫu chuẩn, để tiết kiệm thời gian lập báo cáo và chuyển cấp có thẩm quyền phê duyệt | Credit Officer chịu trách nhiệm phân tích hồ sơ, đưa ra nhận xét và lập báo cáo thẩm định trình cấp phê duyệt. | Phải tổng hợp thông tin từ nhiều nguồn và tự viết nội dung nhận xét, đánh giá theo biểu mẫu. Đây là công đoạn tốn thời gian và đòi hỏi khả năng phân tích nghiệp vụ. | “Phần nào trong việc lập báo cáo hiện mất nhiều thời gian nhất, và có mẫu hoặc quy tắc sẵn có nào giúp giảm công việc mà vẫn bảo đảm người có thẩm quyền kiểm tra được?” (Truong Viet Cong) |
|  10 | Đoàn Văn Tú       | Khi nhận nhiều giấy tờ, tôi muốn biết bản nào mới nhất và còn thiếu gì để tránh nhầm lẫn.                                                                                                                              | Nhân viên tiếp nhận hồ sơ                                                                                      | Tìm bản giấy tờ mới nhất và rà soát tài liệu thiếu mất 10 phút/lượt kiểm tra.                                                                                        | Những loại giấy tờ mới đã đáp ứng đủ yêu cầu chưa? (Lê Anh Quân)                                                                                                                 |
|  11 | Đoàn Văn Tú       | Khi cần biết thông tin hồ sơ vay, tôi muốn tự tìm được thông tin để không phải gọi hỏi nhiều lần.                                                                                                                      | Khách hàng có hồ sơ vay                                                                                        | Khách hàng phụ thuộc vào nhân viên; nhân viên phải hỏi bộ phận phụ trách 1–2 lần/hồ sơ, mỗi lần 3 phút.                                                              | Nếu thông tin chưa được cập nhật, trang tra cứu có thực sự giúp khách hàng giảm gọi hỏi không? (Lê Anh Quân)                                                                                                      |
|  12 | Đoàn Văn Tú       | Khi muốn tất toán trước hạn, tôi muốn biết thủ tục và số tiền cần thanh toán để chuẩn bị đầy đủ.                                                                                                                       | Khách hàng muốn tất toán trước hạn                                                                             | Phải liên hệ 1–2 lần để xác nhận thủ tục và số tiền, mỗi cuộc trao đổi 15 phút.                                                                                      | Khách hàng hỏi lại vì hướng dẫn chưa rõ hay vì thay đổi ngày tất toán làm số tiền cần trả thay đổi? (Lê Anh Quân)                                                                                                 |
|  13 | Lê Anh Quân       | Khi rà soát một khoản vay cần theo dõi hoặc thu hồi nợ, tôi muốn nắm được lịch sử xử lý và các lần liên hệ trước đó, để xác định chính xác tình trạng khoản vay.                                                       | Cán bộ quản lý và thu hồi nợ.                                                                                  | Tra cứu lịch sử liên hệ/xử lý cũ qua các file rời rạc và biên bản bàn giao, ước tính 20–30 phút/khoản vay.                                                           | "Nếu hệ thống quản lý nợ đã có ô lưu lịch sử/ghi chú, vấn đề thực sự nằm ở việc thiếu dữ liệu, dữ liệu phân tán hay thao tác tìm kiếm chưa hiệu quả?"                                                |
|  14 | Lê Anh Quân       | Khi tiếp nhận hồ sơ vay vốn, tôi muốn xác định sớm giấy tờ hoặc thông tin còn thiếu, để hạn chế việc yêu cầu khách hàng bổ sung nhiều lần.                                                                             | Nhân viên tín dụng phụ trách tiếp nhận hồ sơ; khách hàng vay vốn.                                              | Kiểm tra tính đầy đủ danh mục giấy tờ và đối chiếu thông tin thiếu, ước tính 30–45 phút/hồ sơ.                                                                       | "Việc hồ sơ bị thiếu là do khách hàng không nắm rõ checklist hay do nghiệp vụ tín dụng quá phức tạp, và AI sẽ đọc hiểu tính hợp lệ của hồ sơ giấy thế nào?"                                          |
|  15 | Lê Anh Quân       | Khi thực hiện nghiệp vụ tín dụng, tôi muốn tìm đúng quy định và biểu mẫu đang có hiệu lực, để tránh sử dụng tài liệu không phù hợp và phải chỉnh sửa hồ sơ.                                                            | Nhân viên tín dụng và cán bộ nghiệp vụ.                                                                        | Tìm kiếm quy định và kiểm tra phiên bản hiệu lực trên các kho tài liệu phân tán, ước tính 20–30 phút/lần.                                                            | "Các quy định và biểu mẫu tín dụng thay đổi thường xuyên, làm thế nào để đảm bảo hệ thống luôn trích xuất đúng phiên bản mới nhất thay vì tài liệu cũ đã hết hiệu lực?"                              |

### 2.2. Cluster

Nhóm có 15 candidate, gom thành 4 cụm dựa trên pattern bản chất công việc:

| Cluster | Các candidate | Pattern chung |
| ------- | ------------- | ------------- |
| A — Tiếp nhận & Kiểm tra hồ sơ tín dụng | #1, #7, #8, #10, #14 | Rà soát danh mục giấy tờ, đối chiếu tính đầy đủ, hợp lệ và tính nhất quán dữ liệu giữa nhiều tài liệu/hệ thống |
| B — Xử lý báo cáo & Phân tích chuyên sâu | #4, #9 | Bóc tách số liệu chuyên ngành từ nhiều nguồn để tổng hợp thành bản nhận xét/báo cáo phân tích |
| C — Theo dõi luồng & Tra cứu trạng thái | #2, #3, #11, #12, #13 | Tra cứu tiến độ xử lý, lịch sử bàn giao hồ sơ và công nợ giữa các phòng ban hoặc với khách hàng |
| D — Chuẩn hóa dữ liệu & Quy định nghiệp vụ | #5, #6, #15 | Làm sạch dữ liệu nội bộ (CRM/regex), trích xuất đầu việc cuộc họp, tra cứu phiên bản biểu mẫu có hiệu lực |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giảm thời gian tiếp nhận và sơ duyệt hồ sơ vay vốn cá nhân mà vẫn đảm bảo tính tuân thủ và chính xác
├── Opportunity A1: Cán bộ tín dụng mất nhiều thời gian mở từng file để rà soát đủ/thiếu danh mục giấy tờ
├── Opportunity A2: Tốn nhiều thời gian đối chiếu chéo số liệu giữa tài liệu giấy/ảnh (CCCD, sao kê, hợp đồng) với hệ thống Core Banking
└── Opportunity A3: Khách hàng thường xuyên bị yêu cầu bổ sung giấy tờ nhiều lần do nhân viên phát hiện thiếu sót rải rác
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- ✗ "Dùng OCR và AI Agent tự động thẩm định và duyệt hồ sơ vay" (Đây là giải pháp nằm ngoài phạm vi bài toán kiểm tra hồ sơ; quyết định tín dụng phải do người có thẩm quyền theo quy trình của tổ chức. Yêu cầu pháp lý/tuân thủ cụ thể cần được bộ phận có thẩm quyền xác nhận.)
- ✗ "Xây dựng cổng portal/chatbot cho khách hàng tra cứu trạng thái hồ sơ" (Đây là solution tính năng phần mềm)
- ✗ "Tự động gửi email đòi khách bổ sung giấy tờ" (Đây là feature/automation cụ thể)

### 2.4. Chấm điểm shortlist (1–5)

Nhóm chọn 3 candidate đại diện nổi bật nhất từ 15 bài toán:

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
| --------- | -------: | -----------: | -----------------: | -------------: | ----------: | -------------------------------------: | ---------------: | ---: |
| **Kiểm tra tính đầy đủ và nhất quán hồ sơ vay (#7 & #8)** | 5 | 5 | 4 | 4 | 4 | 5 | 5 | **32** |
| Bóc tách tài liệu kỹ thuật & đối thủ (#4) | 4 | 4 | 4 | 4 | 4 | 4 | 4 | 28 |
| Tự động tạo dự thảo báo cáo thẩm định (#9) | 4 | 3 | 4 | 4 | 2 | 4 | 3 | 24 |

**Candidate được chọn:** Kiểm tra tính đầy đủ và nhất quán dữ liệu hồ sơ vay vốn cá nhân (Gộp trọng tâm của #1, #7, #8 và #14).

**Vì sao chọn:** 
- Đây là "nỗi đau" lớn nhất trong nhóm, được 4/5 thành viên cùng đưa ra trong buổi pitch với cùng một pattern.
- Quy trình rõ ràng: hồ sơ vay vốn cá nhân luôn có bộ danh mục chuẩn (Checklist: Pháp lý, Nguồn thu, Tài sản bảo đảm).
- Survey CP4 (N=8) cho thấy 7/8 người gặp công đoạn đối chiếu thủ công lâu nhất; thời gian tiếp nhận được chọn nhiều nhất là 30–45 phút (4/8), không phải giá trị trung bình. 7/8 người cho biết 3–5 trong 10 hồ sơ gần nhất cần bổ sung từ 2 lần trở lên.
- Có thể dùng candidate này để so sánh các mức can thiệp No AI, Rule, Workflow và Agent; khảo sát hiện chỉ xác nhận pain, chưa chứng minh mức giải pháp nào hiệu quả.

**Vì sao loại các candidate còn lại:**
- *Bóc tách tài liệu kỹ thuật (#4):* Pain có thật nhưng chỉ phục vụ cá nhân/bộ phận hẹp, không phải là pain tập trung của đa số thành viên nhóm.
- *Tự động tạo dự thảo báo cáo thẩm định (#9):* Đòi hỏi đánh giá năng lực tài chính và phê duyệt rủi ro mang tính chủ quan nghiệp vụ rất cao; khó xây dựng tiêu chí đánh giá (eval) chuẩn mực trong thời lượng buổi lab.

**Xử lý bất đồng (nếu có):** Linh ban đầu muốn bảo lưu bài toán Bóc tách tài liệu kỹ thuật (#4) vì bản thân đã chuẩn bị kỹ ở cá nhân. Tuy nhiên sau khi cả nhóm phân tích cây OST và bảng chấm điểm, Linh đồng thuận chuyển sang bài toán tín dụng vì đây là nghiệp vụ phổ biến, impact lớn cho doanh nghiệp và có nhiều dữ liệu mẫu để giả lập kiểm chứng hơn.

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|--:|---|---|---:|---:|---|
| 1 | Hồ sơ thường thiếu hoặc không nhất quán giấy tờ/thông tin đến mức gây thêm việc cho người tiếp nhận. | Value | 5 | 4 | Survey: 6/8 nêu thiếu phụ lục/sao kê hoặc thông tin không khớp là nguyên nhân gửi lại; mẫu nhỏ, tự báo cáo. |
| 2 | Thiếu sót thường chỉ được phát hiện sau lần kiểm tra đầu, dẫn đến liên hệ bổ sung hoặc hồ sơ phải quay lại bước trước. | Value | 5 | 3 | 5/8 hồ sơ gần nhất cần bổ sung từ 2 lượt trở lên; khảo sát chưa xác nhận chính xác thời điểm phát hiện. |
| 3 | Checklist theo loại hồ sơ có thể giúp phát hiện thiếu giấy tờ sớm mà không làm bỏ qua điểm kiểm soát. | Usability | 4 | 2 | Survey cho thấy 5/8 dùng bảng theo dõi riêng và 3/8 đối chiếu bằng mắt; chưa thử hiệu quả checklist. |
| 4 | Thông tin cần đối chiếu giữa tài liệu và Core Banking có thể được xác định rõ theo quy tắc nghiệp vụ. | Feasibility | 4 | 2 | 7/8 nêu đối chiếu tài liệu với Core Banking là công đoạn tốn thời gian; bộ quy tắc và nguồn chuẩn chưa được xác minh. |
| 5 | Dữ liệu hồ sơ có thể được xử lý trong công cụ được tổ chức cho phép mà vẫn đáp ứng yêu cầu bảo mật và tuân thủ. | Viability | 5 | 1 | Sau — cần xác nhận chính sách với người có thẩm quyền; không tải dữ liệu thật lên dịch vụ ngoài. |
| 6 | Checklist, quy tắc hoặc chức năng sẵn có có thể giảm vấn đề mà chưa cần AI. | Feasibility / Value | 4 | 2 | 5/8 dùng Excel/Google Sheets, 3/8 kiểm tra thủ công; khảo sát chưa đo hiệu quả của các cách này. Cần thử trên bộ hồ sơ mẫu. |

Survey (N=8) cho tín hiệu về #1–#2 và xác nhận đối chiếu thủ công là bottleneck được nêu nhiều nhất. Không có log đối chiếu; thời gian theo khoảng tự báo cáo. Cần hỏi sâu thời điểm phát hiện thiếu sót, kiểm tra hiệu quả checklist/Rule; #4–#5 (nguồn chuẩn và chính sách dữ liệu) vẫn chưa được xác minh.

### 3.2. Kiểm chứng

**Phương pháp:** Nhóm thu thập **8 câu trả lời** qua biểu mẫu khảo sát. Các câu hỏi tập trung vào thời gian tiếp nhận hồ sơ, công đoạn tốn thời gian nhất, số hồ sơ phải yêu cầu bổ sung nhiều lần, cách kiểm tra hiện tại, số lượt bổ sung ở hồ sơ gần nhất, nguyên nhân gửi lại và trải nghiệm gây phiền nhất. Thời gian là nhóm lựa chọn theo khoảng tự báo cáo, không phải số đo từ log.

**Kết quả survey (N = 8):**

| Chỉ số | Kết quả |
|---|---|
| Thời gian tiếp nhận một hồ sơ | 4/8 chọn 30–45 phút; 3/8 chọn 15–30 phút; 1/8 chọn dưới 15 phút. 30–45 phút là khoảng được chọn nhiều nhất, không phải giá trị trung bình. |
| Công đoạn tốn nhiều thời gian nhất | 7/8 chọn đối chiếu số liệu giữa tài liệu giấy/ảnh với Core Banking; 1/8 chọn mở từng file để kiểm tra checklist. |
| Số hồ sơ trong 10 hồ sơ gần nhất cần yêu cầu bổ sung từ 2 lần trở lên | 7/8 chọn 3–5 hồ sơ; 1/8 chọn 0–2 hồ sơ. |
| Số lượt bổ sung ở hồ sơ gần nhất | 3/8 trả lời 1 lần; 4/8 trả lời 2–3 lần; 1/8 trả lời hơn 4 lần. |
| Lý do chính phải gửi lại/bổ sung | 3/8 nêu thông tin không khớp giữa giấy tờ; 3/8 thiếu trang phụ lục/sao kê; 1/8 ảnh mờ/lóa/mất góc; 1/8 danh mục giấy tờ ban đầu chưa rõ. |
| Cách kiểm tra hiện tại | 5/8 dùng Excel/Google Sheets theo dõi riêng; 3/8 nhìn màn hình và đối chiếu thủ công bằng mắt/nhớ. |
| Trải nghiệm gây phiền hoặc tốn thời gian nhất | 5/8 chọn chờ lâu mới biết hồ sơ hợp lệ hay chưa; 2/8 chọn phải chụp và gửi lại nhiều lần; 1/8 chọn khâu chuẩn bị giấy tờ phức tạp. |

Các câu trả lời cho thấy bottleneck nổi bật trong mẫu là đối chiếu thủ công giữa nhiều nguồn. Số liệu là tự báo cáo từ 8 người; chưa có log để xác nhận thời gian thực tế hoặc đại diện cho toàn bộ người xử lý hồ sơ.

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác / giới hạn |
|---|---:|---|---|
| Micro survey người có trải nghiệm | 8 | 7/8 nêu đối chiếu tài liệu với Core Banking là công đoạn tốn thời gian nhất; 7/8 cho biết 3–5 trong 10 hồ sơ gần nhất phải bổ sung từ 2 lần trở lên. | 1/8 cho biết chỉ 0–2 trong 10 hồ sơ cần bổ sung từ 2 lần trở lên; khảo sát không đo log và mẫu nhỏ. |
| Log/timestamp/checklist thực tế | Không sử dụng | Chưa có dữ liệu đối chiếu | Chưa có dữ liệu đối chiếu |

**Nhóm đã sửa problem thế nào sau kiểm chứng:** Nhóm chuyển trọng tâm từ kiểm đếm thiếu giấy tờ đơn thuần sang “đối chiếu thủ công giữa tài liệu và Core Banking, đồng thời phát hiện thông tin không khớp/thiếu trang trước khi chuyển hồ sơ”. Khảo sát cho thấy checklist hiện không phải cách duy nhất đang dùng (5/8 dùng bảng theo dõi riêng, 3/8 đối chiếu bằng mắt), nhưng chưa đo hiệu quả của checklist hay quy tắc. Vì vậy, nhóm sẽ thử checklist/Rule trước; OCR chỉ là hướng cân nhắc nếu đo được rằng thao tác đọc/trích xuất vẫn là bottleneck.
### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Microsoft Azure AI Document Intelligence — OCR và trích xuất biểu mẫu/tài liệu | [Tài liệu chính thức](https://learn.microsoft.com/en-us/azure/ai-services/document-intelligence/overview?view=doc-intel-3.1.0) | Đọc văn bản, cấu trúc, bảng và trường key/value từ tài liệu; có mô hình dựng sẵn và mô hình tùy chỉnh. | Có thể hỗ trợ số hóa/trích xuất dữ liệu để nhân viên rà soát. | Trích xuất không tự chứng minh giấy tờ hợp lệ, dữ liệu đúng hay đủ điều kiện vay; cần kiểm tra độ chính xác trên loại tài liệu thực tế và chính sách lưu/chuyển dữ liệu. | Tách bước OCR/trích xuất khỏi bước xác minh nghiệp vụ; chỉ dùng như hỗ trợ nếu được tổ chức cho phép. |
| Google Cloud Document AI — OCR và bộ xử lý trích xuất | [Danh sách processor chính thức](https://docs.cloud.google.com/document-ai/docs/processors-list) | Nhận dạng văn bản và trích xuất thực thể/trường theo loại processor. | Có các processor theo nhiệm vụ; có thể tham khảo cho bước đọc tài liệu. | Khả năng theo ngôn ngữ/loại giấy tờ và vùng xử lý cần kiểm tra; không thay thế xác minh nguồn chuẩn hay phê duyệt tín dụng. | So sánh trên tài liệu giả lập/đã khử định danh; không đưa hồ sơ thật vào thử nghiệm khi chưa được phép. |
| Amazon Textract — phân tích biểu mẫu và bảng | [Tài liệu chính thức](https://docs.aws.amazon.com/textract/latest/dg/how-it-works-analyzing.html) | Trích xuất text, key-value từ biểu mẫu, bảng và phản hồi theo truy vấn. | Có thể hỗ trợ lấy trường dữ liệu có cấu trúc từ tài liệu. | Đầu ra trích xuất vẫn có thể sai; cần người kiểm tra và cần đánh giá riêng trên tài liệu tiếng Việt/định dạng thực tế cùng yêu cầu bảo mật. | Công cụ có thể hỗ trợ đọc/đối chiếu sơ bộ; quyết định hợp lệ, hạn mức và phê duyệt vẫn thuộc quy trình nghiệp vụ. |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text
Khách hàng nộp hồ sơ
        |
        v
[Nhân viên tiếp nhận mở và sắp xếp từng tài liệu]
        |
        v
[Đối chiếu checklist: đủ / thiếu / không hợp lệ?]
        |
        +---- Phát hiện thiếu/sai ----> [Liên hệ khách hàng bổ sung]
        |                                      |
        |                                      v
        |                              [Nhận lại và kiểm tra lại]
        |                                      |
        +--------------------------------------+
        |
        v
[Đối chiếu thông tin giữa tài liệu và Core Banking]
        |
        v
[Chuyển hồ sơ sang thẩm định khi đã được xác nhận]
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
| ---: | ----- | ----- | ------ | -------------------- | ------- |
| 1 | Khách hàng / nhân viên tiếp nhận | Bộ hồ sơ vay vốn cá nhân và danh mục giấy tờ | Hồ sơ được tiếp nhận, thường gồm nhiều file/ảnh | Mỗi hồ sơ | Tài liệu có thể chưa sắp xếp, khác định dạng hoặc thiếu thông tin |
| 2 | Nhân viên tiếp nhận / tín dụng | Từng tài liệu trong hồ sơ và checklist nghiệp vụ | Danh sách tài liệu đã kiểm tra, các mục nghi thiếu/không hợp lệ | Chưa đo riêng | Phải mở và xem từng tài liệu riêng lẻ; ước tính thời gian trong pitch chưa được bấm giờ xác nhận |
| 3 | Nhân viên tín dụng | Tài liệu đã kiểm tra và dữ liệu trên Core Banking | Kết quả đối chiếu thông tin khách hàng/khoản vay | Chưa đo riêng | 7/8 người chọn đây là công đoạn tốn thời gian nhất; khảo sát không đo thời lượng riêng của bước |
| 4 | Nhân viên tiếp nhận / khách hàng | Danh sách thiếu, sai hoặc cần làm rõ | Yêu cầu bổ sung/chỉnh sửa và hồ sơ được gửi lại | Thường lặp lại 1 hoặc nhiều lần | Các thiếu sót được phát hiện rải rác, khách hàng phải bổ sung nhiều lần |
| 5 | Nhân viên tín dụng / thẩm định | Hồ sơ đã bổ sung và kết quả đối chiếu | Hồ sơ được xác nhận để chuyển sang thẩm định | Thời gian tự báo cáo: 4/8 chọn 30–45 phút; 3/8 chọn 15–30 phút; 1/8 chọn dưới 15 phút | Đây là các khoảng lựa chọn, không phải thời gian trung bình; chưa đối chiếu log |

**Bottleneck chính:** Trong khảo sát, 7/8 người chọn đối chiếu thông tin giữa tài liệu và Core Banking là công đoạn tốn thời gian nhất; 5/8 chọn việc chờ lâu mới biết hồ sơ hợp lệ hay chưa là trải nghiệm phiền nhất. Khảo sát ghi nhận 5/8 hồ sơ gần nhất cần bổ sung từ 2 lượt trở lên, nhưng chưa xác định được thiếu sót được phát hiện ở bước nào hoặc đo thời gian của từng bước.

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text
Khách hàng nộp tài liệu
        |
        v
[Rule: tiếp nhận, phân loại tài liệu và kiểm tra định dạng cơ bản]
        |
        v
[AI: OCR/trích xuất các trường cần thiết từ tài liệu]
        |
        v
[Rule: đối chiếu checklist bắt buộc và dữ liệu Core Banking]
        |
        +---- Dữ liệu đầy đủ, khớp và độ tin cậy đạt ngưỡng ----+
        |                                                       |
        |                                                       v
        |                                      [Con người xác nhận kết quả]
        |                                                       |
        |                                                       v
        |                                      [Chuyển hồ sơ sang thẩm định]
        |
        +---- Thiếu/sai/không chắc chắn ----------------------->
                         [Con người xem tài liệu gốc và quyết định]
                                      |
                    +-----------------+------------------+
                    |                                    |
                    v                                    v
       [Yêu cầu khách hàng bổ sung]        [Chấp nhận ngoại lệ/cần làm rõ]
                    |                                    |
                    +----------------> [Cập nhật và kiểm tra lại]

Boundary: Hệ thống chỉ trích xuất, kiểm tra đầy đủ và đánh dấu sai lệch;
không tự động kết luận khả năng vay, xếp hạng rủi ro hay phê duyệt khoản vay.
```

| Bước | Loại xử lý | Actor chính | Input / output | Boundary và phương án quay về |
| ---: | --------- | ----------- | -------------- | ----------------------------- |
| 1 | **Rule** | Hệ thống + nhân viên tiếp nhận | Tiếp nhận file, phân loại theo loại giấy tờ, kiểm tra file có đọc được và đúng định dạng | File không đọc được được đưa vào hàng đợi xử lý thủ công; không tự động loại hồ sơ |
| 2 | **AI** | Hệ thống hỗ trợ, nhân viên giám sát | OCR/trích xuất các trường trên CCCD, sao kê, hợp đồng và tài liệu liên quan | Nếu độ tin cậy thấp, thiếu trường hoặc sai loại tài liệu thì giữ lại tài liệu gốc và chuyển HITL |
| 3 | **Rule** | Hệ thống + nhân viên tín dụng | Kiểm tra checklist bắt buộc và đối chiếu các trường với Core Banking | Rule chỉ đánh dấu thiếu/sai lệch; không tự kết luận hồ sơ đủ điều kiện vay |
| 4 | **Con người (HITL)** | Nhân viên tiếp nhận / tín dụng | Xem danh sách cảnh báo, tài liệu gốc và nguồn dữ liệu chuẩn | Nhân viên xác nhận, sửa kết quả trích xuất hoặc ghi nhận ngoại lệ; đây là điểm kiểm soát bắt buộc |
| 5 | **Con người + workflow** | Nhân viên tiếp nhận và khách hàng | Danh sách thiếu/sai đã được gom theo một lần yêu cầu | Nếu còn thiếu thông tin, quay về bước 1-3; nếu đạt yêu cầu, chuyển sang thẩm định |

**Phương án quay về khi AI sai:** Không dùng kết quả AI nếu không đạt ngưỡng độ tin cậy hoặc không khớp với tài liệu gốc. Nhân viên mở tài liệu gốc, sửa/xác nhận trường dữ liệu thủ công và ghi nhận lý do. Nếu hệ thống không hoạt động, quy trình fallback là checklist và đối chiếu thủ công như quy trình hiện tại.

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
| ------ | ----- | ------------- | ------- |
| Số bước | 5 bước chính, có thể lặp lại bước 3-4 | 5 bước chính; phần kiểm tra được chạy tự động trước khi chuyển HITL | Số bước trên sơ đồ không giảm nhiều, nhưng giảm số lần lặp và thời gian xử lý ở mỗi bước |
| Tổng thời gian | Survey tự báo cáo: 4/8 chọn 30–45 phút, 3/8 chọn 15–30 phút, 1/8 chọn dưới 15 phút | Mục tiêu thử nghiệm: 15–25 phút/hồ sơ nếu tài liệu đọc được và dữ liệu khớp; ngoại lệ có thể lâu hơn | 30–45 phút là khoảng được chọn nhiều nhất, không phải trung bình; đo trước/sau trên cùng bộ hồ sơ để kiểm tra target |
| Số bước thủ công | Khoảng 4-5 bước: mở file, kiểm tra checklist, đối chiếu Core Banking, lập yêu cầu bổ sung và kiểm tra lại | Khoảng 1-2 bước: xem cảnh báo/tài liệu gốc và xác nhận hoặc sửa kết quả trước khi chuyển thẩm định | Rule và AI chỉ hỗ trợ sàng lọc; quyết định nghiệp vụ vẫn do con người thực hiện |
| Bottleneck chính | Mở và kiểm tra từng tài liệu; đối chiếu thủ công giữa nhiều nguồn; phát hiện thiếu sót rải rác nên phải yêu cầu bổ sung nhiều lần | Xử lý các trường hợp AI trích xuất không chắc chắn, dữ liệu không khớp hoặc checklist có ngoại lệ | Cần thiết kế hàng đợi HITL và hiển thị bằng chứng từ tài liệu gốc để người dùng kiểm tra nhanh |
| Rủi ro mới phát sinh | Bỏ sót thiếu/sai lệch, xử lý lại nhiều lần và kéo dài thời gian chờ | OCR/trích xuất sai, cảnh báo nhầm hoặc bỏ sót; rò rỉ dữ liệu hồ sơ; người dùng quá tin vào kết quả tự động | Giảm thiểu bằng ngưỡng độ tin cậy, đối chiếu tài liệu gốc, log/audit, phân quyền dữ liệu và bắt buộc HITL trước khi chuyển thẩm định |

---

## 5. Problem Statement v0 (CP5)
 
| Trường | Nội dung |
| ------ | -------- |
| **Actor** | Nhân viên tiếp nhận / Credit Officer xử lý hồ sơ vay vốn cá nhân. Khách hàng vay vốn là bên chịu ảnh hưởng khi bị yêu cầu bổ sung nhiều lần. |
| **Quy trình** | Từ lúc nhận bộ hồ sơ của khách đến lúc chuyển sang thẩm định: mở từng tài liệu, đối chiếu checklist đủ/thiếu/hợp lệ, đối chiếu thông tin giữa tài liệu và Core Banking, liên hệ khách bổ sung rồi kiểm tra lại. |
| **Bottleneck** | Survey (N=8): 7/8 chọn đối chiếu số liệu giữa tài liệu giấy/ảnh với Core Banking là công đoạn tốn thời gian nhất; 1/8 chọn mở từng file kiểm tra checklist. Khảo sát không đo thời lượng từng công đoạn; các con số 10–20 phút ở một số pitch là ước tính ban đầu, chưa được xác minh bằng bấm giờ. |
| **Impact** | Survey (N=8): thời gian tiếp nhận tự báo cáo gồm 4/8 chọn 30–45 phút, 3/8 chọn 15–30 phút, 1/8 chọn dưới 15 phút. 5/8 trả lời hồ sơ gần nhất cần bổ sung từ 2 lượt trở lên; riêng câu hỏi về 10 hồ sơ gần nhất, 7/8 chọn khoảng 3–5 hồ sơ cần bổ sung từ 2 lần trở lên. 5/8 cũng chọn chờ lâu mới biết hồ sơ hợp lệ hay chưa là trải nghiệm phiền nhất. Đây là tự báo cáo, chưa đối chiếu log. |
| **Success Metric** (baseline → target, cách đo) | **Chính:** baseline khảo sát là phân bố theo khoảng: 4/8 ở 30–45 phút, 3/8 ở 15–30 phút, 1/8 dưới 15 phút; không suy ra trung bình chính xác. Mục tiêu thử nghiệm đề xuất là 15–25 phút/hồ sơ; đo bằng cách bấm giờ cùng 5–10 hồ sơ giả lập/đã ẩn danh trước và sau. **Phụ:** baseline tự báo cáo gồm 5/8 hồ sơ gần nhất có từ 2 lượt bổ sung trở lên; pilot đo lại số lượt bổ sung trên cùng bộ hồ sơ và đặt mục tiêu giảm. **Guardrail:** tỉ lệ bỏ sót thiếu/sai lệch trên bộ hồ sơ đã gài lỗi sẵn không cao hơn cách làm thủ công hiện tại. |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | AI/Rule **không** kết luận hồ sơ đủ điều kiện vay, không xếp hạng rủi ro, không đề xuất hay phê duyệt/từ chối khoản vay; không tự sửa dữ liệu Core Banking; không tự gửi yêu cầu cho khách hàng; không tự loại hồ sơ khi file không đọc được. Con người **luôn** kiểm tra: mọi cảnh báo thiếu/sai lệch, mọi trường độ tin cậy thấp hoặc thiếu, và xác nhận hồ sơ trước khi chuyển thẩm định. Dữ liệu thật không được đưa lên dịch vụ ngoài khi chưa có xác nhận của người có thẩm quyền; lab chỉ dùng dữ liệu giả lập/khử định danh. |
 
**Phản biện nhận được và nhóm có đồng ý không:**
 
 
| # | Câu hỏi / lỗ hổng (từ AI) | Nhóm trả lời / điều chỉnh | Đồng ý? |
| -: | ------------------------- | ------------------------- | ------- |
| 1 | Nhân viên có kiểm tra tài liệu gốc hay chỉ bấm xác nhận cảnh báo? | Hiển thị cảnh báo cạnh trang tài liệu và đánh dấu vị trí cần kiểm tra. Với cảnh báo quan trọng, nhân viên phải xác nhận từng mục và ghi lý do xử lý, không cho xác nhận hàng loạt. Kiểm tra mẫu định kỳ để phát hiện việc duyệt qua loa; thiết kế không thể bảo đảm tuyệt đối nhân viên luôn đọc kỹ. | ☑ Đồng ý |
| 2 | Bổ sung nhiều lần do khách không biết cần nộp gì hay nhân viên phát hiện thiếu muộn? | Bổ sung checklist cho khách ngay khi tạo hồ sơ; hệ thống kiểm tra sơ bộ lúc tải lên và nhân viên rà soát trước khi chuyển thẩm định. Các yêu cầu bổ sung phát hiện được trong lượt kiểm tra được tổng hợp thành một danh sách gửi khách sau khi nhân viên xác nhận. | ☑ Đồng ý |
| 3 | Ảnh mờ, cắt góc, sai định dạng được xử lý ở đâu? | Kiểm tra chất lượng ngay lúc khách tải tài liệu lên. Nếu ảnh không đọc được hoặc thiếu phần cần thiết, thông báo rõ lỗi và yêu cầu chụp lại tại bước đó. Trường hợp không xác định được chuyển nhân viên kiểm tra; nhân viên xác nhận yêu cầu bổ sung trước khi gửi khách. | ☑ Đồng ý |
| 4 | Ai chịu trách nhiệm khi hệ thống bỏ sót? Kết quả kiểm tra có được công nhận không? | Không có cảnh báo không đồng nghĩa hồ sơ đạt. Nhân viên vẫn kiểm tra các mục bắt buộc và quyết định trong phạm vi thẩm quyền. Nhóm chưa có căn cứ kết luận trách nhiệm pháp lý hoặc giá trị chứng từ của kết quả máy; cần bộ phận nghiệp vụ, pháp chế và tuân thủ xác nhận trước triển khai thật. Trước mắt chỉ thử nghiệm hỗ trợ, không thay thế bước kiểm soát hiện hành. | ☑ Đồng ý |
| 5 | Ai định nghĩa “hợp lệ” và cập nhật checklist? | Đổi “hợp lệ” thành “đủ và khớp theo checklist phiên bản đang áp dụng”, không đồng nghĩa đủ điều kiện cho vay. Đề xuất bộ phận nghiệp vụ quản lý nội dung, bộ phận có thẩm quyền phê duyệt và bộ phận kỹ thuật triển khai. Mỗi checklist phải có phiên bản, ngày hiệu lực và người duyệt; lưu phiên bản đã dùng cho từng lượt kiểm tra. Nếu chưa xác định được checklist áp dụng thì chuyển xử lý thủ công. | ☑ Đồng ý |
| 6 | Giấy tờ giả hoặc chỉnh sửa có thuộc phạm vi không? | Phát hiện giả mạo chưa thuộc phạm vi phiên bản đầu. OCR đọc đúng và các trường khớp nhau không chứng minh giấy tờ thật. Giữ bước xác minh danh tính, nguồn chứng từ và kiểm soát gian lận theo quy trình của đơn vị; cần xác nhận cụ thể các bước này trước khi thử nghiệm thực tế. Trường hợp nghi ngờ chuyển người có thẩm quyền xử lý. | ☑ Đồng ý |
| 7 | Độ chính xác OCR và ngưỡng tin cậy được đánh giá thế nào? | Đánh giá OCR theo từng loại tài liệu và từng trường thông tin, ưu tiên các trường quan trọng như số CCCD, họ tên và số tiền. Điểm tin cậy chỉ dùng để hỗ trợ phân luồng; trường khó đọc hoặc có mâu thuẫn phải được nhân viên đối chiếu bản gốc. Bộ phận nghiệp vụ phối hợp với nhóm kỹ thuật quyết định ngưỡng chấp nhận dựa trên kết quả đánh giá và mức độ rủi ro. | ☑ Đồng ý |
| 8 | Lấy dữ liệu Core Banking thế nào, so bằng khóa nào và nguồn nào là chuẩn? | Đề xuất lấy dữ liệu qua API được ngân hàng cấp quyền hoặc file xuất theo mẫu thống nhất; ghép bằng mã hồ sơ liên kết với mã khách hàng, không chỉ dựa vào họ tên. Bộ phận nghiệp vụ xác định nguồn chuẩn cho từng trường và thời điểm cập nhật. Khi có chênh lệch, hệ thống đánh dấu để nhân viên xác minh, không tự ghi đè hoặc mặc định dữ liệu Core Banking luôn đúng. | ☑ Đồng ý |
| 9 | Dữ liệu được lưu ở đâu, ai được xem và truy vết thế nào? | Thiết kế lưu và xử lý dữ liệu trong môi trường được ngân hàng phê duyệt, phân quyền theo vai trò và hồ sơ được giao. Nhật ký ghi phiên bản tài liệu, mô hình và checklist, kết quả trích xuất, cảnh báo, người sửa hoặc duyệt, thời điểm và lý do. Hạn chế đưa dữ liệu nhạy cảm vào log; quy định thời hạn lưu, quyền truy cập và cách xóa dữ liệu. | ☑ Đồng ý |

## 6. Mức can thiệp AI (CP6)

 
### 6.1. Ma trận độ mơ hồ × độ phức tạp

 
| Trục | Định nghĩa (worksheet) | Bài của nhóm | Kết luận |
| ---- | ---------------------- | ------------ | -------- |
| **Độ mơ hồ** | Thấp khi kết quả có đúng/sai rõ; cao khi nhiều đầu ra khác nhau đều chấp nhận được | Mỗi phép kiểm tra cho kết quả có/không: giấy tờ có trong hồ sơ hay không, còn hạn hay không, số CCCD trên tài liệu có trùng dữ liệu Core Banking hay không. Hai người kiểm tra cùng một hồ sơ theo cùng checklist sẽ ra cùng kết quả. Những việc cần phán đoán (chấp nhận ngoại lệ, kết luận hồ sơ) nhóm giao cho con người và đặt ngoài phạm vi của AI . | **Thấp** |
| **Độ phức tạp** | Cao khi có từ 3 bước nối tiếp, từ 3 nguồn dữ liệu, và bước sau phụ thuộc bước trước | Có 5 bước nối tiếp (bảng 4.1); 3 nguồn dữ liệu (tài liệu ảnh/scan, checklist, Core Banking); việc đối chiếu chỉ làm được sau khi đã đọc xong tài liệu. | **Cao** |
 
 Không cần AI tự quyết bước tiếp theo, nên không chọn Agent. AI (nếu dùng) chỉ cần làm một bước là đọc nội dung ảnh/scan; các bước còn lại do Rule hoặc con người đảm nhiệm.
 

### 6.2. So sánh 4 mức
 
| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
| --- | -------------------------- | ---------- | ------ | ----- |
| **No AI** (sửa quy trình) | Checklist chuẩn theo loại khoản vay, hướng dẫn khách nộp đúng định dạng và đủ giấy tờ, thư mục chuẩn khi tiếp nhận | Thiếu sót chủ yếu do khách không nắm checklist (câu hỏi ở pitch #14); tài liệu phần lớn là file số rõ nét | Nhân viên vẫn mở từng file và đối chiếu Core Banking bằng tay, nên không chạm tới bottleneck chính | **Có, giai đoạn 1** (không đủ khi đứng một mình) |
| **Rule** | Script kiểm tra danh mục bắt buộc, định dạng file, ngày cấp/hạn; so khớp trường dữ liệu với Core Banking | Dữ liệu đã ở dạng có cấu trúc (nhập sẵn hoặc file số đọc được) | Không đọc được nội dung ảnh/scan CCCD, sao kê, hợp đồng; vẫn phải nhập tay những trường này | **Có, giai đoạn 1** (bước 1 và 3 trong quy trình tương lai) |
| **Workflow** | Các bước định sẵn bằng code; AI chỉ làm **một bước**: OCR/trích xuất trường từ ảnh/scan, kèm độ tin cậy; con người xác nhận | Tài liệu chủ yếu là ảnh/scan, nhiều loại giấy tờ, Rule một mình không đọc được | OCR sai (nhất là tiếng Việt, ảnh mờ, cắt góc); dữ liệu nhạy cảm; automation bias; chi phí vận hành | **Có, giai đoạn 2**, chỉ khi giai đoạn 1 chưa đủ và vượt các điều kiện ở mục 8 |
| **Agent** | AI tự quyết bước tiếp theo: tự chọn tài liệu cần xem, tự hỏi khách, tự kết luận hồ sơ | Quy trình không định sẵn được, nhiều nhánh không đoán trước | Vi phạm boundary và yêu cầu tuân thủ; khó kiểm soát trách nhiệm; không có bằng chứng cần thiết | **Không** |
 
**Mức chọn:** Workflow - AI chỉ ở một bước trích xuất, Rule làm phần còn lại, con người quyết định, **triển khai theo giai đoạn**: giai đoạn 1 là No AI + Rule, giai đoạn 2 thêm OCR nếu đo thấy chưa đủ.
 
**Vì sao không chọn mức đơn giản hơn:**  Nhóm sẽ thử checklist và Rule trước để kiểm tra giấy tờ bắt buộc và đối chiếu dữ liệu đã có sẵn. Nếu nhân viên vẫn phải mở nhiều ảnh/scan để đọc và nhập thông tin, nhóm mới bổ sung OCR trong Workflow: trích xuất thông tin → Rule đối chiếu → nhân viên kiểm tra. Vì dữ liệu khách hàng gắn cho vay vốn đóng vai trò quan trọng trong việc xác minh, OCR có tỷ lệ sai lệch nhất định.
 
### 6.3. AI Canvas rút gọn
 
| Thành phần | Nội dung |
| ---------- | -------- |
| **Prediction** — AI dự đoán / tạo ra gì? | Đọc ảnh/scan CCCD, sao kê, hợp đồng và trả về các trường dữ liệu (họ tên, số CCCD, ngày sinh, thu nhập…) kèm độ tin cậy và cờ chất lượng (mờ, cắt góc, sai loại tài liệu). AI **không** dự đoán khả năng vay hay rủi ro tín dụng. |
| **Judgment** — con người cân nhắc, quyết định gì? | Credit Officer xem tài liệu gốc ở các ô bị cờ hoặc độ tin cậy thấp, quyết định trường nào đúng, ngoại lệ nào chấp nhận, hồ sơ cần bổ sung hay đã đủ để chuyển thẩm định. |
| **Action** — hành động cuối cùng là gì, ai làm? | Nhân viên xác nhận/sửa dữ liệu, gửi yêu cầu bổ sung gộp một lần cho khách, chuyển hồ sơ sang thẩm định. Hệ thống không tự làm các việc này. |
| **Outcome** — đo kết quả bằng gì? | Thời gian kiểm tra/hồ sơ , số lượt bổ sung/hồ sơ (→ tối đa 1), tỉ lệ bỏ sót và báo nhầm trên bộ hồ sơ giả lập. |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | Ảnh/scan tài liệu của hồ sơ; checklist bắt buộc theo loại khoản vay; dữ liệu Core Banking để so khớp. Hồ sơ có sẵn nhưng là dữ liệu nhạy cảm, nên lab dùng hồ sơ giả lập/khử định danh. **Chưa xác nhận** quyền truy cập Core Banking thật và chính sách cho phép xử lý dữ liệu ngoài hạ tầng tổ chức. |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | Log các trường nhân viên sửa so với kết quả AI (theo loại giấy tờ); lý do ngoại lệ; hồ sơ bị trả lại ở bước thẩm định; ý kiến nhân viên về cảnh báo thừa/thiếu. |
 
### 6.4. Hai câu hỏi của Google PAIR
 
- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Survey xác nhận một số khó khăn nhưng không hỏi sở thích giao việc hay hỗ trợ. Thiết kế tạm chọn **augment**, dựa trên yêu cầu nhân viên xác nhận/sửa kết quả và giới hạn quyền tự quyết; cần kiểm chứng riêng với người làm nghiệp vụ.
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? **Bỏ sót tệ hơn**: một giấy tờ thiếu hoặc sai lệch lọt qua có thể ảnh hưởng chất lượng thẩm định và tuân thủ, còn báo nhầm chỉ tốn thêm vài phút xem lại tài liệu gốc. Thiết kế đã xử lý: đặt ngưỡng cờ thận trọng (nghiêng về báo nhầm), mọi trường độ tin cậy thấp luôn vào HITL, bước 4 xác nhận bắt buộc với mọi hồ sơ, và có guardrail bỏ sót. Đồng thời phải giới hạn báo nhầm, vì cảnh báo thừa quá nhiều sẽ khiến người dùng bỏ qua cảnh báo (alert fatigue).
---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường                                          | Nội dung                        |
| ----------------------------------------------- | ------------------------------- |
| **Actor**                                       |Nhân viên tiếp nhận / Credit Officer phụ trách rà soát sơ bộ hồ sơ vay vốn cá nhân. Khách hàng vay vốn là đối tượng thụ hưởng gián tiếp (giảm số lần bị đòi bổ sung giấy tờ).                                 |
| **Quy trình**                                   |Quy trình tiếp nhận & sơ duyệt (5 bước): Tiếp nhận & kiểm tra định dạng file (Rule) $\rightarrow$ OCR/Trích xuất trường dữ liệu từ ảnh/scan (AI) $\rightarrow$ Kiểm tra danh mục checklist & đối chiếu chéo số liệu với Core Banking (Rule) $\rightarrow$ Cán bộ tín dụng rà soát cảnh báo, đối chiếu tài liệu gốc và xác nhận (HITL) $\rightarrow$ Xuất biên bản tiếp nhận/yêu cầu bổ sung gộp 1 lần hoặc chuyển thẩm định.                                 |
| **Bottleneck**                                  |Thao tác mở từng file ảnh/scan để đọc và gõ lại thông tin; đối chiếu thủ công từng trường dữ liệu giữa hồ sơ và Core Banking; phát hiện sai sót rải rác qua nhiều lượt dẫn đến lặp lại quy trình.                                 |
| **Impact**                                      |Survey (N=8): 7/8 chọn đối chiếu thủ công giữa tài liệu với Core Banking là công đoạn tốn thời gian nhất; thời gian tiếp nhận tự báo cáo phân bố 4/8 ở 30–45 phút, 3/8 ở 15–30 phút và 1/8 dưới 15 phút. 5/8 hồ sơ gần nhất có từ 2 lượt bổ sung trở lên; ở câu hỏi về 10 hồ sơ gần nhất, 7/8 chọn khoảng 3–5 hồ sơ có từ 2 lượt bổ sung trở lên; 5/8 chọn chờ lâu mới biết hồ sơ hợp lệ hay chưa là trải nghiệm phiền nhất. Mẫu nhỏ, tự báo cáo, chưa có log.                                 |
| **Success Metric** (baseline → target, cách đo) |- Metric chính (Thời gian): baseline là phân bố theo khoảng nêu trên, không phải trung bình. Mục tiêu thử nghiệm đề xuất 15–25 phút/hồ sơ; đo bằng cách bấm giờ 5–10 bộ hồ sơ giả lập/đã khử định danh trước và sau. <br>- Metric phụ (Lần lặp): baseline survey là 5/8 hồ sơ gần nhất có từ 2 lượt bổ sung trở lên; pilot đo lại trên cùng bộ hồ sơ và đặt mục tiêu giảm tỷ lệ này. <br>- Guardrail metric: Tỉ lệ bỏ sót sai lệch/thiếu sót (False Negative) trên bộ test gài lỗi không cao hơn phương pháp thủ công hiện tại; mục tiêu 0% bỏ sót sai lệch nghiêm trọng về danh tính và nguồn thu.                                |
| **Boundary**                                    |- AI/Rule tuyệt đối không: tự động duyệt/từ chối khoản vay, không xếp hạng điểm tín dụng, không tự sửa dữ liệu trên Core Banking, không tự động gửi email/tin nhắn yêu cầu khách bổ sung khi chưa có nhân viên duyệt, không tự động xóa/loại bỏ hồ sơ bị lỗi mờ. <br>- Con người bắt buộc kiểm tra (HITL): Mọi cờ cảnh báo bất thường, các trường dữ liệu có điểm tin cậy (confidence score) thấp hơn ngưỡng quy định, và ký xác nhận chuyển bước. Không đưa dữ liệu thật lên dịch vụ đám mây công cộng bên ngoài.                                 |
| **AI intervention point**                       |Can thiệp duy nhất tại Bước 2: Đọc và bóc tách các trường thực thể có cấu trúc (Họ tên, CCCD/CMND, Ngày sinh, Địa chỉ, Thu nhập, Ngày cấp...) từ các file tài liệu scan/ảnh (CCCD, hợp đồng lao động, sao kê tài khoản ngân hàng), đồng thời gắn nhãn chất lượng ảnh (đủ sáng, mờ, mất góc).                                 |
| **Mức chọn**                                    | Workflow (Phối hợp đa tầng: Triển khai Giai đoạn 1 gồm No AI + Rule; Giai đoạn 2 tích hợp AI OCR trích xuất trường dữ liệu trong workflow có con người kiểm soát - HITL). |
| **Rủi ro & người kiểm tra**                     |- Rủi ro: AI trích xuất sai số liệu tiếng Việt/ảnh mờ; Cán bộ tín dụng bị phụ thuộc/chủ quan duyệt vội (automation bias); Báo nhầm quá nhiều gây mệt mỏi (alert fatigue); Rò rỉ thông tin cá nhân. <br>- Người kiểm tra: Credit Officer trực tiếp phụ trách hồ sơ (kiểm tra hàng ngày); Trưởng bộ phận thẩm định/kiểm soát chất lượng (hậu kiểm ngẫu nhiên định kỳ 10% hồ sơ).                                 |

**Thay đổi so với v0 và lý do:**

| Trường | v0  | v1  | Vì sao đổi |
| ------ | --- | --- | ---------- |
|AI intervention point|Chưa định vị rõ ràng vị trí đứng của mô hình trong luồng hệ thống.|Xác định cụ thể duy nhất ở Bước 2 (chỉ làm nhiệm vụ OCR/trích xuất thực thể từ ảnh/scan tài liệu).|Tránh bẫy giải pháp "AI làm tất cả", làm rõ ranh giới kỹ thuật giữa Rule Engine (đối chiếu logic, checklist) và AI (thị giác máy tính/NLP trích xuất văn bản).|
|Boundary & HITL|Đặt ranh giới chung chung là "không tự duyệt vay, con người kiểm tra cảnh báo".|Cụ thể hóa cơ chế HITL: bắt buộc duyệt từng trường có điểm tin cậy (confidence) thấp; cấm hoàn toàn tính năng "xác nhận hàng loạt" (bulk approve) để chống duyệt qua loa; cấm tự động gửi mail/tin nhắn cho khách.|Khắc phục trực tiếp lỗ hổng phản biện số 1 và số 4: ngăn chặn triệt để tâm lý chủ quan (automation bias) và bảo đảm tính chịu trách nhiệm cá nhân trong nghiệp vụ ngân hàng.|
|Mức chọn|Chỉ ghi nhận chọn mức can thiệp là Workflow.|Bổ sung chiến lược triển khai theo 2 giai đoạn: Giai đoạn 1 làm No AI (chuẩn hóa checklist) + Rule; Giai đoạn 2 mới gắn AI OCR vào luồng.|Giảm thiểu rủi ro đầu tư lãng phí; nếu bước 1 giải quyết được phần lớn rắc rối do khách nộp sai mà không tốn chi phí AI thì giữ nguyên, chỉ nâng cấp khi dữ liệu scan/ảnh thực sự là điểm nghẽn lớn.|
|Success Metric|Bản v0 từng nêu thời lượng mục tiêu mà chưa ghi rõ cách đo.|Bản v1 giữ 15–25 phút/hồ sơ như mục tiêu thử nghiệm đề xuất, kèm cách bấm giờ trên bộ hồ sơ giả lập/đã khử định danh và guardrail về bỏ sót sai lệch nghiêm trọng.|Đây là target cần kiểm chứng, không phải kết quả khảo sát hay mức giảm đã được chứng minh.|

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

|   # | Tiêu chí | Đạt khi | Không đạt khi |
| --: | -------- | ------- | ------------- |
|   1 |Độ chính xác trích xuất thực thể quan trọng (Field-level Accuracy)|Trích xuất chính xác $\ge 98\%$ trên các trường cốt lõi (Số CCCD, Họ tên, Ngày cấp/hết hạn, Số tài khoản, Thu nhập ròng từng tháng) đối với tài liệu đạt chuẩn chất lượng scan/ảnh rõ nét.|Nhận diện sai ký tự số CCCD, đọc nhầm số tiền lương (sai dấu chấm/phẩy), hoặc làm biến dạng họ tên tiếng Việt có dấu.|
|   2 |Khả năng nhận diện chất lượng tài liệu đầu vào (Quality Pre-check)|Cảnh báo đúng $\ge 95\%$ các trường hợp ảnh mờ, chói lóa, mất 4 góc, nghiêng lệch quá $15^\circ$ hoặc tải sai danh mục (ví dụ: tải ảnh bằng lái xe vào ô CCCD).|Bỏ qua ảnh chụp không thể đọc được nội dung hoặc báo lỗi sai trên tài liệu scan rõ ràng, hợp lệ.|
|   3 |Độ tin cậy của chỉ số tin cậy (Confidence Calibration)|Mô hình gán điểm tin cậy (Confidence score) thấp ($< 0.85$) chính xác vào các ký tự/vùng ảnh bị mờ, đè chữ, chữ viết tay hoặc chữ ký để đẩy sang hàng đợi HITL.|Tự tin gán nhãn điểm cao ($\ge 0.95$) cho một trường dữ liệu bị đọc sai lệch ký tự thực tế (False High-Confidence).|
|   4 |Định dạng cấu trúc dữ liệu đầu ra (Schema Conformance)|$100\%$ kết quả trả về đúng định dạng JSON/Schema chuẩn mực theo quy định (ngày tháng theo chuẩn YYYY-MM-DD, số tiền dạng số nguyên chuẩn hóa, loại bỏ ký tự rác).|JSON sai định dạng, gán sai kiểu dữ liệu (chuỗi text lẫn vào trường số tiền) làm sập Rule Engine đối chiếu ở bước kế tiếp.|

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro          | Câu hỏi                                                           | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
| --------------- | ----------------------------------------------------------------- | ----------------------------------------------------- | ------------------ |
| **Value**       | Người dùng có thật sự cần và sẽ dùng không?                       | Trung bình | Trong 8 câu trả lời, 7/8 nêu đối chiếu thủ công với Core Banking là công đoạn tốn thời gian nhất; 5/8 hồ sơ gần nhất cần bổ sung từ 2 lượt trở lên. Mẫu nhỏ, tự báo cáo và chưa có log để xác nhận tác động. |
| **Usability**   | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | Trung bình | Luồng dự kiến có nhân viên xem cảnh báo cạnh tài liệu gốc và xác nhận/sửa trước khi chuyển bước. Chưa thử nghiệm với Credit Officer; cảnh báo nhiều có thể làm tăng tải và gây mệt mỏi. |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không?                     | Cao | Tài liệu công khai cho thấy có công cụ OCR/trích xuất biểu mẫu, nhưng nhóm chưa thử trên hồ sơ tiếng Việt đại diện, chưa đo độ chính xác trên tài liệu mờ/đa định dạng và chưa xác nhận quyền truy cập hay tích hợp Core Banking. |
| **Viability**   | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành?     | Cao | Hồ sơ vay chứa dữ liệu tài chính và định danh. Chưa có xác nhận của bộ phận bảo mật, pháp chế/tuân thủ hoặc chủ hệ thống về nơi xử lý, lưu trữ, quyền truy cập, chi phí và trách nhiệm vận hành. |

### 8.2. Kết luận

**Quyết định: Not Yet.** Chỉ cân nhắc pilot kỹ thuật giới hạn sau khi hoàn tất các điều kiện bên dưới; chưa đủ căn cứ triển khai trên hồ sơ thật hoặc hệ thống ngân hàng.

**Lý do:** Candidate có thể kiểm chứng và có hướng thử đơn giản bằng checklist/Rule, nhưng Value chưa được xác nhận với người làm nghiệp vụ. Rủi ro Feasibility và Viability đang cao vì chưa đánh giá trên tài liệu phù hợp và chưa có phê duyệt về dữ liệu/hệ thống. Tài liệu nhà cung cấp chỉ chứng minh có khả năng OCR/trích xuất nói chung, không chứng minh độ chính xác hoặc tính phù hợp cho quy trình tín dụng của nhóm.

**Nếu đủ điều kiện để pilot nhỏ nhất:** Bắt đầu bằng checklist và Rule trên bộ hồ sơ tổng hợp/giả lập, không chứa dữ liệu cá nhân; đo thời gian, số mục bị đánh dấu sai và số lỗi bị bỏ sót. Chỉ thử OCR trong môi trường được tổ chức phê duyệt, với nhân viên kiểm tra từng cảnh báo cạnh tài liệu gốc. Không kết nối Core Banking, không tự gửi yêu cầu khách hàng, không đưa ra quyết định tín dụng.

**Nếu Not Yet — cần kiểm chứng gì trước:** (1) Hỏi sâu một số trường hợp survey để xác nhận thời điểm phát hiện thiếu sót và nguyên nhân; đối chiếu thời gian với log nếu được phép; (2) xác nhận checklist/nguồn dữ liệu chuẩn và control point bắt buộc; (3) hỏi bộ phận có thẩm quyền về môi trường xử lý dữ liệu được phép; (4) thử nghiệm trên bộ tài liệu giả lập/đã khử định danh trước khi chọn công cụ.

**Nếu No-Go — nên làm gì thay AI:** Chuẩn hóa checklist theo loại hồ sơ, hướng dẫn chất lượng ảnh/tài liệu, gom các mục cần bổ sung thành một lần rà soát, làm rõ trạng thái và đầu mối xử lý; tiếp tục kiểm tra thủ công theo control point hiện hành.

**Ngưỡng dừng:** Dừng thử nghiệm ngay nếu phát hiện một lỗi thiếu/sai thông tin định danh hoặc nguồn thu lọt qua bước kiểm tra của nhân viên, nếu công cụ xử lý dữ liệu ngoài môi trường được phê duyệt, hoặc nếu chưa có người chịu trách nhiệm kiểm tra. Với bộ test, nếu độ chính xác trường cốt lõi thấp hơn ngưỡng nhóm đặt ở mục 7 hoặc thời gian xử lý không giảm so với checklist/Rule, không mở rộng OCR và quay về quy trình No AI/Rule.

---

## 9. Hạn chế và hướng tiếp theo

- Survey ở mục 3.2 có 8 câu trả lời; mẫu nhỏ và tự báo cáo nên không đại diện cho toàn bộ người làm nghiệp vụ. Chưa có log để xác nhận thời gian hoặc tần suất trên toàn bộ hồ sơ.
- Thời gian tiếp nhận được chọn theo khoảng: 4/8 chọn 30–45 phút, 3/8 chọn 15–30 phút, 1/8 chọn dưới 15 phút; không có cơ sở tính trung bình chính xác từ các khoảng này. Target 15–25 phút và ngưỡng eval vẫn là đề xuất, cần thử nghiệm.
- Research ở mục 3.3 là tài liệu về khả năng OCR/trích xuất tổng quát, không phải đánh giá nhà cung cấp cho ngân hàng; chưa xác minh hỗ trợ tiếng Việt, loại giấy tờ, độ chính xác, vùng lưu trữ, chi phí, bảo mật hoặc tích hợp Core Banking trong môi trường cụ thể.
- Hướng tiếp theo: hỏi sâu một số trường hợp survey để xác nhận khi nào và vì sao thiếu sót được phát hiện; xác nhận checklist và quyền dữ liệu với bộ phận nghiệp vụ/bảo mật/tuân thủ; xây bộ test giả lập có lỗi gài sẵn; đo thời gian trước/sau và thử checklist/Rule trước. Chỉ cân nhắc OCR nếu các bước trên cho thấy còn bottleneck và có phê duyệt phù hợp.

## 10. Tài liệu tham khảo

- Microsoft Learn, [Azure AI Document Intelligence overview](https://learn.microsoft.com/en-us/azure/ai-services/document-intelligence/overview?view=doc-intel-3.1.0) — OCR và trích xuất cấu trúc/trường từ tài liệu.
- Google Cloud, [Document AI processor list](https://docs.cloud.google.com/document-ai/docs/processors-list) — danh sách processor cho OCR và trích xuất.
- Amazon Web Services, [Analyzing Documents with Amazon Textract](https://docs.aws.amazon.com/textract/latest/dg/how-it-works-analyzing.html) — phân tích văn bản, biểu mẫu và bảng.
- VinUni AI20K, `docs/01-worksheet.md`, `CHECKPOINTS.md` — yêu cầu và hướng dẫn CP4–CP6 của bài lab.
