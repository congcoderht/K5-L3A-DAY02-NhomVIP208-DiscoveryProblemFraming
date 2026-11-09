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
|   4 | Lê Quang Linh     | Khi thẩm định tài liệu kỹ thuật/báo cáo đối thủ (15–20 trang), tôi muốn bóc tách nhanh thông số và chi phí, để lập bảng so sánh đối chuẩn (benchmarking) phục vụ họp chiến lược.                                       | Product Owner / Business Analyst / Solution Engineer                                                           | Bước bóc tách bảng giá/thông số kỹ thuật vào bảng tính (90 phút) và đối chiếu chéo tiêu chí kỹ thuật tương đương (45 phút).                                          | "Nếu tài liệu của các bên dùng thuật ngữ chuyên môn khác nhau hoặc cấu trúc giá dị biệt (bên tính theo API call, bên tính theo user/tháng), hệ thống chuẩn hóa thế nào để số liệu không bị bóp méo?" |(Đoàn Văn Tú)
|   5 | Lê Quang Linh     | Khi đối soát dữ liệu xuất từ CRM/database, tôi muốn rà soát và làm sạch các trường trùng lặp, sai định dạng số ĐT/email, để nạp vào hệ thống marketing mà không bị lỗi bounce.                                         | Data Ops / Sales Operations                                                                                    | Bước rà soát bằng mắt các lỗi font, số ĐT, email (60 phút) và sửa thủ công từng ô lỗi (30 phút).                                                                     | "Tại sao không dùng bộ lọc Regex hoặc validation ngay tại form nhập liệu CRM để chặn lỗi từ đầu mà lại cần tới một quy trình can thiệp phức tạp?"                                                     | (Đoàn Văn Tú)
|   6 | Lê Quang Linh     | Khi kết thúc cuộc họp điều hành/khách hàng, tôi muốn trích xuất chính xác các quyết định và đầu việc được giao kèm người phụ trách, để gửi biên bản họp (meeting recap) trong ngày.                                    | Project Manager / Thư ký cuộc họp                                                                              | Bước nghe tua lại các đoạn thảo luận cam kết phức tạp (40 phút) và tổng hợp danh sách việc/deadline (25 phút).                                                       | "Văn phong nói chuyện lúc họp thường nhảy ý và không có cấu trúc cố định; nếu bóc tách tự động bị ảo giác (hallucination) rồi gán nhầm trách nhiệm/deadline cho người khác thì rủi ro xử lý ra sao?" |(Đoàn Văn Tú)
|   7 | Nguyễn Trường Duy | Khi tiếp nhận một bộ hồ sơ vay vốn cá nhân, tôi muốn nhanh chóng kiểm tra tính đầy đủ và hợp lệ của các tài liệu, để đảm bảo hồ sơ đáp ứng yêu cầu trước khi tiến hành thẩm định.                                      | Credit Officer trực tiếp tiếp nhận và kiểm tra hồ sơ vay vốn cá nhân.                                          | Phải mở và kiểm tra từng tài liệu riêng lẻ, mất thời gian khi hồ sơ có nhiều giấy tờ hoặc tài liệu không được sắp xếp thống nhất.                                    | “Lần gần nhất hồ sơ bị thiếu hoặc không hợp lệ là khi nào, và việc đó khiến hồ sơ bị chậm hoặc phải xử lý lại ra sao?” (Người hỏi: điền sau buổi pitch.) |
|   8 | Nguyễn Trường Duy | Khi thẩm định hồ sơ vay vốn, tôi muốn nhanh chóng phát hiện những thông tin không nhất quán giữa các tài liệu và dữ liệu Core Banking, để hạn chế sai sót trong quá trình đánh giá khách hàng và khoản vay.            | Credit Officer chịu trách nhiệm kiểm tra, đối chiếu và xác minh thông tin khách hàng.                          | Phải đối chiếu thủ công giữa nhiều tài liệu và hệ thống khác nhau. Những sai lệch nhỏ có thể bị bỏ sót khi số lượng hồ sơ lớn.                                       | “Những loại sai lệch nào thường gặp, và hiện có bước kiểm tra nào để phát hiện chúng trước khi ảnh hưởng đến kết quả thẩm định?” (Người hỏi: điền sau buổi pitch.) |
|   9 | Nguyễn Trường Duy | Khi hoàn tất quá trình thẩm định hồ sơ vay vốn, tôi muốn tự động tổng hợp thông tin và tạo bản dự thảo báo cáo thẩm định theo biểu mẫu chuẩn, để tiết kiệm thời gian lập báo cáo và chuyển cấp có thẩm quyền phê duyệt | Credit Officer chịu trách nhiệm phân tích hồ sơ, đưa ra nhận xét và lập báo cáo thẩm định trình cấp phê duyệt. | Phải tổng hợp thông tin từ nhiều nguồn và tự viết nội dung nhận xét, đánh giá theo biểu mẫu. Đây là công đoạn tốn thời gian và đòi hỏi khả năng phân tích nghiệp vụ. | “Phần nào trong việc lập báo cáo hiện mất nhiều thời gian nhất, và có mẫu hoặc quy tắc sẵn có nào giúp giảm công việc mà vẫn bảo đảm người có thẩm quyền kiểm tra được?” (Người hỏi: điền sau buổi pitch.) |
|  10 | Đoàn Văn Tú       | Khi nhận nhiều giấy tờ, tôi muốn biết bản nào mới nhất và còn thiếu gì để tránh nhầm lẫn.                                                                                                                              | Nhân viên tiếp nhận hồ sơ                                                                                      | Tìm bản giấy tờ mới nhất và rà soát tài liệu thiếu mất 10 phút/lượt kiểm tra.                                                                                        | Những loại giấy tờ mới đã đáp ứng đủ yêu cầu chưa?                                                                                                                  |
|  11 | Đoàn Văn Tú       | Khi cần biết thông tin hồ sơ vay, tôi muốn tự tìm được thông tin để không phải gọi hỏi nhiều lần.                                                                                                                      | Khách hàng có hồ sơ vay                                                                                        | Khách hàng phụ thuộc vào nhân viên; nhân viên phải hỏi bộ phận phụ trách 1–2 lần/hồ sơ, mỗi lần 3 phút.                                                              | Nếu thông tin chưa được cập nhật, trang tra cứu có thực sự giúp khách hàng giảm gọi hỏi không?                                                                                                       |
|  12 | Đoàn Văn Tú       | Khi muốn tất toán trước hạn, tôi muốn biết thủ tục và số tiền cần thanh toán để chuẩn bị đầy đủ.                                                                                                                       | Khách hàng muốn tất toán trước hạn                                                                             | Phải liên hệ 1–2 lần để xác nhận thủ tục và số tiền, mỗi cuộc trao đổi 15 phút.                                                                                      | Khách hàng hỏi lại vì hướng dẫn chưa rõ hay vì thay đổi ngày tất toán làm số tiền cần trả thay đổi?                                                                                                  |
|  13 | Lê Anh Quân       | Khi rà soát một khoản vay cần theo dõi hoặc thu hồi nợ, tôi muốn nắm được lịch sử xử lý và các lần liên hệ trước đó, để xác định chính xác tình trạng khoản vay.                                                       | Cán bộ quản lý và thu hồi nợ.                                                                                  | Tra cứu lịch sử liên hệ/xử lý cũ qua các file rời rạc và biên bản bàn giao, ước tính 20–30 phút/khoản vay.                                                           | "Nếu hệ thống quản lý nợ đã có ô lưu lịch sử/ghi chú, vấn đề thực sự nằm ở việc thiếu dữ liệu, dữ liệu phân tán hay thao tác tìm kiếm chưa hiệu quả?"                                                |
|  14 | Lê Anh Quân       | Khi tiếp nhận hồ sơ vay vốn, tôi muốn xác định sớm giấy tờ hoặc thông tin còn thiếu, để hạn chế việc yêu cầu khách hàng bổ sung nhiều lần.                                                                             | Nhân viên tín dụng phụ trách tiếp nhận hồ sơ; khách hàng vay vốn.                                              | Kiểm tra tính đầy đủ danh mục giấy tờ và đối chiếu thông tin thiếu, ước tính 30–45 phút/hồ sơ.                                                                       | "Việc hồ sơ bị thiếu là do khách hàng không nắm rõ checklist hay do nghiệp vụ tín dụng quá phức tạp, và AI sẽ đọc hiểu tính hợp lệ của hồ sơ giấy thế nào?"                                          |
|  15 | Lê Anh Quân       | Khi thực hiện nghiệp vụ tín dụng, tôi muốn tìm đúng quy định và biểu mẫu đang có hiệu lực, để tránh sử dụng tài liệu không phù hợp và phải chỉnh sửa hồ sơ.                                                            | Nhân viên tín dụng và cán bộ nghiệp vụ.                                                                        | Tìm kiếm quy định và kiểm tra phiên bản hiệu lực trên các kho tài liệu phân tán, ước tính 20–30 phút/lần.                                                            | "Các quy định và biểu mẫu tín dụng thay đổi thường xuyên, làm thế nào để đảm bảo hệ thống luôn trích xuất đúng phiên bản mới nhất thay vì tài liệu cũ đã hết hiệu lực?"                              |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
| ------- | ------------- | ------------- |
| A       |               |               |
| B       |               |               |
| C       |               |               |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME:
├── Opportunity A:
├── Opportunity B:
└── Opportunity C:
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

-

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
| --------- | -------: | -----------: | -----------------: | -------------: | ----------: | -------------------------------------: | ---------------: | ---: |
|           |          |              |                    |                |             |                                        |                  |      |
|           |          |              |                    |                |             |                                        |                  |      |
|           |          |              |                    |                |             |                                        |                  |      |

**Candidate được chọn:**

**Vì sao chọn:**

**Vì sao loại các candidate còn lại:**

**Xử lý bất đồng (nếu có):**

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

|   # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
| --: | -------- | -------------------------------------------------- | ---------------: | ---------------------: | ----------------- |
|   1 |          |                                                    |                  |                        |                   |
|   2 |          |                                                    |                  |                        |                   |
|   3 |          |                                                    |                  |                        |                   |
|   4 |          |                                                    |                  |                        |                   |
|   5 |          |                                                    |                  |                        |                   |
|   6 |          |                                                    |                  |                        |                   |

_Điền 4–6 giả định; xóa dòng thừa._

Giả định nhóm kiểm chứng trong buổi này:

### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn / Survey / Log, ticket, review

Interview snapshot (mỗi buổi phỏng vấn một bảng, hoặc đặt file trong `report/assets/cp4-interview-snapshot-N.md`):

| Trường                                            | Nội dung |
| ------------------------------------------------- | -------- |
| Người được hỏi (vai trò, không ghi tên thật)      |          |
| Câu nói đáng nhớ nhất (nguyên văn)                |          |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? |          |
| Hiện đang xử lý bằng cách nào (workaround)?       |          |
| Mất bao lâu, bao lần?                             |          |
| Insight / opportunity rút ra                      |          |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
| ----- | ----------------: | ----------------- | ----------------- |
|       |                   |                   |                   |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
| ------------------------ | ---- | ------------------------------ | --------- | --------------------- | ---------------- |
|                          |      |                                |           |                       |                  |
|                          |      |                                |           |                       |                  |
|                          |      |                                |           |                       |                  |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text

```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
| ---: | ----- | ----- | ------ | -------------------- | ------- |
|    1 |       |       |        |                      |         |
|    2 |       |       |        |                      |         |
|    3 |       |       |        |                      |         |
|    4 |       |       |        |                      |         |
|    5 |       |       |        |                      |         |

**Bottleneck chính:**

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text

```

### 4.3. Before / after

| Chỉ số               | Trước | Sau (kỳ vọng) | Ghi chú |
| -------------------- | ----: | ------------: | ------- |
| Số bước              |       |               |         |
| Tổng thời gian       |       |               |         |
| Số bước thủ công     |       |               |         |
| Bottleneck chính     |       |               |         |
| Rủi ro mới phát sinh |       |               |         |

---

## 5. Problem Statement v0 (CP5)

| Trường                                                                     | Nội dung |
| -------------------------------------------------------------------------- | -------- |
| **Actor**                                                                  |          |
| **Quy trình**                                                              |          |
| **Bottleneck**                                                             |          |
| **Impact**                                                                 |          |
| **Success Metric** (baseline → target, cách đo)                            |          |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) |          |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

- ***

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
