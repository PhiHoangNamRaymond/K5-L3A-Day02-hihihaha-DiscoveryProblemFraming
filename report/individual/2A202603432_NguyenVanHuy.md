# Báo cáo cá nhân — Nguyễn Văn Huy (2A202603432)

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Văn Huy
- MSSV: 2A202603432
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: hihihaha
- Link repo nhóm: https://github.com/PhiHoangNamRaymond/K5-L3A-Day02-hihihaha-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

Bối cảnh: tôi làm pe (product engineer) ở nhà máy sản xuất mạch điện tử, mỗi tuần phải lập một báo cáo tuần (weekly report).

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại · Tốn thời gian | Khi tới cuối tuần phải nộp weekly report, tôi muốn có sẵn số liệu và nội dung trong một chỗ, để không phải tổng hợp lại từ đầu mỗi tuần | Tôi (PE – product engineer) | Lặp lại mỗi tuần; tổng ~180 phút/tuần (3 giờ) |
| 2 | Tốn thời gian | Khi bắt đầu viết report, tôi muốn tra nhanh số lượng sản xuất của tuần trước, để không phải mở nhiều màn hình và cộng tay | Tôi | ~20 phút mỗi tuần; số liệu tra trên phần mềm test/hệ thống sản xuất |
| 3 | Cần đọc, tổng hợp nhiều thông tin | Khi cần phần lỗi trong report, tôi muốn gom và xếp hạng mã lỗi test nhiều nhất trong tuần, để xác định đúng top 3 thay vì tự lọc tay | Tôi | ~60 phút/tuần: tải file Excel từ phần mềm test rồi lọc mã lỗi bằng tool |
| 4 | Cần đọc, tổng hợp nhiều thông tin | Khi viết action cho mỗi lỗi và mỗi sản phẩm, tôi muốn tra lại cách đã xử lý lỗi tương tự trước đây, để không phải nghĩ lại từ đầu và giữ action nhất quán | Tôi, tổ bảo trì/QA | Lỗi cũ ~20 phút; lỗi mới ~30 phút mỗi tuần |
| 5 | Lặp lại | Khi sản phẩm/line thay đổi, tôi muốn biết mã lỗi mới phát sinh so với tuần trước, để report nêu đúng điểm mới | Tôi, quản lý line | Mỗi tuần đều có mã lỗi mới; viết action cho lỗi mới tốn thêm ~30 phút/lần |
| 6 | Pain từ người khác | Khi tổ test/QA cần số liệu lỗi, tôi muốn trả lời nhanh số lỗi và action, để không bị hỏi lại nhiều lần | Tôi, tổ test/QA | ~1 lần/tuần; có thể nhiều hơn khi phát sinh bất thường |
| 7 | Tốn thời gian | Khi định dạng report theo template cố định, tôi muốn số liệu tự vào đúng ô/bảng, để không mất thời gian copy-paste | Tôi | ~50 phút/tuần copy dữ liệu dán vào form báo cáo |
| 8 | Cần đọc, tổng hợp nhiều thông tin | Khi phải viết phần nhận định cho report, tôi muốn có sẵn dàn ý từ số liệu, để viết nhận xét nhanh hơn | Tôi | ~15 phút/tuần cho phần review/nhận định |

Phân bổ 180 phút/tuần: tra số lượng 20' + lọc top 3 mã lỗi 60' + viết action lỗi cũ 20' + viết action lỗi mới 30' + copy dữ liệu vào form 50' (trong đó có ~15' review/nhận định).

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- Giữ lại dòng 5–8 (mã lỗi mới, tổ test/QA hỏi lại, copy dữ liệu vào form, viết nhận định) — đúng với trải nghiệm thật ở nhà máy.
- Bỏ: chưa có ý nào bị bỏ. Các dòng 6 và 8 cần bổ sung con số thật (mấy lần/tuần, mấy phút).

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Lọc & xếp hạng top 3 mã lỗi test nhiều nhất trong tuần (60') | Bottleneck lớn nhất, số phút đo được, dữ liệu đã nằm trong phần mềm test, vừa sức một buổi lab | Chưa rõ thời gian thật nằm ở bước tải file hay bước lọc; có thể chỉ cần pivot/công thức (Rule) là đủ |
| 2 | Viết action cho từng mã lỗi (cũ 20' + mới 30') | Impact rõ, đụng đúng chuyên môn PE; có thể dùng kiến thức lịch sử để hỗ trợ | Action phụ thuộc nhiều ngữ cảnh và kinh nghiệm, khó "đúng/sai" rõ |
| 3 | Tổng hợp & điền form weekly report (tra số lượng 20' + copy 50') | Đụng cả quy trình, dễ thấy before/after | Đây là việc tổng hợp, chủ yếu copy-paste — phần lớn có thể là No AI |

### Problem Card #1 — Lọc top 3 mã lỗi test

| Trường | Nội dung |
|---|---|
| Job Story | Khi chuẩn bị phần lỗi cho weekly report, tôi muốn biết ngay 3 mã lỗi test xuất hiện nhiều nhất trong tuần, để nêu đúng trọng tâm mà không phải lọc tay |
| Actor | Tôi — PE phụ trách weekly report của line |
| Thời điểm / bối cảnh | Cuối tuần, trước khi nộp report; dữ liệu test cả tuần đã nằm trong phần mềm test |
| Quy trình hiện tại (3–7 bước) | 1. Chọn khoảng thời gian trong phần mềm test → 2. Tải file Excel kết quả test → 3. Lọc mã lỗi bằng tool trong Excel → 4. Đếm, xếp hạng, chọn top 3 → 5. Ghi vào report |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 lọc mã lỗi bằng tay (~30') và bước 2 tải/làm sạch file (~10') |
| Impact (nếu không giải thì sao) | Mất 60'/tuần; làm vội dễ đếm sai/sót lỗi → report sai trọng tâm, bỏ lọt lỗi lặp lại |
| Success metric (baseline → target) | 60 phút/tuần → dưới 15 phút/tuần, đo bằng tự bấm giờ mỗi tuần trong 4 tuần pilot |
| Phương án không dùng AI | Template Excel có pivot table + công thức COUNTIF theo mã lỗi, hoặc script lọc/pivot cố định (Rule) |
| Giả thuyết về AI (nếu có) | AI đọc file Excel và trả về danh sách top mã lỗi kèm số lượng (chỉ cân nhắc sau khi Rule đã dùng) |
| Cảm nhận nhanh | Rule |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — ~60 phút/tuần

[Chọn thời gian trên phần mềm test: 5'] → [Tải file Excel: 10']
→ [Lọc mã lỗi bằng tool trong Excel: 30'] ← BOTTLENECK
→ [Đếm, xếp hạng, chọn top 3: 10'] → [Ghi vào report: 5']
```

### Problem Card #2 — Viết action cho từng mã lỗi

| Trường | Nội dung |
|---|---|
| Job Story | Khi viết action cho mỗi mã lỗi, tôi muốn tra lại nhanh cách đã xử lý lỗi tương tự trước đây, để ra action nhất quán mà không phải nghĩ lại từ đầu |
| Actor | Tôi — PE, phối hợp tổ bảo trì/QA |
| Thời điểm / bối cảnh | Sau khi đã có top 3 mã lỗi, khi viết phần action của report |
| Quy trình hiện tại (3–7 bước) | 1. Xem mã lỗi cần viết action → 2. Tra lịch sử/tài liệu xem lỗi này đã gặp chưa → 3. Trao đổi tổ bảo trì/QA nếu là lỗi mới → 4. Viết action → 5. Ghi vào report |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2–3 tra lịch sử và hỏi người; lỗi mới tốn nhất (cũ ~20', mới ~30') |
| Impact (nếu không giải thì sao) | 50'/tuần; action chậm, không nhất quán, lỗi dễ tái diễn |
| Success metric (baseline → target) | 50 phút/tuần → dưới 20 phút/tuần; đo bằng bấm giờ và số lần phải hỏi lại bộ phận khác |
| Phương án không dùng AI | Bảng tra cứu "mã lỗi → action chuẩn" dạng wiki/sổ tay cập nhật (No AI / Rule) |
| Giả thuyết về AI (nếu có) | AI gợi ý action dựa trên lịch sử xử lý; con người (PE) duyệt trước khi ghi vào report |
| Cảm nhận nhanh | Workflow (AI gợi ý, người duyệt) hoặc No AI nếu bảng tra đã đủ |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — ~50 phút/tuần (cũ 20' + mới 30')

[Xem mã lỗi: 2'] → [Tra lịch sử đã gặp chưa: 15'] ← BOTTLENECK
→ [Hỏi tổ bảo trì/QA nếu lỗi mới: 20'] ← BOTTLENECK (lỗi mới)
→ [Viết action: 10'] → [Ghi vào report: 3']
```

### Problem Card #3 — Tổng hợp & điền form weekly report

| Trường | Nội dung |
|---|---|
| Job Story | Khi tới cuối tuần phải nộp weekly report, tôi muốn số liệu tự vào đúng form báo cáo, để không phải tra số lượng và copy-paste thủ công |
| Actor | Tôi — PE phụ trách weekly report |
| Thời điểm / bối cảnh | Cuối tuần, khi lắp report từ các phần đã chuẩn bị |
| Quy trình hiện tại (3–7 bước) | 1. Tra số lượng sản xuất tuần trước → 2. Ghép top 3 lỗi + action → 3. Copy dữ liệu dán vào form báo cáo → 4. Đọc lại → 5. Gửi |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 copy-paste và sắp lại form (~50'); bước 1 tra số lượng (~20') |
| Impact (nếu không giải thì sao) | 70'/tuần; dễ nhập nhầm, sai format, mất thời gian hơn cần thiết |
| Success metric (baseline → target) | 70 phút/tuần → dưới 20 phút/tuần; đo bằng bấm giờ và số lỗi phải sửa lại sau khi nộp |
| Phương án không dùng AI | Form Excel có ô liên kết/lookup tự kéo số liệu; template cố định (Rule) |
| Giả thuyết về AI (nếu có) | Chưa chắc cần AI; nhiều khả năng chỉ cần tự động hoá form. Nếu có, AI chỉ hỗ trợ viết phần nhận định |
| Cảm nhận nhanh | Rule |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — ~70 phút/tuần

[Tra số lượng sản xuất: 20'] → [Ghép top 3 lỗi + action: 5']
→ [Copy dữ liệu dán vào form: 50'] ← BOTTLENECK
→ [Đọc lại: 5'] → [Gửi: 2']
```

### Card muốn pitch nhất

- Card số: 1
- Vì sao: bottleneck lớn nhất (60'), số phút đo được, dữ liệu đã có sẵn trong phần mềm test, vừa sức một buổi lab.
- Câu hỏi muốn nhóm phản biện: "Nếu pivot table/công thức COUNTIF (Rule) đã giảm được phần lớn 60 phút, thì đâu mới thật sự là phần cần AI — làm sạch dữ liệu test hay gợi ý phần nhận định?"

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Card #1: pivot table/công thức COUNTIF có thể đã giải ~80%, nên chưa chắc cần AI | Đồng ý | Ghi rõ phương án No AI/Rule trước; chỉ cân nhắc AI ở bước làm sạch/chuẩn hoá dữ liệu test |
| Actor "PE" còn chung, chưa nói PE nào | Đồng ý một phần | Thu hẹp thành "PE phụ trách weekly report của line" |
| Chưa chắc bottleneck là bước lọc (30'), có thể là bước tải file (10') | Đồng ý | Ghi cả hai bước vào ô bottleneck để kiểm chứng bằng bấm giờ |
| Card #3 phần lớn là copy-paste, dễ bị "solution-first" | Đồng ý | Hạ cảm nhận nhanh của Card #3 xuống Rule, không đẩy lên AI |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Pitch 3 candidate #10–#12 xuất phát từ trải nghiệm PE tại nhà máy; mô tả quy trình lập báo cáo tuần. | Cả 3 vào bảng pitch của nhóm; #12 vào shortlist và được nhóm chọn (29/35 điểm). |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: "Trong 30 phút chuẩn bị bài Day 1, riêng việc đọc và tổng hợp yêu cầu mất bao lâu nếu tách thời gian tìm hiểu Colab?" (cho candidate #4 của Nam). | Câu hỏi được đưa vào bảng pitch CP3 ở ô phản biện của #4 (mục 2.1 báo cáo nhóm), giúp nhóm khoanh lại phạm vi cần đo của #4 thay vì gộp cả 30 phút. |
| Nhận phản biện | Câu hỏi tôi nhận được: "Trong lần lập báo cáo tuần gần nhất, phần nào tốn thời gian nhất trong 50 phút điền form: tìm đúng mục, chép số liệu hay kiểm tra lại?" (từ Thành, cho #12). | Tôi tách rõ #12 thành hai bước đo riêng: tra số lượng (~20') và điền form (~50'), thay vì gộp chung "lập báo cáo" — đúng như bảng pitch và quy trình CP5 ghi. |
| Gom cluster / cây OST | Cung cấp mô tả quy trình để nhóm xếp #10–#12 vào cụm A (báo cáo định kỳ của PE/QA). | Cây OST có 1 outcome gốc và 3 nhánh pain, trong đó #12 thuộc nhánh tổng hợp số liệu báo cáo. |
| Chọn candidate problem | Đưa baseline cho #12: ~20 phút tra số lượng + ~50 phút điền biểu mẫu. | Nhóm chọn #12 làm candidate problem. |
| Kiểm chứng / research | Phụ trách CP4: chạy 5 survey + 2 phỏng vấn (QA, PM) và lập bảng research 3 nguồn có link. | Kiểm chứng xác nhận pain ở bước chép số liệu vào form; phỏng vấn PM cho thấy hệ quả tới khách hàng. |
| Quy trình nhóm (CP5) | Cung cấp quy trình weekly report thật (2 bước: tra số lượng ~20' + điền form ~50') để nhóm vẽ before/after. | Bảng 4.1 và 4.3 dùng đúng baseline này; bước điền biểu mẫu (50') được xác định là bottleneck. |
| Problem Statement (CP5) | Cho số liệu để nhóm viết Problem Statement v0: actor là PE phụ trách weekly report của line; bottleneck là điền/copy số liệu vào form. | Actor, bottleneck và impact của PS v0 (70 phút/tuần) lấy từ trải nghiệm thật của tôi; nhóm ghi rõ baseline cần đo lại bằng bấm giờ. |
| Mức can thiệp AI (CP6) | Góp ý bước tra/copy số liệu chỉ cần Rule (Power Query + công thức Excel), chưa cần AI; giữ PE đối chiếu (HITL). | Định hướng quy trình tương lai (4.2) chọn Rule/Power Query thay vì AI; AI không được tự tạo/sửa số liệu hay tự gửi báo cáo. |
| Quyết định (CP6) | Góp ý ngưỡng dừng dựa trên kinh nghiệm: nếu mapping sai hoặc file nguồn đổi cấu trúc thì dừng tự động, quay về điền tay. | Nhóm đưa "phương án quay về" và điều kiện HITL vào quy trình tương lai; phần quyết định Go / Not Yet / No-Go còn chờ nhóm chốt. |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Nhờ AI gợi ý thêm lăng kính và cách diễn đạt 8 Job Story. | Giúp chuẩn hoá câu chữ và gợi ý thêm các tình huống về mã lỗi mới, tổ test/QA hỏi lại, copy dữ liệu vào form, viết nhận định. | AI đề xuất thêm dòng nhưng chưa có số đo thật (dòng 6 và 8 thiếu con số). | Giữ dòng 5–8 vì đúng trải nghiệm nhà máy, nhưng ghi rõ dòng 6 và 8 phải bổ sung số thật, không lấy số AI bịa. |
| CP2 Problem Card | Nhờ AI phản biện 3 Problem Card. | Chỉ ra Card #1 có thể giải ~80% bằng pivot table/COUNTIF; actor "PE" quá chung; bottleneck chưa chắc nằm ở bước lọc. | AI ban đầu vẫn nghiêng về hướng dùng AI cho việc copy-paste (solution-first). | Thu hẹp actor thành "PE phụ trách weekly report của line"; ghi phương án No AI/Rule trước; hạ cảm nhận nhanh của Card #3 xuống Rule. |
| CP4 Research | Nhờ AI tìm giải pháp đã có cho phần gom số liệu và điền form. | Gợi ý nhanh 3 nguồn có link (Power Query, xlwings Reports, InfinityQS) và chỉ ra khoảng trống của từng cái. | Nguồn quá tầm: InfinityQS là giải pháp cấp nhà máy; xlwings Reports cần bản PRO trả phí — không hợp bối cảnh. | Chỉ giữ Power Query làm hướng chính vì có sẵn trong Excel; loại phương án mua SPC. |
| CP5 Quy trình | Nhờ AI đối chiếu quy trình trước/sau và cách đặt boundary. | Giúp tách bước, viết BOUNDARY và "phương án quay về" rõ ràng. | AI có xu hướng vẽ thêm bước không có thật trong quy trình của tôi. | Đối chiếu lại với quy trình thật (chỉ 2 bước hiện tại) trước khi chốt; không thêm bước ngoài thực tế. |
| CP5–6 Problem Statement | Nhờ AI góp ý success metric và cách đo. | Giúp đặt metric có cách đo và theo dõi cả số lần sửa/lỗi. | AI có xu hướng đưa target không có cơ sở. | Giữ baseline 70 phút là ước tính tự báo cáo và ghi rõ phải đo lại bằng bấm giờ. |
| CP6 Mức can thiệp / quyết định | Đối chiếu 4 mức No AI / Rule / Workflow / Agent cho bài của nhóm. | Giúp lập luận vì sao chọn Rule thay vì AI. | AI có xu hướng đẩy lên Workflow/Agent dù việc chính chỉ là copy số liệu. | Hạ về Rule (Power Query + công thức) và giữ PE kiểm tra (HITL) trước khi dùng. |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Nghe 3 problem của nhóm, tôi nhận ra pain không chỉ nằm ở "tốn thời gian" mà còn ở chỗ yêu cầu và trách nhiệm chưa rõ. Problem #7 của Thành (hỏi lại sau họp không rõ việc, người phụ trách, hạn) và #4 của Nam (tổng hợp đầu việc bài lab) cho thấy nhiều người phải hỏi lại hoặc đọc lại tài liệu chỉ vì thông tin không tập trung. Điều này giúp tôi thấy vấn đề của mình (#12 — chép số liệu vào form báo cáo tuần) cũng nằm trong cùng một họ: thông tin đã có sẵn nhưng phải tổng hợp thủ công. Tôi cũng học được cách hỏi theo The Mom Test — hỏi về lần gần nhất đã xảy ra chuyện gì, thay vì hỏi "bạn có muốn…".

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Có, và khá rõ. Ngay khi vừa kể pain, cả QA lẫn PM được phỏng vấn đều tự đề xuất giải pháp: QA nói cần "AI agent quản lý dữ liệu", PM nói cần "một tool quản lý dữ liệu". Nhóm nhận ra đây là solution đội lốt, nên chỉ ghi lại như một ghi chú và không đưa vào tầng opportunity của cây OST. Ở CP3, nhóm cũng gạch bỏ "Form Excel dùng công thức tra cứu để tự điền số liệu (#12)" khỏi tầng opportunity vì đó là phương án giải quyết, còn vấn đề thật là thời gian tôi mất để tra và điền số liệu. Bản thân tôi cũng bị cuốn theo hướng này khi lần đầu nghĩ tới việc dùng AI cho bước copy dữ liệu.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Có, một lần cụ thể. Ban đầu tôi chọn pitch Card #1 — lọc và xếp hạng top 3 mã lỗi (khoảng 60 phút/tuần) — và nghĩ đây là chỗ cần AI. Nhưng khi bị phản biện rằng pivot table/công thức COUNTIF trong Excel có thể đã giải được khoảng 80%, tôi phải hạ kỳ vọng từ AI xuống Rule. Sau đó, trước câu hỏi của Thành về việc trong 50 phút điền form thì phần nào tốn thời gian nhất, tôi tách rõ #12 thành hai bước đo riêng — tra số lượng (khoảng 20 phút) và điền form (khoảng 50 phút) — thay vì gộp chung là "lập báo cáo". Việc tách bước này khiến nhóm thấy bottleneck thật nằm ở bước điền/chép số liệu vào form, đúng bài toán nhóm chọn ở #12.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

Có, hai điều khiến tôi bất ngờ. Thứ nhất, con số thời gian: tôi tự ước tính khoảng 70 phút/tuần, nhưng 5 phản hồi survey cho 170, 200, 210, 170 và 140 phút (trung vị 170) — cao hơn gấp đôi. Điều này cho thấy ước tính chủ quan rất dễ sai và baseline phải đo lại. Thứ hai, hệ quả không chỉ nằm trong nội bộ: phỏng vấn PM cho biết sai số liệu từng khiến khách hàng phàn nàn (cách đây khoảng 3 tuần, tần suất khoảng 3 tháng một lần), trong khi trước đó tôi chỉ nghĩ tới việc tốn thời gian nội bộ. Ngoài ra, 4/5 người từng nhập sai số trong 4 tuần gần nhất nhưng 0/5 nộp trễ — cho thấy pain nằm ở độ chính xác nhiều hơn ở hạn nộp.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Khó nhất là chốt chỉ số đo. Baseline 70 phút chỉ là con số tôi tự ước tính, không phải số bấm giờ, nên khi viết Problem Statement tôi phải ghi rõ đó là ước tính và cần đo lại. Khó thứ hai là vẽ boundary: phải nói rõ rule/AI không được làm gì (không tự tạo hay sửa số liệu nguồn, không tự gửi báo cáo) và chỗ nào con người phải kiểm tra (HITL) — trong khi vẫn phải đưa ra được một quy trình tương lai cụ thể, không rơi vào chung chung.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

Nếu làm lại, tôi sẽ bấm giờ thật ngay từ CP3 thay vì ước tính, để baseline không lệch xa thực tế như lần này (70 phút so với 140–210 phút). Tôi cũng sẽ phản biện nhóm mạnh hơn khi có người gộp nhiều bước vào một con số thời gian, vì chính việc tách bước mới giúp xác định đúng bottleneck. Với #12, tôi sẽ chốt trước định nghĩa "thời gian lập báo cáo" gồm những bước nào, vì mẫu khảo sát đang tính rộng hơn phạm vi 2 bước của nhóm, dẫn tới so sánh chưa thật công bằng.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

Bài của nhóm bắt đầu từ problem #12: PE tại nhà máy sản xuất mạch điện tử lập báo cáo tuần và tốn khoảng 70 phút cho hai bước tra số lượng sản xuất rồi điền vào biểu mẫu. Quy trình hiện tại có 2 bước: tra số lượng (khoảng 20 phút) và chép số liệu vào đúng mục của form (khoảng 50 phút — đây là bottleneck chính). Metric là thời gian mỗi tuần: baseline ước tính 70 phút, mục tiêu không quá 30 phút, đo bằng bấm giờ và theo dõi cả số lần sửa/lỗi trong 4 tuần pilot. Boundary: rule chỉ gom và ánh xạ dữ liệu theo mapping đã xác nhận, không tự suy đoán hay sửa số liệu nguồn, không tự gửi báo cáo; PE phải đối chiếu với nguồn trước khi hoàn tất. Về mức can thiệp, nhóm chọn Rule (Power Query + công thức Excel) chứ không lên AI/Agent, vì phần lớn công việc là gom và điền số liệu, không phải suy luận. Quyết định hướng tới là Not Yet/Go có điều kiện: có ngưỡng dừng — nếu file nguồn đổi cấu trúc hoặc kết quả không khớp thì dừng tự động, quay về điền tay. Kiểm chứng ban đầu (5 survey + 2 phỏng vấn) xác nhận pain nằm ở bước tổng hợp/chép số liệu vào form, nhưng cũng cho thấy baseline phải đo lại vì mẫu cao hơn nhiều so với con số ước tính.

---

## 7. Tài liệu tham khảo

-
