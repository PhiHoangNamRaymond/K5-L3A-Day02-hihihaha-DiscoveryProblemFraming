# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: hihihaha
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): #12 — Khi lập báo cáo tuần, kỹ sư sản phẩm tại nhà máy sản xuất mạch điện tử mất khoảng 70 phút mỗi tuần để tra số lượng sản xuất và đưa số liệu vào đúng mục trong biểu mẫu.
- Quyết định cuối: Go / Not Yet / No-Go

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

Các câu có nhãn **Dự kiến** là bản nháp. Sau lượt phản biện, nhóm cập nhật câu thực tế và người hỏi vào đúng dòng.

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Nguyen Tien Dat | Import Excel sổ quỹ: Khi làm task import Excel cho sổ quỹ tiền mặt, tôi muốn xác định đúng dữ liệu và cột ngay từ đầu, để không phải sửa lại file sau khi test | Thực tập sinh dev (MobifoneIT), mentor, BA | Map cột Excel (~40 phút/lần) | **Nguyễn Bá Thành:** Trong lần gần nhất, điều gì khiến bạn mất nhiều thời gian nhất khi map cột Excel? |
| 2 | Nguyen Tien Dat | Vẽ diagram đồ án: Khi vẽ diagram cho bài tập/đồ án, tôi muốn ra đúng cấu trúc ngay bản đầu, để không phải sửa nhiều vòng theo feedback | Sinh viên năm cuối, bạn cùng nhóm | Sửa diagram theo feedback (~20–25 phút/lần, 2 vòng) | |
| 3 | Nguyen Tien Dat | Đọc hiểu task Jira: Khi nhận task mới trên Jira, tôi muốn hiểu đúng yêu cầu và tài liệu liên quan trong một lần đọc, để không làm sai hướng rồi phải hỏi lại mentor | Thực tập sinh dev, mentor, BA | Đọc tài liệu nội bộ + đối chiếu (~35 phút/lần) | **Dự kiến – Nam:** Trong lần gần nhất, phần lớn 35 phút mất ở bước tìm tài liệu hay ở bước đối chiếu yêu cầu trên Jira? |
| 4 | Phí Hoàng Nam | Tổng hợp đầu việc lab. Khi nhận bài lab, tôi muốn xác định các đầu việc, thứ tự thực hiện và yêu cầu nộp để bắt đầu làm mà không bỏ sót phần bắt buộc. | Học viên làm bài lab | Đọc checkpoint và tổng hợp yêu cầu từ nhiều tệp Markdown (ước tính 15 phút, cần đo lại). | **Dự kiến – Huy:** Trong 30 phút chuẩn bị bài Day 1, riêng việc đọc và tổng hợp yêu cầu mất bao lâu nếu tách thời gian tìm hiểu Colab? |
| 5 | Phí Hoàng Nam | Tìm link Phoenix. Khi chuẩn bị gửi stand-up buổi sáng, tôi muốn tìm được link Phoenix để gửi bài trước 10 giờ và nhận XP. | Học viên cần gửi stand-up | Tìm lại tin nhắn chứa link Phoenix (khoảng 2 phút ở lần gần nhất). | **Nguyễn Bá Thành:** Lần gần nhất tìm link Phoenix, bạn đã tìm ở đâu và mất khoảng bao lâu? |
| 6 | Phí Hoàng Nam | Theo dõi thông báo trên Outlook và Discord. Khi kiểm tra thông báo của chương trình, tôi muốn nhận ra những thông tin có việc cần làm để không bỏ lỡ yêu cầu hoặc thời hạn. | Học viên theo dõi thông báo của chương trình | Xác định thông báo nào có việc cần làm (ước tính 7 phút, cần kiểm tra xem có phải bước dẫn đến bỏ sót hay không). | |
| 7 | Nguyễn Bá Thành | Sau họp nhóm, tôi muốn rõ việc, người phụ trách và hạn để không phải hỏi lại. | Thành viên nhóm; nhóm trưởng | Hỏi lại thông tin sau họp: 5 lần từ 3 thành viên; chưa rõ thuộc bao nhiêu buổi. | **Dự kiến – Đạt:** Năm lượt hỏi lại xảy ra trong bao nhiêu buổi họp, và mọi người thường phải hỏi lại thông tin gì? |
| 8 | Nguyễn Bá Thành | Sau mỗi buổi LEC, tôi muốn tìm đủ link học tập để tiếp tục làm bài. | Học viên | Tìm lại link bài giảng, GitHub và nộp bài: khoảng 10 phút/buổi. |  |
| 9 | Nguyễn Bá Thành | Đầu ngày, tôi muốn nắm lịch và việc cần làm để chủ động sắp xếp. | Học viên; thành viên nhóm | Tổng hợp lịch học, việc nhóm, workshop/Office Hours: khoảng 10 phút/ngày. | |
| 10 | Nguyễn Văn Huy | Khi chuẩn bị weekly report, tôi muốn xác định 3 mã lỗi test xuất hiện nhiều nhất trong tuần, để tập trung báo cáo các lỗi chính | PE tại nhà máy sản xuất mạch điện tử | Tải file Excel từ phần mềm test và lọc, xếp hạng mã lỗi mất khoảng 60 phút mỗi tuần | **Nguyễn Bá Thành:** Trong 60 phút lọc và xếp hạng mã lỗi, bước nào mất nhiều thời gian nhất? |
| 11 | Nguyễn Văn Huy | Khi viết weekly report, tôi muốn xác định action phù hợp cho từng mã lỗi cũ và mới theo từng sản phẩm, để báo cáo có hướng xử lý rõ ràng | PE tại nhà máy sản xuất mạch điện tử | Viết action cho lỗi cũ mất khoảng 20 phút và lỗi mới khoảng 30 phút mỗi tuần | |
| 12 | Nguyễn Văn Huy | Khi tổng hợp weekly report, tôi muốn tra cứu số lượng sản xuất của tuần trước và đưa dữ liệu vào đúng mục, để báo cáo đầy đủ và hạn chế nhập sai | PE tại nhà máy sản xuất mạch điện tử | Tra số lượng mất khoảng 20 phút và copy-paste dữ liệu vào form báo cáo mất khoảng 50 phút mỗi tuần | **Dự kiến – Thành:** Trong lần lập báo cáo tuần gần nhất, phần nào tốn thời gian nhất trong 50 phút điền form: tìm đúng mục, chép số liệu hay kiểm tra lại? |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A — Xử lý dữ liệu và hoàn thiện báo cáo | #1, #10, #11, #12 | Mất thời gian đối chiếu cột dữ liệu, lọc mã lỗi, xác định hướng xử lý hoặc điền số liệu vào đúng mục báo cáo. |
| B — Làm rõ yêu cầu và đầu việc | #2, #3, #4, #7 | Phải đọc lại tài liệu, hỏi thêm hoặc sửa qua nhiều vòng để hiểu yêu cầu, việc cần làm và ai phụ trách. |
| C — Tìm và theo dõi thông tin | #5, #6, #8, #9 | Link, lịch và thông báo nằm ở nhiều nơi, khiến người dùng mất thời gian tìm lại hoặc dễ bỏ sót việc cần làm. |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME — Giảm số phút tìm, hiểu và tổng hợp thông tin cho mỗi đầu việc
├── Opportunity A — Mất thời gian đối chiếu, lọc và điền số liệu vào đúng chỗ
├── Opportunity B — Phải hỏi lại hoặc sửa nhiều vòng vì yêu cầu và trách nhiệm chưa rõ
└── Opportunity C — Mất thời gian tìm lại link, lịch và thông báo nằm rải rác
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- Form Excel dùng công thức tra cứu để tự điền số liệu (#12) là một phương án giải quyết. Vấn đề ở nhánh A là thời gian Huy mất để tra và điền số liệu.

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| #12 — Tra số liệu và điền báo cáo tuần (Huy) | 5 | 5 | 3 | 5 | 4 | 4 | 3 | **29** |
| #7 — Làm rõ đầu việc sau họp nhóm (Thành) | 5 | 3 | 3 | 3 | 4 | 4 | 5 | **27** |
| #8 — Tìm lại link sau buổi học (Thành) | 5 | 4 | 3 | 4 | 5 | 2 | 5 | **28** |

Mức điểm phản ánh dữ kiện hiện có. #12 có thể đo riêng thời gian tra số lượng và điền biểu mẫu. Nhóm quen bối cảnh của #7 và #8 hơn, còn số liệu hiện có của cả ba đề tài cần được kiểm chứng.

**Candidate được chọn** — #12 của Nguyễn Văn Huy, đạt 29/35 điểm.

**Vì sao chọn** — Công việc lặp lại hằng tuần và có số liệu ban đầu
cho hai bước cụ thể: khoảng 20 phút tra số lượng sản xuất và 50 phút
điền form. Nhóm có thể kiểm chứng thời gian từng bước ở CP4.

**Vì sao loại #7** — Có 5 lượt hỏi lại từ 3 thành viên, nhưng chưa rõ
xảy ra trong bao nhiêu buổi họp và làm mất thêm bao nhiêu thời gian.

**Vì sao loại #8** — Ước tính 10 phút mỗi buổi đang gộp việc tìm link
bài giảng, GitHub và nơi nộp bài. Chưa rõ bước nào chiếm nhiều thời
gian nhất để khoanh phạm vi kiểm chứng.

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | PE khác trong nhà máy (không chỉ Huy) cũng mất ≥60 phút/tuần cho báo cáo tuần | Value | 5 | 2 | ✅ |
| 2 | Bước tốn thời gian nhất là chép số liệu vào form (50 phút), không phải tra số lượng (20 phút) | Value | 5 | 2 | ✅ |
| 3 | File số lượng xuất ra từ phần mềm test có cấu trúc cột ổn định giữa các tuần | Feasibility | 4 | 3 | ✅ (kiểm tra file thật của Huy) |
| 4 | Biểu mẫu báo cáo tuần dùng ô/mục cố định, map được từ cột dữ liệu | Feasibility | 4 | 3 | ✅ |
| 5 | Nhà máy cho phép chạy công cụ ngoài (Power Query/Python) trên máy và dùng dữ liệu nội bộ | Viability | 5 | 1 | Hỏi sau (quy định IT) |
| 6 | PE muốn tự kiểm số liệu trước khi nộp nên cần hỗ trợ (augment) hơn là giao hẳn (automate) | Usability | 4 | 2 | ✅ |

Giả định nhóm kiểm chứng trong buổi này: **#1, #2, #6** — đều nằm ở ô "quan trọng nhưng ít bằng chứng".

### 3.2. Kiểm chứng

Cách đã dùng: **Survey 5–10 người** (đồng nghiệp PE/QA cùng nhà máy và bạn học có lập báo cáo định kỳ).

Bộ câu hỏi survey — hỏi **hành vi đã xảy ra**, không hỏi giả định, không có câu dạng "Bạn có muốn…":

1. Công việc của bạn có phải lập báo cáo định kỳ (tuần/tháng) không? (Có / Không)
2. Lần gần nhất lập báo cáo tuần, bạn mất tổng bao nhiêu phút?
3. Trong đó bước nào tốn thời gian nhất? (tra/tìm số liệu · chép số liệu vào form · viết nhận xét/action · kiểm tra lại · khác)
4. Số liệu sản xuất bạn lấy từ đâu? (phần mềm test xuất Excel · MES/hệ thống · hỏi bộ phận khác · khác)
5. Bạn điền form bằng cách nào? (copy-paste tay · công thức Excel · macro · công cụ khác)
6. Bạn lập báo cáo bao nhiêu lần mỗi tuần/tháng?
7. Trong 4 tuần gần nhất, có tuần nào bạn nhập sai số hoặc nộp trễ không? Chuyện gì đã xảy ra?
8. Bạn từng dùng công cụ nào (Power Query, macro, phần mềm SPC/MES…) để giảm thời gian chưa? Kết quả ra sao?

Kết quả survey: _(chưa thu thập — điền sau khi có phản hồi thật; không bịa số liệu.)_

*Nếu bổ sung phỏng vấn, mỗi buổi ghi một Interview Snapshot theo bảng dưới (hoặc đặt file trong `report/assets/cp4-interview-snapshot-N.md`):*

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | |
| Câu nói đáng nhớ nhất (nguyên văn) | |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | |
| Hiện đang xử lý bằng cách nào (workaround)? | |
| Mất bao lâu, bao lần? | |
| Insight / opportunity rút ra | |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| Survey (đồng nghiệp PE/QA) | _ | _ | _(bắt buộc ghi ≥1 tín hiệu phản bác, dù nhỏ)_ |

**Nhóm đã sửa problem thế nào sau kiểm chứng:** _(điền sau khi có kết quả — ví dụ nếu đa số nói bước tốn nhất không phải chép số liệu thì phải thu hẹp lại phạm vi)_

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Excel Power Query — connector Folder (gộp nhiều file tự động) | https://learn.microsoft.com/en-us/power-query/connectors/folder | Bước tra/gom số lượng sản xuất (~20 phút): tự đọc mọi file cùng cấu trúc trong một thư mục, Refresh khi có file mới | Có sẵn trong Excel; "Combine & Load/Transform" gộp file không cần code | File nguồn phải cùng định dạng/cấu trúc (sheet/table, header); phần mềm test đổi layout là query lỗi; không tự quyết số liệu thuộc mục nào của form | Dùng tốt cho bước gom số liệu nếu file export ổn định; vẫn cần rule map sang đúng mục + người kiểm |
| xlwings Reports (template → Excel/PDF) | https://docs.xlwings.org/en/0.24.4/reports.html | Bước điền form báo cáo (~50 phút): ghi DataFrame vào ô/bảng template có sẵn, xuất Excel/PDF | Tách code xử lý và template; người dùng tự sửa layout; hỗ trợ bảng, chart, ảnh, PDF | Tính năng Reports cần xlwings **PRO** (trả phí); cần Python + setup; có thể bị chặn script trên máy văn phòng | Pattern "template + engine điền" đúng hướng, nhưng phải kiểm chi phí/quy định IT; có thể thay bằng Excel-native (Power Query + công thức) |
| InfinityQS ProFicient (SPC real-time) | https://help.infinityqs.com/help/en/ProFicient/ | Thu thập dữ liệu chất lượng tự động + kho dữ liệu tập trung: thay việc lọc/xếp hạng mã lỗi thủ công (#10) và nhập tay | Kết nối nhiều nguồn nhà máy (OPC, file phẳng, DB…), thu thập tự động, báo cáo/dashboard real-time | Giải pháp cấp nhà máy, chi phí & triển khai lớn; cần tích hợp MES/ERP; quá tầm cho báo cáo tuần của một PE | Thế giới đã có giải pháp mạnh nhưng đắt; phạm vi lab nên chọn mức nhẹ (Rule/Power Query) thay vì mua SPC |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Tần suất: mỗi tuần, khi PE lập báo cáo tuần. 

```text
[PE] Tra số lượng sản xuất tuần trước từ dữ liệu nguồn (20')
  Input: dữ liệu sản xuất của tuần trước
  Output: số lượng cần đưa vào báo cáo
  → [PE] Mở biểu mẫu báo cáo và copy-paste số liệu vào đúng mục (50')
      Input: số lượng đã tra + biểu mẫu báo cáo tuần
      Output: biểu mẫu có số liệu sản xuất
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Handoff |
|---:|---|---|---|---|---|
| 1. Tra số lượng sản xuất tuần trước | PE | Dữ liệu sản xuất của tuần trước | Số lượng sản xuất cần báo cáo | Khoảng 20 phút / tuần (ước tính Huy, CP3) | PE chuyển số liệu sang bước điền biểu mẫu |
| 2. Điền số liệu vào đúng mục | PE | Số lượng đã tra và biểu mẫu báo cáo tuần | Biểu mẫu có số liệu sản xuất | Khoảng 50 phút / tuần (ước tính Huy, CP3) | PE hoàn thiện biểu mẫu để tiếp tục quy trình báo cáo hiện có |

**Bottleneck chính:** Bước 2 — copy-paste số liệu vào đúng mục của biểu mẫu, khoảng 50 phút mỗi tuần theo ước tính của Huy. Chưa có log bấm giờ hoặc dữ liệu kiểm chứng độc lập; cần xác nhận trong pilot.

### 4.2. Quy trình tương lai

Đề xuất thử trước bằng quy tắc/Excel (Power Query và biểu mẫu), không cần AI để tra hay tính số liệu. Thời gian từng bước là mục tiêu giả thuyết để kiểm tra, không phải kết quả đã đo.

```text
[PE] Đưa file nguồn đúng kỳ vào thư mục đã thống nhất (3')       ← CON NGƯỜI
  → [Power Query / rule] Refresh và gom số lượng (5')            ← RULE
  → [Rule / biểu mẫu] Ánh xạ số lượng vào các mục báo cáo (5')    ← RULE
  → [PE] Đối chiếu số trong biểu mẫu với nguồn và sửa nếu cần (12') ← CON NGƯỜI / HITL
  → [PE] Hoàn tất và gửi theo quy trình hiện tại (5')              ← CON NGƯỜI

BOUNDARY: Rule chỉ đọc file nguồn đã chọn và điền theo mapping đã xác nhận;
không tự suy đoán số thiếu, không ghi đè dữ liệu nguồn, không tự gửi báo cáo.
Nếu sau này thêm AI, AI không được tự tạo/sửa số liệu hay tự gửi; PE phải đối chiếu
mọi số liệu với nguồn trước khi đầu ra được dùng.
PHƯƠNG ÁN QUAY VỀ: Nếu file đổi cấu trúc, mapping sai hoặc kết quả không khớp,
dừng dùng kết quả tự động; PE tra và điền thủ công theo quy trình hiện tại,
đồng thời ghi nhận lỗi để sửa mapping trước lần chạy sau.
```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | 2 | 5 | Tương lai tách riêng nạp file, gom số, ánh xạ, kiểm tra và gửi |
| Tổng thời gian | Khoảng 70 phút / tuần | Mục tiêu khoảng 30 phút / tuần | Baseline = 20' + 50' theo ước tính ở CP3; thời gian tương lai là giả thuyết cần pilot |
| Số bước thủ công | 2/2 | 3/5 | PE nạp file, kiểm tra kết quả và gửi; 2 bước xử lý bằng rule |
| Bottleneck chính | Điền biểu mẫu (khoảng 50') | Đối chiếu số liệu (mục tiêu 12') | Dành thời gian cho kiểm soát chất lượng; phải đo lại khi pilot |
| Rủi ro mới phát sinh | — | File đổi cấu trúc hoặc mapping sai làm điền nhầm mục/số | Đối chiếu với file nguồn; dừng và quay về quy trình thủ công nếu không khớp |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | PE tại nhà máy sản xuất mạch điện tử, phụ trách tổng hợp số lượng sản xuất vào báo cáo tuần. |
| **Quy trình** | Mỗi tuần, PE tra số lượng sản xuất của tuần trước từ dữ liệu nguồn rồi điền số liệu vào đúng mục trong biểu mẫu báo cáo. |
| **Bottleneck** | Điền/copy-paste số liệu vào đúng mục của biểu mẫu, ước tính khoảng 50 phút mỗi tuần theo thông tin Huy nêu ở CP3; chưa được bấm giờ độc lập. |
| **Impact** | Quy trình tra và điền số liệu chiếm khoảng 70 phút mỗi tuần theo ước tính ban đầu (20 phút tra + 50 phút điền). Nếu sai số hoặc điền nhầm mục, báo cáo có thể không chính xác; mức độ và tần suất lỗi chưa được xác minh. |
| **Success Metric** (baseline → target, cách đo) | Baseline tạm tính khoảng 70 phút/tuần (ước tính CP3) → mục tiêu không quá 30 phút/tuần. Trong 4 tuần lập báo cáo, PE bấm giờ từ lúc bắt đầu tra dữ liệu đến khi hoàn tất phần số liệu; ghi riêng thời gian từng bước, số lần sửa và số mục sai/thiếu khi đối chiếu với nguồn. Chỉ đạt mục tiêu nếu giảm thời gian mà không tăng lỗi; xác nhận baseline bằng lần đo đầu tiên. |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | CP5 chưa đề xuất dùng AI để xử lý số liệu. Rule chỉ gom và ánh xạ dữ liệu theo nguồn/mapping đã xác nhận; không suy đoán hoặc sửa số liệu nguồn, không tự gửi báo cáo. PE phải đối chiếu số và mục trong biểu mẫu với nguồn trước khi hoàn tất. Nếu sau này dùng AI, AI không được tự tạo/sửa số liệu hay tự gửi; đầu ra phải được PE kiểm tra. |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

- Phản biện: Baseline khoảng 70 phút hiện là ước tính tự báo cáo, chưa phải số đo; target thời gian đơn lẻ có thể khuyến khích điền nhanh nhưng kém chính xác. Cần đo baseline bằng bấm giờ và theo dõi lỗi/sửa trong pilot.
- Trạng thái: Đã đưa cách đo và kiểm tra lỗi vào Success Metric v0; nhóm cần xác nhận/điều chỉnh sau khi có số liệu pilot. Chưa ghi nhận phản biện từ nhóm khác.

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô:

Vì sao:

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | | | | |
| **Rule** | | | | |
| **Workflow** | | | | |
| **Agent** | | | | |

**Mức chọn:**

**Vì sao không chọn mức đơn giản hơn:**

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | |
| **Judgment** — con người cân nhắc, quyết định gì? | |
| **Action** — hành động cuối cùng là gì, ai làm? | |
| **Outcome** — đo kết quả bằng gì? | |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng:
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào:

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** | |
| **AI intervention point** | |
| **Mức chọn** | No AI / Rule / Workflow / Agent |
| **Rủi ro & người kiểm tra** | |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| | | | |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | | | |
| 2 | | | |
| 3 | | | |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | | |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | | |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | | |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | | |

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
