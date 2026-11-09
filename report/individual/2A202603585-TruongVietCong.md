# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Trương Việt Công
- MSSV: 2A202603585
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: NhomVIP208
- Link repo nhóm: https://github.com/congcoderht/K5-L3A-DAY02-NhomVIP208-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi tiếp nhận hồ sơ vay, tôi muốn nhận biết sớm giấy tờ hoặc thông tin còn thiếu để hạn chế yêu cầu khách hàng bổ sung nhiều lần. | Nhân viên tiếp nhận; khách hàng; nhân viên thẩm định | 20–30% hồ sơ cần bổ sung ít nhất một lần, thường 1–2 lượt. |
| 2 | Tốn thời gian | Khi hồ sơ đi qua các bước thẩm định và phê duyệt, tôi muốn biết hồ sơ đang chờ ở đâu và ai xử lý tiếp để giảm thời gian chờ không rõ nguyên nhân. | Nhân viên xử lý; quản lý quy trình; khách hàng | Tra cứu trạng thái mất 5–10 phút/lần; cần xem thêm thời gian chờ theo bước, số hồ sơ tồn và tần suất tra cứu. |
| 3 | Cần đọc, tổng hợp nhiều thông tin | Khi rà soát hồ sơ, tôi muốn đối chiếu thông tin giữa biểu mẫu và giấy tờ liên quan để phát hiện mục thiếu hoặc không nhất quán trước khi chuyển bước. | Nhân viên thẩm định; nhân viên kiểm soát | Rà soát ban đầu mất 20–40 phút/hồ sơ; cần xem thêm số trường hợp phải sửa/xác minh. Không dùng hồ sơ định danh. |
| 4 | Lặp lại / pain từ người khác | Khi chuẩn bị giải ngân cho hồ sơ đã được duyệt, tôi muốn xác nhận các điều kiện và điểm kiểm soát đã hoàn tất để tránh hồ sơ bị trả lại hoặc xử lý lại. | Nhân viên giải ngân; bộ phận phê duyệt/kiểm soát; khách hàng | 5–10% hồ sơ bị trả lại để hoàn tất/đối chiếu điều kiện; cần ghi nhận lý do và thời gian xử lý lại. |
| 5 | Pain từ người khác | Khi tiếp nhận hồ sơ thu hồi nợ, tôi muốn xem lịch sử xử lý và các cam kết đã ghi nhận để tiếp tục làm việc nhất quán, không phải hỏi lại nhiều nơi. | Nhân viên thu hồi nợ; quản lý hồ sơ; khách hàng | Tìm lịch sử hoặc hỏi bàn giao mất 5–15 phút/hồ sơ; cần ghi nhận số lần hỏi lại và tỷ lệ thiếu ghi chú. |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- AI được dùng để gợi ý các hướng vấn đề quanh tiếp nhận, thẩm định, phê duyệt, giải ngân và thu hồi nợ. Tôi giữ các hướng có thể mô tả thành quy trình và đo bằng thời gian, tỷ lệ bổ sung, số lần chuyển hoặc lỗi kiểm soát. Đây mới là danh sách giả thuyết; cần hỏi người làm nghiệp vụ và kiểm tra bằng chứng được phép trước khi xem là vấn đề đã xác nhận. Không đưa dữ liệu định danh khách hàng hoặc thông tin tín dụng vào công cụ AI.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Hồ sơ vay phải bổ sung giấy tờ/thông tin nhiều lần | Có điểm bắt đầu và kết thúc tương đối rõ; có thể khảo sát số lượt bổ sung và thời gian chờ; liên quan trực tiếp tới trải nghiệm khách hàng và thời gian xử lý. | Chưa biết tỷ lệ thực tế, nguyên nhân thiếu thông tin, và phần nào do khách hàng/phần nào do biểu mẫu hoặc quy trình. |
| 2 | Khó theo dõi hồ sơ đang chờ ở bước duyệt nào và ai xử lý tiếp | Có thể vẽ các bước/handoff và đo thời gian chờ theo timestamp; phù hợp để xem bottleneck nằm ở bước nào. | Chưa biết hệ thống Core Banking đã có trạng thái/cảnh báo đáp ứng nhu cầu chưa; cần được người có quyền mô tả hoặc xem dữ liệu đã ẩn danh. |
| 3 | Thông tin phải đối chiếu lặp lại giữa các bước kiểm tra | Có thể xác định trường thông tin/bước kiểm soát lặp, thời gian rà soát và lỗi phát hiện; có phương án cải tiến quy trình không cần AI để so sánh. | Chưa rõ việc lặp là kiểm soát bắt buộc hay thao tác trùng có thể giảm; không được đề xuất bỏ control point khi chưa có thẩm quyền. |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi tiếp nhận hồ sơ vay, tôi muốn nhận biết sớm giấy tờ hoặc thông tin còn thiếu để hạn chế yêu cầu bổ sung nhiều lần và giúp hồ sơ được chuyển bước đầy đủ. |
| Actor | Nhân viên tiếp nhận hồ sơ; khách hàng là bên cung cấp thông tin. |
| Thời điểm / bối cảnh | Khi khách hàng nộp hồ sơ và trước khi hồ sơ được chuyển sang thẩm định. |
| Quy trình hiện tại (3–7 bước) | 1) Nhận hồ sơ; 2) kiểm tra danh mục giấy tờ/thông tin; 3) ghi nhận mục thiếu hoặc cần làm rõ; 4) liên hệ yêu cầu bổ sung; 5) nhận và kiểm tra phần bổ sung; 6) chuyển hồ sơ khi đủ điều kiện tiếp nhận. Thứ tự thực tế cần xác minh với nhân viên. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Kiểm tra tính đầy đủ và phát hiện mục thiếu ở bước 2–3; 10–20 phút rà soát ban đầu/hồ sơ. |
| Impact (nếu không giải thì sao) | Có thể phát sinh thêm lượt liên hệ, thời gian chờ, thao tác kiểm tra lại và chậm chuyển hồ sơ. Mức độ ảnh hưởng cần xác minh bằng dữ liệu hoặc phỏng vấn. |
| Success metric (baseline → target) | Tỷ lệ hồ sơ phải bổ sung 25% → mục tiêu 18%; đo bằng số hồ sơ có ít nhất một yêu cầu bổ sung / tổng hồ sơ tiếp nhận. Metric phụ: số lượt bổ sung trung bình/hồ sơ. |
| Phương án không dùng AI | Làm rõ checklist theo loại hồ sơ, hướng dẫn cách kiểm tra, ghi rõ lý do thiếu và đầu mối theo dõi; không tự ý bỏ hoặc nới lỏng điều kiện kiểm soát. |
| Giả thuyết về AI (nếu có) | Chưa giả định cần AI. Chỉ khảo sát sau khi hiểu quy trình và chính sách dữ liệu; AI không quyết định điều kiện tín dụng hay thay thế kiểm tra nghiệp vụ. |
| Cảm nhận nhanh | Chưa biết; ưu tiên kiểm tra No AI/Rule trước. |

Quy trình nháp hiện tại:

```text
Nhận hồ sơ
  → Kiểm tra danh mục giấy tờ/thông tin (10–20 phút)
  → Ghi nhận mục thiếu/cần làm rõ (5–10 phút)
  → Liên hệ khách hàng yêu cầu bổ sung (chờ phản hồi 1–3 ngày)
  → Nhận và kiểm tra phần bổ sung (10–20 phút)
  → Hồ sơ đủ điều kiện tiếp nhận thì chuyển thẩm định

Bottleneck giả thuyết: kiểm tra tính đầy đủ và vòng yêu cầu bổ sung.
Tần suất và thời gian cần cập nhật theo quy trình bạn khảo sát.
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi hồ sơ đang qua các bước thẩm định/phê duyệt, tôi muốn biết hồ sơ đang chờ ở đâu và ai phụ trách tiếp theo để theo dõi việc bàn giao kịp thời. |
| Actor | Nhân viên xử lý hồ sơ hoặc quản lý theo dõi tiến độ. |
| Thời điểm / bối cảnh | Sau khi hồ sơ được tiếp nhận và trong các lần chuyển giữa các bước kiểm tra/phê duyệt. |
| Quy trình hiện tại (3–7 bước) | 1) Hoàn tất bước hiện tại; 2) cập nhật trạng thái; 3) chuyển hồ sơ/đầu việc tới bước hoặc người tiếp theo; 4) người nhận tiếp nhận và xử lý; 5) nếu chờ lâu, nhân viên tra cứu hoặc liên hệ để hỏi trạng thái. Cần xác minh luồng thực tế. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Khoảng chờ giữa lúc chuyển giao và lúc bước tiếp theo được nhận/xử lý; 2–8 giờ làm việc/lần bàn giao. |
| Impact (nếu không giải thì sao) | Có thể khó phân biệt hồ sơ đang được xử lý với hồ sơ bị tồn, phát sinh việc hỏi trạng thái và kéo dài thời gian hoàn tất. Cần kiểm chứng, không suy diễn ảnh hưởng tới quyết định cấp tín dụng. |
| Success metric (baseline → target) | Thời gian trung vị chờ bàn giao 4 giờ làm việc → mục tiêu 3 giờ; đo từ timestamp bàn giao tới timestamp tiếp nhận. |
| Phương án không dùng AI | Chuẩn hóa trạng thái, người/bộ phận nhận, thời điểm bàn giao và quy tắc nhắc việc; dùng chức năng sẵn có nếu được phép. |
| Giả thuyết về AI (nếu có) | Chưa có lý do để dùng AI; trạng thái và thời gian chờ có thể xử lý bằng quy tắc/nhắc việc nếu dữ liệu hệ thống đủ rõ. |
| Cảm nhận nhanh | Rule hoặc No AI; cần kiểm tra hệ thống hiện tại trước. |

Quy trình nháp hiện tại:

```text
Hoàn tất bước hiện tại
  → Cập nhật trạng thái và thời điểm bàn giao (2–5 phút)
  → Chuyển hồ sơ/đầu việc tới người hoặc bộ phận tiếp theo
  → Người nhận tiếp nhận và xử lý (chờ 2–8 giờ làm việc)
  → Nếu quá ngưỡng: nhân viên kiểm tra trạng thái/đầu mối (5–10 phút)

Bottleneck giả thuyết: khoảng chờ hoặc thiếu cập nhật tại điểm bàn giao.
Các mốc thời gian cần lấy từ quy trình/log được phép, hiện chưa có baseline.
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi rà soát hồ sơ vay, tôi muốn biết trường thông tin nào đã được kiểm tra và kết quả ra sao để tránh đối chiếu trùng không cần thiết mà vẫn giữ đủ các điểm kiểm soát bắt buộc. |
| Actor | Nhân viên thẩm định/kiểm soát; quản lý quy trình. |
| Thời điểm / bối cảnh | Khi hồ sơ được rà soát ở một hoặc nhiều bước trước khi ra quyết định theo thẩm quyền. |
| Quy trình hiện tại (3–7 bước) | 1) Nhận hồ sơ và kết quả kiểm tra trước; 2) đối chiếu trường thông tin theo checklist; 3) ghi nhận kết quả/ngoại lệ; 4) yêu cầu làm rõ nếu cần; 5) chuyển bước theo quy trình và thẩm quyền. Cần xác minh liệu các bước có lặp và vì sao. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Đối chiếu lại các trường đã được kiểm tra hoặc tìm kết quả kiểm tra trước; 10–20 phút rà soát/đối chiếu. Không mặc định kiểm tra lặp là lãng phí vì có thể là control point bắt buộc. |
| Impact (nếu không giải thì sao) | Có thể tốn thêm thời gian rà soát; ngược lại, giảm kiểm tra thiếu kiểm soát có thể tạo rủi ro nghiêm trọng. Chỉ khảo sát cơ hội giảm thao tác trùng, không đề xuất bỏ kiểm soát. |
| Success metric (baseline → target) | Giảm 15% thời gian tìm/đối chiếu lại kết quả; đo bằng thời gian quan sát trên mẫu hồ sơ. Điều kiện bắt buộc: không giảm tỷ lệ hoàn thành control point. |
| Phương án không dùng AI | Làm rõ checklist, ghi nhận kết quả kiểm tra có truy vết và phân định trách nhiệm giữa các bước; chỉ thay đổi khi người có thẩm quyền phê duyệt. |
| Giả thuyết về AI (nếu có) | Không dùng AI để đánh giá khả năng trả nợ, đề xuất hạn mức hoặc phê duyệt. Trước mắt khảo sát checklist/quy tắc và cách lưu kết quả; có thể không cần AI. |
| Cảm nhận nhanh | No AI/Rule; cần xác minh tính bắt buộc của từng control point. |

Quy trình nháp hiện tại:

```text
Nhận hồ sơ cùng kết quả kiểm tra trước (3–5 phút)
  → Đối chiếu thông tin theo checklist (10–20 phút)
  → Ghi nhận kết quả và ngoại lệ (5–10 phút)
  → Nếu cần, yêu cầu làm rõ/xác minh (thời gian chờ: cần đo)
  → Chuyển bước theo quy trình và thẩm quyền

Bottleneck giả thuyết: tìm/đối chiếu lại kết quả đã có.
Cần xác minh bước nào là kiểm soát bắt buộc; không được lược bỏ control point.
```

### Card muốn pitch nhất

- Card số: 1 — Hồ sơ phải bổ sung giấy tờ/thông tin nhiều lần.
- Vì sao: Quy trình có thể quan sát từ tiếp nhận đến khi đủ hồ sơ; có các chỉ số kiểm chứng được như số lượt bổ sung, tỷ lệ hồ sơ phải bổ sung và thời gian chờ. Đây là candidate ưu tiên để pitch, chưa phải vấn đề đã được xác nhận.
- Câu hỏi muốn nhóm phản biện: Nguyên nhân chính có thật sự nằm ở bước kiểm tra ban đầu, hay do yêu cầu hồ sơ/phản hồi từ khách hàng thay đổi? Bằng chứng nào giúp phân biệt hai nguyên nhân?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Chưa có baseline; không thể ghi thời gian/tỷ lệ như sự thật. | Đồng ý. | Đánh dấu số liệu là cần đo; đề xuất lấy tỷ lệ bổ sung, số lượt bổ sung và thời gian chờ từ phỏng vấn/log được phép. |
| Chưa xác định nguyên nhân của việc bổ sung; có thể do khách hàng thiếu giấy tờ, hướng dẫn chưa rõ hoặc quy trình thay đổi. | Đồng ý. | Giữ nội dung ở dạng giả thuyết và thêm câu hỏi kiểm chứng về lần gần nhất, lý do bổ sung và bước phát hiện. |
| Quy trình ngân hàng có control point; tối ưu tốc độ không được làm giảm kiểm soát hoặc thay quyết định nghiệp vụ. | Đồng ý. | Giới hạn candidate vào tính đầy đủ, bàn giao và thao tác theo dõi; ghi rõ không đề xuất AI quyết định tín dụng hay bỏ bước kiểm soát. |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | | |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: | |
| Nhận phản biện | Câu hỏi tôi nhận được: | Tôi đã sửa gì: |
| Gom cluster / cây OST | | |
| Chọn candidate problem | | |
| Kiểm chứng / research | | |
| Quy trình nhóm | | |
| Problem Statement | | |
| Mức can thiệp AI | | |
| Quyết định | | |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | | | | |
| CP2 Problem Card | | | | |
| CP4 Research | | | | |
| CP5 Quy trình | | | | |
| CP5–6 Problem Statement | | | | |
| CP6 Mức can thiệp / quyết định | | | | |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

---

## 7. Tài liệu tham khảo

-
