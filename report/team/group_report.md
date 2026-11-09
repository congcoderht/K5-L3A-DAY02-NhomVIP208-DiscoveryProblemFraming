# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: NhomVIP208
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu):
- Quyết định cuối: Go / Not Yet / No-Go

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
OUTCOME: Rút ngắn 50% thời gian tiếp nhận và sơ duyệt một bộ hồ sơ vay vốn cá nhân mà vẫn đảm bảo tính tuân thủ và chính xác
├── Opportunity A1: Cán bộ tín dụng mất nhiều thời gian mở từng file để rà soát đủ/thiếu danh mục giấy tờ
├── Opportunity A2: Tốn nhiều thời gian đối chiếu chéo số liệu giữa tài liệu giấy/ảnh (CCCD, sao kê, hợp đồng) với hệ thống Core Banking
└── Opportunity A3: Khách hàng thường xuyên bị yêu cầu bổ sung giấy tờ nhiều lần do nhân viên phát hiện thiếu sót rải rác
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- ✗ "Dùng OCR và AI Agent tự động thẩm định và duyệt hồ sơ vay" (Đây là solution công nghệ, vi phạm quy định tuân thủ ngân hàng)
- ✗ "Xây dựng cổng portal/chatbot cho khách hàng tra cứu trạng thái hồ sơ" (Đây là solution tính năng phần mềm)
- ✗ "Tự động gửi email đòi khách bổ sung giấy tờ" (Đây là feature/automation cụ thể)

### 2.4. Chấm điểm shortlist (1–5)

Nhóm chọn 3 candidate đại diện nổi bật nhất từ 15 bài toán:

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
| --------- | -------: | -----------: | -----------------: | -------------: | ----------: | -------------------------------------: | ---------------: | ---: |
| **Kiểm tra tính đầy đủ và nhất quán hồ sơ vay (#7 & #8)** | 5 | 5 | 5 | 5 | 4 | 5 | 5 | **34** |
| Bóc tách tài liệu kỹ thuật & đối thủ (#4) | 4 | 4 | 4 | 4 | 4 | 4 | 4 | 28 |
| Tự động tạo dự thảo báo cáo thẩm định (#9) | 4 | 3 | 4 | 4 | 2 | 4 | 3 | 24 |

**Candidate được chọn:** Kiểm tra tính đầy đủ và nhất quán dữ liệu hồ sơ vay vốn cá nhân (Gộp trọng tâm của #1, #7, #8 và #14).

**Vì sao chọn:** 
- Đây là "nỗi đau" lớn nhất trong nhóm, được 4/5 thành viên cùng đưa ra trong buổi pitch với cùng một pattern.
- Quy trình rõ ràng: hồ sơ vay vốn cá nhân luôn có bộ danh mục chuẩn (Checklist: Pháp lý, Nguồn thu, Tài sản bảo đảm).
- Đo lường được ngay: hiện tại mất trung bình 35–45 phút/bộ hồ sơ, hay bị trả về hoặc yêu cầu bổ sung nhiều lần.
- Hoàn toàn khả thi để so sánh rõ nét giữa 4 mức giải pháp: No AI (Checklist giấy) vs Rule (Script đối chiếu cứng) vs Workflow (Trích xuất OCR + đối chiếu thực thể + người duyệt) vs Agent (Tự động duyệt vay).

**Vì sao loại các candidate còn lại:**
- *Bóc tách tài liệu kỹ thuật (#4):* Pain có thật nhưng chỉ phục vụ cá nhân/bộ phận hẹp, không phải là pain tập trung của đa số thành viên nhóm.
- *Tự động tạo dự thảo báo cáo thẩm định (#9):* Đòi hỏi đánh giá năng lực tài chính và phê duyệt rủi ro mang tính chủ quan nghiệp vụ rất cao; khó xây dựng tiêu chí đánh giá (eval) chuẩn mực trong thời lượng buổi lab.

**Xử lý bất đồng (nếu có):** Linh ban đầu muốn bảo lưu bài toán Bóc tách tài liệu kỹ thuật (#4) vì bản thân đã chuẩn bị kỹ ở cá nhân. Tuy nhiên sau khi cả nhóm phân tích cây OST và bảng chấm điểm, Linh đồng thuận chuyển sang bài toán tín dụng vì đây là nghiệp vụ phổ biến, impact lớn cho doanh nghiệp và có nhiều dữ liệu mẫu để giả lập kiểm chứng hơn.

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|--:|---|---|---:|---:|---|
| 1 | Hồ sơ thường thiếu hoặc không nhất quán giấy tờ/thông tin đến mức gây thêm việc cho người tiếp nhận. | Value | 5 | 1 | Có — hỏi về các trường hợp gần đây và tần suất. |
| 2 | Thiếu sót thường chỉ được phát hiện sau lần kiểm tra đầu, dẫn đến liên hệ bổ sung hoặc hồ sơ phải quay lại bước trước. | Value | 5 | 1 | Có — lần gần nhất, số lượt bổ sung và hệ quả. |
| 3 | Checklist theo loại hồ sơ có thể giúp phát hiện thiếu giấy tờ sớm mà không làm bỏ qua điểm kiểm soát. | Usability | 4 | 1 | Sau — hỏi nhân viên đang dùng checklist nào và ngoại lệ nào checklist chưa bao quát. |
| 4 | Thông tin cần đối chiếu giữa tài liệu và Core Banking có thể được xác định rõ theo quy tắc nghiệp vụ. | Feasibility | 4 | 1 | Sau — hỏi trường dữ liệu, nguồn chuẩn và cách xử lý khi nguồn không khớp. |
| 5 | Dữ liệu hồ sơ có thể được xử lý trong công cụ được tổ chức cho phép mà vẫn đáp ứng yêu cầu bảo mật và tuân thủ. | Viability | 5 | 1 | Sau — cần xác nhận chính sách với người có thẩm quyền; không tải dữ liệu thật lên dịch vụ ngoài. |
| 6 | Checklist, quy tắc hoặc chức năng sẵn có có thể giảm vấn đề mà chưa cần AI. | Feasibility / Value | 4 | 1 | Có — hỏi về workaround và chức năng đang dùng. |

Giả định ưu tiên kiểm chứng: #1 và #2 (pain/tần suất/tác động) cùng #6 (giải pháp hiện có). Các pitch và mức độ đồng thuận trong nhóm là tín hiệu ban đầu, chưa thay thế bằng chứng từ người trực tiếp làm nghiệp vụ. Điểm bằng chứng hiện chấm thấp vì báo cáo chưa ghi nhận phỏng vấn, survey hoặc log độc lập; cập nhật sau khi thu thập dữ liệu.

### 3.2. Kiểm chứng

**Trạng thái:** Chưa ghi nhận kết quả phỏng vấn/survey/log trong tài liệu. Nhóm cần thực hiện phỏng vấn 2–3 nhân viên từng tiếp nhận hoặc thẩm định hồ sơ; nếu không tiếp cận được, khảo sát 5–10 người có trải nghiệm phù hợp. Không phỏng vấn thành viên nhóm thay cho người dùng quy trình.

**Câu hỏi phỏng vấn gợi ý (hỏi về lần đã xảy ra, không hỏi về ý tưởng AI):**

1. Lần gần nhất hồ sơ bị yêu cầu bổ sung là khi nào? Thiếu hoặc cần làm rõ nội dung gì?
2. Ở bước nào phát hiện thiếu sót? Hồ sơ đã được kiểm tra trước đó chưa?
3. Sau khi phát hiện, chuyện gì xảy ra tiếp theo? Có phải liên hệ lại hoặc chuyển hồ sơ về bước trước không?
4. Trường hợp đó làm tăng thêm bao nhiêu lượt trao đổi hoặc thời gian chờ? Anh/chị ước lượng dựa trên hồ sơ nào/kỳ nào?
5. Anh/chị hiện dùng checklist, quy tắc hoặc chức năng nào để kiểm tra? Cách đó còn vướng ở đâu?
6. Có trường hợp nào checklist phát hiện đủ ngay lần đầu, hoặc việc bổ sung không làm chậm đáng kể không? (tín hiệu phản bác)

Không ghi tên khách hàng, mã hồ sơ, số giấy tờ, thông tin tài chính hay dữ liệu nội bộ nhạy cảm vào báo cáo.

Interview snapshot (mỗi buổi phỏng vấn một bảng, hoặc đặt file trong `report/assets/cp4-interview-snapshot-N.md`):

| Trường                                            | Nội dung |
| ------------------------------------------------- | -------- |
| Người được hỏi (vai trò, không ghi tên thật)      | Chờ phỏng vấn; điền vai trò sau khi thực hiện. |
| Câu nói đáng nhớ nhất (nguyên văn)                | Chưa có dữ liệu. |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Chưa có dữ liệu. |
| Hiện đang xử lý bằng cách nào (workaround)?       | Chưa có dữ liệu. |
| Mất bao lâu, bao lần?                             | Chưa có dữ liệu; hỏi về một trường hợp cụ thể. |
| Insight / opportunity rút ra                      | Chưa kết luận; cập nhật sau phỏng vấn. |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| Phỏng vấn nhân viên tiếp nhận/thẩm định hoặc survey người có trải nghiệm | Chưa thực hiện; mục tiêu 2–3 phỏng vấn hoặc 5–10 phản hồi survey | Chưa có dữ liệu; điền sau khi thu thập | Chưa có dữ liệu; ghi cả trường hợp ít/không gặp vấn đề |
| Log/timestamp/checklist đã ẩn danh và được phép sử dụng (nếu có) | Chưa tiếp cận | Chưa có dữ liệu | Chưa có dữ liệu |

**Nhóm đã sửa problem thế nào sau kiểm chứng:** Chưa thể kết luận trước khi phỏng vấn/survey hoặc xem dữ liệu được phép. Sau khi có kết quả, ghi điều chỉnh actor, bước nghẽn, phạm vi hồ sơ và metric; nếu bằng chứng yếu thì thu hẹp hoặc đổi candidate.

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
| 2 | Nhân viên tiếp nhận / tín dụng | Từng tài liệu trong hồ sơ và checklist nghiệp vụ | Danh sách tài liệu đã kiểm tra, các mục nghi thiếu/không hợp lệ | Khoảng 10-20 phút/hồ sơ | Phải mở và xem từng tài liệu riêng lẻ |
| 3 | Nhân viên tín dụng | Tài liệu đã kiểm tra và dữ liệu trên Core Banking | Kết quả đối chiếu thông tin khách hàng/khoản vay | Khoảng 10-20 phút/hồ sơ | Sai lệch nhỏ có thể bị bỏ sót khi phải đối chiếu thủ công |
| 4 | Nhân viên tiếp nhận / khách hàng | Danh sách thiếu, sai hoặc cần làm rõ | Yêu cầu bổ sung/chỉnh sửa và hồ sơ được gửi lại | Thường lặp lại 1 hoặc nhiều lần | Các thiếu sót được phát hiện rải rác, khách hàng phải bổ sung nhiều lần |
| 5 | Nhân viên tín dụng / thẩm định | Hồ sơ đã bổ sung và kết quả đối chiếu | Hồ sơ được xác nhận để chuyển sang thẩm định | Tổng cộng ước tính 35-45 phút/hồ sơ, chưa tính thời gian chờ bổ sung | Nếu vẫn còn sai lệch, hồ sơ quay lại bước 3 hoặc 4 |

**Bottleneck chính:** Nhân viên phải kiểm tra thủ công từng file, đối chiếu thông tin giữa nhiều nguồn và phát hiện thiếu sót theo từng lần. Vì vậy, thiếu sót có thể chỉ được phát hiện sau khi hồ sơ đã đi qua một bước, dẫn đến liên hệ bổ sung nhiều lần, tăng thời gian xử lý và nguy cơ bỏ sót sai lệch.

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
| Tổng thời gian | Khoảng 35-45 phút/hồ sơ, chưa tính thời gian chờ khách hàng bổ sung | Khoảng 15-25 phút/hồ sơ nếu tài liệu đọc được và dữ liệu khớp; hồ sơ ngoại lệ có thể lâu hơn | Cần đo lại bằng hồ sơ giả lập hoặc log thực tế; đây là target kỳ vọng, chưa phải số liệu đã xác nhận |
| Số bước thủ công | Khoảng 4-5 bước: mở file, kiểm tra checklist, đối chiếu Core Banking, lập yêu cầu bổ sung và kiểm tra lại | Khoảng 1-2 bước: xem cảnh báo/tài liệu gốc và xác nhận hoặc sửa kết quả trước khi chuyển thẩm định | Rule và AI chỉ hỗ trợ sàng lọc; quyết định nghiệp vụ vẫn do con người thực hiện |
| Bottleneck chính | Mở và kiểm tra từng tài liệu; đối chiếu thủ công giữa nhiều nguồn; phát hiện thiếu sót rải rác nên phải yêu cầu bổ sung nhiều lần | Xử lý các trường hợp AI trích xuất không chắc chắn, dữ liệu không khớp hoặc checklist có ngoại lệ | Cần thiết kế hàng đợi HITL và hiển thị bằng chứng từ tài liệu gốc để người dùng kiểm tra nhanh |
| Rủi ro mới phát sinh | Bỏ sót thiếu/sai lệch, xử lý lại nhiều lần và kéo dài thời gian chờ | OCR/trích xuất sai, cảnh báo nhầm hoặc bỏ sót; rò rỉ dữ liệu hồ sơ; người dùng quá tin vào kết quả tự động | Giảm thiểu bằng ngưỡng độ tin cậy, đối chiếu tài liệu gốc, log/audit, phân quyền dữ liệu và bắt buộc HITL trước khi chuyển thẩm định |

---

## 5. Problem Statement v0 (CP5)
 
| Trường | Nội dung |
| ------ | -------- |
| **Actor** | Nhân viên tiếp nhận / Credit Officer xử lý hồ sơ vay vốn cá nhân. Khách hàng vay vốn là bên chịu ảnh hưởng khi bị yêu cầu bổ sung nhiều lần. |
| **Quy trình** | Từ lúc nhận bộ hồ sơ của khách đến lúc chuyển sang thẩm định: mở từng tài liệu, đối chiếu checklist đủ/thiếu/hợp lệ, đối chiếu thông tin giữa tài liệu và Core Banking, liên hệ khách bổ sung rồi kiểm tra lại. |
| **Bottleneck** | Kiểm tra thủ công từng file (khoảng 10–20 phút/hồ sơ) và đối chiếu thủ công giữa tài liệu với Core Banking (khoảng 10–20 phút/hồ sơ). Thiếu sót được phát hiện rải rác qua nhiều lần kiểm tra nên hồ sơ phải quay lại bước trước, sai lệch nhỏ dễ bị bỏ sót. |
| **Impact** | Mỗi hồ sơ tốn khoảng 35–45 phút kiểm tra (chưa tính thời gian chờ khách bổ sung); khách bị yêu cầu bổ sung 1 hoặc nhiều lần; sai lệch bị bỏ sót có thể ảnh hưởng chất lượng thẩm định. Các số liệu này là **ước tính từ pitch (CP3), chưa được kiểm chứng ở CP4**. |
| **Success Metric** (baseline → target, cách đo) | **Chính:** thời gian kiểm tra sơ bộ/hồ sơ, baseline 35–45' (ước tính) → target ≤ 25' (kỳ vọng 15–25'; mức 20' tương ứng outcome giảm 50% ở OST). Cách đo: bấm giờ 5–10 hồ sơ giả lập/đã ẩn danh, trước và sau, cùng một người thực hiện. **Phụ:** số lượt yêu cầu bổ sung/hồ sơ, baseline chưa có (đếm trên 5–10 hồ sơ gần nhất hoặc hồ sơ giả lập) → giảm xuống tối đa 1 lượt. **Guardrail:** tỉ lệ bỏ sót thiếu/sai lệch trên bộ hồ sơ đã gài lỗi sẵn không cao hơn cách làm thủ công hiện tại. |
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

Bài của nhóm nằm ở ô:

Vì sao:

### 6.2. So sánh 4 mức

| Mức                       | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
| ------------------------- | -------------------------- | ---------- | ------ | ----- |
| **No AI** (sửa quy trình) |                            |            |        |       |
| **Rule**                  |                            |            |        |       |
| **Workflow**              |                            |            |        |       |
| **Agent**                 |                            |            |        |       |

**Mức chọn:**

**Vì sao không chọn mức đơn giản hơn:**

### 6.3. AI Canvas rút gọn

| Thành phần                                                        | Nội dung |
| ----------------------------------------------------------------- | -------- |
| **Prediction** — AI dự đoán / tạo ra gì?                          |          |
| **Judgment** — con người cân nhắc, quyết định gì?                 |          |
| **Action** — hành động cuối cùng là gì, ai làm?                   |          |
| **Outcome** — đo kết quả bằng gì?                                 |          |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? |          |
| **Feedback** — lấy phản hồi ở đâu để cải thiện?                   |          |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng:
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào:

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường                                          | Nội dung                        |
| ----------------------------------------------- | ------------------------------- |
| **Actor**                                       |                                 |
| **Quy trình**                                   |                                 |
| **Bottleneck**                                  |                                 |
| **Impact**                                      |                                 |
| **Success Metric** (baseline → target, cách đo) |                                 |
| **Boundary**                                    |                                 |
| **AI intervention point**                       |                                 |
| **Mức chọn**                                    | No AI / Rule / Workflow / Agent |
| **Rủi ro & người kiểm tra**                     |                                 |

**Thay đổi so với v0 và lý do:**

| Trường | v0  | v1  | Vì sao đổi |
| ------ | --- | --- | ---------- |
|        |     |     |            |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

|   # | Tiêu chí | Đạt khi | Không đạt khi |
| --: | -------- | ------- | ------------- |
|   1 |          |         |               |
|   2 |          |         |               |
|   3 |          |         |               |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro          | Câu hỏi                                                           | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
| --------------- | ----------------------------------------------------------------- | ----------------------------------------------------- | ------------------ |
| **Value**       | Người dùng có thật sự cần và sẽ dùng không?                       |                                                       |                    |
| **Usability**   | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? |                                                       |                    |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không?                     |                                                       |                    |
| **Viability**   | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành?     |                                                       |                    |

### 8.2. Kết luận

**Quyết định:** Go / Not Yet / No-Go

**Lý do:**

**Nếu Go — pilot nhỏ nhất:**

**Nếu Not Yet — cần kiểm chứng gì trước:**

**Nếu No-Go — nên làm gì thay AI:**

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):

---

## 9. Hạn chế và hướng tiếp theo

-

## 10. Tài liệu tham khảo

-
