# Báo cáo cá nhân — 2A202603452_NguyenTienDat

> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm, commit bằng tài khoản GitHub của chính mình.

## 1. Thông tin học viên

- Họ tên: Nguyen Tien Dat
- MSSV: 2A202603452
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: (điền khi chốt tên nhóm)
- Link repo nhóm: https://github.com/PhiHoangNamRaymond/K5-L3A-Day02-PhiHoangNam-2A202603435-DiscoveryProblemFraming

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
| CP1 Scan | Nhờ AI viết lại các problem tôi đã tự liệt kê thành Job Story và kiểm tra dấu hiệu thật | Viết nhanh hơn, chỉ ra dòng nào còn thiếu số liệu | AI gợi ý thêm hướng "nhắc deadline cá nhân" quá rộng, không có bằng chứng lặp lại | Bỏ ý đó, giữ 8 problem từ trải nghiệm thật |
| CP2 Problem Card | Nhờ AI đóng vai PM hoài nghi phản biện 3 card | Chỉ ra baseline 1 lần chưa đủ, metric chỉ đo thời gian | AI đề xuất Agent tự đọc Jira và tự code | Giữ mức Workflow và thêm bước người kiểm |
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
