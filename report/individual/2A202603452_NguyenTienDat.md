# Báo cáo cá nhân — Nguyễn Tiến Đạt (2A202603452)

> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm, commit bằng tài khoản GitHub của chính mình.

## 1. Thông tin học viên

- Họ tên: Nguyen Tien Dat
- MSSV: 2A202603452
- Email trường 26ai.datnt23@vinuni.edu.vn
- Tên nhóm: hihihaha
- Link repo nhóm: https://github.com/PhiHoangNamRaymond/K5-L3A-Day02-hihihaha-DiscoveryProblemFraming.git

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Cần đọc, tổng hợp nhiều thông tin | Khi bắt đầu một task mới trên Jira, tôi muốn nắm đúng yêu cầu và tài liệu liên quan ngay từ đầu, để không phải đọc lại nhiều lần | Thực tập sinh, mentor, BA | Khoảng 60 phút/lần đọc mô tả task và tài liệu nội bộ trước khi bắt tay làm |
| 2 | Tốn thời gian | Khi làm task import Excel cho sổ quỹ tiền mặt, tôi muốn xác định đúng dữ liệu và cột ngay từ đầu, để không phải sửa lại file sau khi test | Thực tập sinh, người test | Task mất khoảng 2 giờ (lần gần nhất); bước xác định dữ liệu và map cột Excel tốn thời gian nhất |
| 3 | Pain từ người khác | Khi đồng nghiệp cần test chức năng, tôi muốn họ tự xem được trạng thái task, để tôi không bị ngắt giữa lúc code | Đồng nghiệp test, thực tập sinh | Bị hỏi "làm xong chưa để test" khoảng 5 lần/tuần |
| 4 | Pain từ người khác | Khi mentor review code, tôi muốn phần giải thích cách làm có sẵn, để không phải giải thích lại từ đầu | Mentor, thực tập sinh | Mentor hỏi "vì sao làm như này" khoảng 2 lần/tuần |
| 5 | Lặp lại | Khi hoàn thành một task, tôi muốn cập nhật tiến độ nhanh, để không mất thời gian mỗi lần chuyển trạng thái | Thực tập sinh, mentor, BA | 5–10 phút/lần cập nhật tiến độ trên Jira |
| 6 | Lặp lại, Pain từ người khác | Khi có người hỏi về tính năng "nhập số dư ban đầu của tài khoản", tôi muốn tìm lại trạng thái và người phụ trách ngay, để trả lời mà không phải lục lại chat | Cả nhóm dev, BA | Khoảng 1 lần/tháng; bằng chứng là tin nhắn hỏi lại trong nhóm chat |
| 7 | Tốn thời gian | Khi vẽ diagram cho bài tập/đồ án, tôi muốn ra đúng cấu trúc ngay bản đầu, để không phải sửa lại nhiều vòng theo feedback | Sinh viên, bạn cùng nhóm | Khoảng 1 giờ/lần, 3 lần/tuần |
| 8 | Pain từ người khác, Cần đọc, tổng hợp nhiều thông tin | Khi làm bài nhóm, tôi muốn biết rõ phần nào mình phải làm, để không hỏi lại bạn và không nộp trễ | Sinh viên, bạn cùng nhóm | 1 lần nộp trễ bị trừ điểm vì nhớ lộn deadline; ít nhất 1 lần phải hỏi lại bạn vì thiếu thông tin |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- Tôi tự scan 8 problem từ trải nghiệm thực tập ở MobifoneIT và làm bài nhóm trước khi hỏi AI.
- AI chỉ giúp viết lại các ý đã có thành Job Story và kiểm tra mỗi dòng đã có dấu hiệu thật chưa; AI không tạo problem mới.
- AI có gợi ý thêm hướng "nhắc deadline cá nhân", nhưng tôi bỏ vì bằng chứng mới chỉ có 1 lần nộp trễ, chưa đủ mạnh để thành một problem riêng.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

> Số phút từng bước là ước lượng từ tổng thời gian tôi đã kể; sẽ cập nhật lại sau khi log thực tế.

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Import Excel sổ quỹ tiền mặt (CP1 #2) | Quy trình rõ, bottleneck là một bước cụ thể (map cột), baseline khoảng 2 giờ | Chưa rõ tần suất task/tháng; bottleneck thật có thể nằm ở khâu nhận yêu cầu từ BA |
| 2 | Vẽ diagram đồ án (CP1 #7) | Lặp 3 lần/tuần, tổng khoảng 3 giờ/tuần, dễ đo thời gian | "Chất lượng diagram" khó đo, dễ thành metric cảm tính |
| 3 | Đọc hiểu yêu cầu task Jira (CP1 #1) | Ảnh hưởng mọi task, khoảng 60 phút/task | "Hiểu đúng" khó đo; dễ trượt sang bài "chat với tài liệu" quá rộng |

### Problem Card #1 — Import Excel sổ quỹ tiền mặt

| Trường | Nội dung |
|---|---|
| Job Story | Khi làm task import Excel cho sổ quỹ tiền mặt, tôi muốn xác định đúng dữ liệu và cột ngay từ đầu, để không phải sửa lại file sau khi test |
| Actor | Thực tập sinh dev ở MobifoneIT, nhận task từ Jira, báo cáo mentor và BA |
| Thời điểm / bối cảnh | Khi nhận task import dữ liệu từ file Excel vào hệ thống sổ quỹ |
| Quy trình hiện tại (3–7 bước) | 1. Nhận task trên Jira, đọc mô tả → 2. Tìm file mẫu và tài liệu định dạng → 3. Xác định dữ liệu nguồn và map cột Excel → 4. Viết code import → 5. Test file mẫu, sửa lỗi → 6. Báo cáo mentor/BA, cập nhật Jira |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 — xác định dữ liệu và map cột Excel: khoảng 40 phút/lần |
| Impact (nếu không giải thì sao) | Mỗi task mất khoảng 2 giờ; chặn bước test của đồng nghiệp; nếu map sai phải sửa code và test lại |
| Success metric (baseline → target) | Từ 120 phút xuống còn 60 phút/task, đo bằng log thời gian 3 task import tiếp theo; số lần phải sửa file sau test không tăng |
| Phương án không dùng AI | Template mapping cột, checklist định dạng file, config/script import tái sử dụng cho các file cùng cấu trúc |
| Giả thuyết về AI (nếu có) | AI đọc mô tả task và file mẫu, đề xuất mapping cột và cảnh báo dữ liệu lỗi; người vẫn kiểm và sửa |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 120 phút/task

[1 Đọc task Jira: 10'] → [2 Tìm file mẫu + tài liệu: 15']
→ [3 Xác định dữ liệu + map cột Excel: 40'] ← BOTTLENECK
→ [4 Viết code import: 30'] → [5 Test + sửa lỗi: 20'] → [6 Báo cáo + cập nhật Jira: 5']
```

### Problem Card #2 — Vẽ diagram đồ án

| Trường | Nội dung |
|---|---|
| Job Story | Khi vẽ diagram cho bài tập/đồ án, tôi muốn ra đúng cấu trúc ngay bản đầu, để không phải sửa lại nhiều vòng theo feedback |
| Actor | Sinh viên năm cuối làm đồ án nhóm |
| Thời điểm / bối cảnh | Các buổi làm đồ án trước deadline, khoảng 3 lần/tuần |
| Quy trình hiện tại (3–7 bước) | 1. Đọc yêu cầu đề và rubric → 2. Xác định actor và luồng chính → 3. Vẽ bản nháp → 4. Nhận feedback và sửa diagram → 5. Xuất ảnh, chèn vào báo cáo |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4 — sửa diagram theo feedback: khoảng 20–25 phút/lần, thường phải sửa 2 vòng |
| Impact (nếu không giải thì sao) | Khoảng 1 giờ/lần, 3 lần/tuần, tức khoảng 3 giờ/tuần; sửa nhiều vòng làm trễ các phần khác của đồ án |
| Success metric (baseline → target) | Từ 60 phút xuống còn 30 phút/lần, đo trong 3 lần vẽ tiếp theo; số vòng sửa feedback giảm từ 2 vòng xuống 1 vòng |
| Phương án không dùng AI | Template diagram, checklist thành phần bắt buộc, vẽ nháp ra giấy trước khi vào tool |
| Giả thuyết về AI (nếu có) | AI chuyển mô tả bằng chữ thành Mermaid/PlantUML nháp; sinh viên kiểm từng bước và sửa |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 60 phút/lần, 3 lần/tuần

[1 Đọc đề + rubric: 5'] → [2 Xác định actor/luồng: 10']
→ [3 Vẽ bản nháp: 25'] → [4 Sửa theo feedback: 20'] ← BOTTLENECK
→ [5 Xuất ảnh + chèn báo cáo: 5']
```

### Problem Card #3 — Đọc hiểu yêu cầu task Jira

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận task mới trên Jira, tôi muốn hiểu đúng yêu cầu và tài liệu liên quan trong một lần đọc, để không làm sai hướng rồi phải hỏi lại mentor |
| Actor | Thực tập sinh dev, mentor, BA |
| Thời điểm / bối cảnh | Mỗi khi nhận task mới trên Jira |
| Quy trình hiện tại (3–7 bước) | 1. Nhận task → 2. Đọc mô tả và acceptance criteria → 3. Tìm tài liệu nội bộ → 4. Đọc và đối chiếu tài liệu → 5. Hỏi lại mentor/BA chỗ chưa rõ → 6. Chốt cách làm, bắt đầu code |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4 — đọc tài liệu nội bộ và đối chiếu với mô tả task: khoảng 35 phút/lần |
| Impact (nếu không giải thì sao) | Khoảng 60 phút/task trước khi code; mentor bị hỏi lại 2 lần/tuần; làm sai hướng thì phải sửa code |
| Success metric (baseline → target) | Từ 60 phút xuống còn 25 phút/task, đo trong 3 task tiếp theo; số câu hỏi lại mentor không tăng; số lần phải làm lại do sai hướng giảm |
| Phương án không dùng AI | Checklist đọc task, template câu hỏi làm rõ gửi BA/mentor, ghi chú knowledge base ngắn |
| Giả thuyết về AI (nếu có) | AI tóm tắt mô tả và tài liệu, liệt kê điểm mơ hồ cần hỏi lại; người quyết định |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 60 phút/task

[1 Nhận task: 2'] → [2 Đọc mô tả + AC: 15'] → [3 Tìm tài liệu nội bộ: 10']
→ [4 Đọc + đối chiếu tài liệu: 35'] ← BOTTLENECK
→ [5 Hỏi lại mentor/BA: 5'] → [6 Chốt cách làm: 3']
```

### Card muốn pitch nhất

- Card số: 1 — Import Excel sổ quỹ tiền mặt
- Vì sao: quy trình rõ nhất, bottleneck là một bước cụ thể, baseline khoảng 2 giờ đo được, ảnh hưởng trực tiếp tới người test.
- Câu hỏi muốn nhóm phản biện: "Map cột Excel có thực sự là bottleneck, hay bottleneck thật là khâu BA mô tả yêu cầu chưa rõ định dạng file?"

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Baseline 120 phút chỉ đến từ 1 lần làm, chưa đủ tin cậy | Đồng ý | Ghi rõ "lần gần nhất"; lên kế hoạch log thêm 2–3 task trước khi chốt |
| Metric chỉ đo thời gian, không đo chất lượng file import | Đồng ý | Thêm "số lần phải sửa file sau test không tăng" vào metric |
| Bottleneck map cột có thể chỉ là triệu chứng của yêu cầu BA mơ hồ | Đồng ý một phần | Đưa vào câu hỏi pitch; nếu nhóm xác nhận thì chuyển bottleneck lên bước nhận yêu cầu |
| Gợi ý để Agent tự đọc Jira rồi tự code | Không đồng ý | Giữ người kiểm ở bước mapping và test; mức đề xuất vẫn là Workflow |
| Card diagram: "sửa feedback" chưa chắc là bottleneck, có thể do đề bài mơ hồ | Đồng ý | Ghi vào "điều còn chưa chắc"; sẽ hỏi bạn cùng nhóm ở CP4 |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Pitch 3 card: #1 import Excel sổ quỹ (bottleneck map cột ~40 phút/lần), #2 vẽ diagram đồ án (~20–25 phút/vòng, 2 vòng), #3 đọc hiểu task Jira (~35 phút/tài liệu). Card tôi muốn pitch nhất là #1 vì quy trình rõ và bottleneck nằm ở một bước cụ thể. | Cả 3 card vào bảng pitch; #1 được giữ lại ở shortlist để so sánh. |
| Phản biện bài của bạn khác | Đặt câu hỏi cho 3 card: #6 (Nam — hỏi lần gần nhất bỏ lỡ 2 workshop thì đọc thông báo ở kênh nào và sót ở bước nào), #7 (Thành — hỏi 5 lượt hỏi lại xảy ra trong bao nhiêu buổi họp), #11 (Huy — hỏi lỗi cũ/mới dựa vào đâu để chọn action và lần gần nhất phải sửa action mất bao lâu). | Kéo các bạn từ mô tả cảm tính sang hành vi đã xảy ra và con số cụ thể. |
| Nhận phản biện | Thành hỏi card #1: “Trong lần gần nhất, điều gì khiến bạn mất nhiều thời gian nhất khi map cột Excel?” | Tôi tách riêng bước map cột khỏi bước đọc yêu cầu BA và ghi lại baseline theo từng bước thay vì gộp chung 2 giờ. |
| Gom cluster / cây OST | Cùng nhóm gom 12 candidate thành 3 cluster; #1 của tôi vào cluster A (xử lý file/dữ liệu), #2 và #3 vào cluster B (đọc hiểu và sửa theo feedback). | Loại “form Excel tự điền” vì đó là giải pháp, không phải vấn đề. |
| Chọn candidate problem | Ban đầu tôi bảo vệ #1, sau khi so sánh thì đồng ý chọn #12 của Huy: lặp lại hằng tuần và đo được 20 phút tra + 50 phút điền. | #12 đạt 29/35 điểm và trở thành candidate của nhóm. |
| Kiểm chứng / research | Đọc lại 5 survey và 2 phỏng vấn; đối chiếu baseline: 140–210 phút cho toàn báo cáo (trung vị 170), 4/5 từng nhập sai, PM bị khách phàn nàn. | Nhóm có bằng chứng định lượng thay cho ước tính 70 phút ban đầu. |
| Quy trình nhóm | Góp ý tách quy trình trước/sau thành 5 bước, trong đó bước PE đối chiếu (12 phút) là điểm kiểm soát. | Quy trình v1 có bước kiểm tra và phương án quay về thủ công. |
| Problem Statement | Hỗ trợ rà Actor, Bottleneck, Impact, baseline 70/170 phút và Boundary giữa v0 và v1. | v1 tách đúng phạm vi đo, thêm chỉ tiêu 0 lỗi số liệu sau nộp. |
| Mức can thiệp AI | So sánh 4 mức: thủ công, Rule, Workflow, Agent. | Nhóm chọn **Rule** (Power Query + biểu mẫu Excel) vì dữ liệu có cấu trúc, mapping xác định; không cần AI. |
| Quyết định | Viết phần rủi ro và tiêu chí dừng cho pilot. | **Go — pilot nhỏ 4 tuần**, 1 PE/1 dây chuyền; dừng nếu thời gian không giảm dưới ngưỡng hoặc phát sinh lỗi số liệu. |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Nhờ AI viết lại các problem tôi đã tự liệt kê thành Job Story và kiểm tra dấu hiệu thật | Viết nhanh hơn, chỉ ra dòng nào còn thiếu số liệu | AI gợi ý thêm hướng "nhắc deadline cá nhân" quá rộng, không có bằng chứng lặp lại | Bỏ ý đó, giữ 8 problem từ trải nghiệm thật |
| CP2 Problem Card | Nhờ AI đóng vai PM hoài nghi phản biện 3 card | Chỉ ra baseline 1 lần chưa đủ, metric chỉ đo thời gian | AI đề xuất Agent tự đọc Jira và tự code | Giữ mức Workflow và thêm bước người kiểm |
| CP4 Research | Nhờ AI tóm tắt 3 link research (Power Query, xlwings Reports, InfinityQS) và so sánh công cụ nào khớp quy trình tra → điền số. | Tóm tắt nhanh, chỉ ra Power Query phù hợp vì dữ liệu nguồn có cấu trúc. | AI gợi ý dùng giải pháp SPC của InfinityQS, quá lớn so với một PE và một biểu mẫu Excel. | Bỏ InfinityQS, chỉ giữ Power Query + mẫu Excel. |
| CP5 Quy trình | Nhờ AI kiểm tra quy trình trước/sau có thiếu bước người kiểm (HITL) và phương án quay về không. | Chỉ ra bước “PE đối chiếu” chưa có tiêu chí dừng rõ ràng. | AI mô tả chung chung kiểu “AI hỗ trợ kiểm tra”, không nói ai kiểm cái gì. | Thêm boundary: Rule không tự sửa số, không tự gửi; PE kiểm từng mục. |
| CP5–6 Problem Statement | Nhờ AI soi lỗ hổng metric: baseline đang trộn 70 phút với 170 phút, thiếu tiêu chí chất lượng. | Phát hiện phạm vi đo chưa tách và metric chỉ có thời gian. | AI đề xuất thêm “AI dự đoán số liệu tuần sau” — không liên quan vì dữ liệu đã có sẵn trong file nguồn. | Tách baseline 70 phút (tra + điền) và 170 phút (toàn báo cáo), thêm 0 lỗi sau nộp. |
| CP6 Mức can thiệp / quyết định | Nhờ AI lập bảng so sánh 4 mức can thiệp và liệt kê rủi ro của từng mức. | Bảng so sánh đủ 4 mức, giúp thấy Rule rẻ và ổn định hơn Agent. | AI nghiêng về Agent/Workflow vì “linh hoạt hơn”, trong khi bài toán chỉ là ánh xạ cột cố định. | Hạ xuống Rule; thêm rủi ro lệch layout file và phương án quay về thủ công. |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Tôi quan sát được cách mọi người nhìn nhận vấn đề

**6.2. Nhóm có lúc nào bị "solution-first" không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Nhóm có bị "solution-first", lúc đó nhóm thảo luận lại kĩ hơn

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Tôi đổi ý từ card #1 sang card #12. Ban đầu tôi bảo vệ #1 vì quy trình rõ và tôi đã trải qua. Nhưng khi đặt hai card cạnh nhau, #1 chỉ xảy ra một lần, còn #12 lặp lại hằng tuần và tách được hai bước đo riêng: 20 phút tra số, 50 phút điền form. Nhóm chấm #12 được 29/35, cao hơn #1. Tôi đồng ý vì tiêu chí lặp lại và đo được quan trọng hơn cảm giác “vấn đề của mình cũng hay”. Đây là lần đầu tôi thấy mình phải bỏ một card do chính mình pitch.
Tôi có đổi ý từ card #1 sang card #12 bởi vì tiêu chí lặp lại, card #12 lặp lại hàng tuần so với card #1 thì chỉ lặp lại 1 lần

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

Kết quả kiểm chứng làm tôi bất ngờ vì con số to hơn tôi nghĩ

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Điều khó nhất khi viết Problem Statement là tách problem khỏi solution

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

Nếu làm lại, tôi nên hỏi cụ thể về những con số từ đâu ra 

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.
PE tại nhà máy sản xuất mạch điện tử mất khoảng 70 phút mỗi tuần để tra số lượng sản xuất và điền vào biểu mẫu báo cáo tuần, trong đó tra số khoảng 20 phút còn copy-paste vào form khoảng 50 phút — đây là bước tốn thời gian nhất. Nhóm đặt mục tiêu giảm phần tra + điền từ 70 xuống 30 phút, cả báo cáo từ 170 xuống 130 phút, kèm 0 lỗi số liệu trong 4 tuần, với boundary là công cụ chỉ được gom số và ánh xạ cột theo mapping có sẵn, không được tự sửa số hay tự gửi, PE vẫn kiểm cuối. Vì dữ liệu có cấu trúc và cột cần điền cố định nên nhóm chọn mức Rule (Power Query + mẫu Excel, không dùng AI) và quyết định Go với pilot nhỏ 4 tuần trên 1 PE/1 dây chuyền, dừng nếu thời gian không giảm hoặc phát sinh lỗi số liệu.

---

## 7. Tài liệu tham khảo

- Microsoft. *Power Query documentation*. https://learn.microsoft.com/en-us/power-query/ — dùng để kiểm tra khả năng gom và biến đổi dữ liệu nguồn trước khi đưa vào biểu mẫu Excel.
- xlwings. *Reports*. https://docs.xlwings.org/en/stable/reports.html — tham khảo cách điền số liệu vào biểu mẫu Excel có sẵn.
- InfinityQS. *Statistical Process Control (SPC) software*. https://www.infinityqs.com/ — so sánh giải pháp SPC thương mại; nhóm loại vì quá lớn so với phạm vi một PE.
- Google. *People + AI Guidebook (PAIR)*. https://pair.withgoogle.com/guidebook/ — tham khảo nguyên tắc thiết kế có người kiểm và minh bạch với người dùng.
- Fitzpatrick, R. *The Mom Test*. https://www.momtestbook.com/ — cách hỏi về hành vi đã xảy ra thay vì xin ý kiến, dùng khi thiết kế câu hỏi phản biện và survey.
- Anthropic. *Building effective agents*. https://www.anthropic.com/engineering/building-effective-agents — cơ sở để so sánh mức Rule, Workflow và Agent trước khi chọn Rule.
- Báo cáo nhóm *hihihaha*: `report/team/group_report.md` — nguồn dữ liệu pitch, 5 survey, 2 phỏng vấn, Problem Statement v0/v1 và quyết định Go.
