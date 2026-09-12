# 01 — Individual Problem Scan

> Điền theo Phase 1 + Phase 2 trong `01-worksheet.md`. Tự scan trước, dùng AI sau để phản biện. Không copy ví dụ Weekly Report.

## Thông tin cá nhân

- Họ và tên:
- Mã học viên:
- Vai trò / bối cảnh (VD: sinh viên năm X, intern PM, ...):
- Công việc hằng tuần (3-5 gạch đầu dòng để soi problem):

---

## Phase 1 — Scan 5+ problems (tối thiểu 5, khuyến khích 8-10)

**Cách điền:** mỗi dòng = việc gì + ai chịu + đo bằng gì. Cột `Dấu hiệu thật` bắt buộc có số: mất bao lâu (bấm giờ mấy lần), mấy lần/tuần, bao nhiêu người gặp, log/ticket/quote nào.

| # | Lăng kính (Lặp lại / Tốn thời gian / AI có thể tốt hơn / Pain từ người khác) | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật (số + bằng chứng) |
|---|---|---|---|---|
| 1 | AI có thể tốt hơn | Người đi đường đi vào đường bị ngập vào mỗi khi trời mưa ngập lụt | Người tham gia giao thông, tài xế | Xe chết máy, mất nửa ngày đi sửa |
| 2 | Lặp lại | Mỗi ngày phải tập hợp task trên Jira về Google doc cho team | PM, Team Lead| Mất 10-15 phút mỗi sáng, lặp lại hàng ngày |
| 3 | Lặp lại | Khi có thông báo trên khóa học thì ban tổ chức cần phải thông báo ở nhiều nền tảng | Ban tổ chức, Admin, Trợ giảng | Mất 20-30 phút mỗi lần |
| 4 | AI có thể tốt hơn | Đặt lịch đi chơi vào ngày có khả năng mưa bão | Khách du lịch, người lên kế hoạch | Phải hủy chuyến, mất tiền cọc khách sạn/vé máy bay, mất nửa ngày đến vài ngày ở trong nhà |
| 5 | Tốn thời gian | Tìm kiếm tài liệu đã được nhắc đến từ lâu dựa trên 1 keyword trên Jira và slack | Cả team | Mất 20-40 phút lội lịch sử chat/ticket, đôi khi bế tắc phải hỏi lại người khác |

> Gợi ý tự soi: tuần trước mất nhiều thời gian nhất vào việc gì? Việc gì hay trì hoãn? Người khác hay hỏi lại câu gì? Workflow nào ai cũng biết là chậm?

**AI đã dùng ở Phase 1 (nếu có):**
- Prompt đã hỏi: 
- Ý dùng được:
- Ý bỏ vì không phải pain thật:

**Self-check Phase 1:**
- [x] Đủ 5+ dòng, mỗi dòng có actor + số đo cụ thể
- [x] Dùng ít nhất 3/4 lăng kính
- [x] Không có dòng chung chung kiểu "mất nhiều thời gian"

---

## Phase 2 — Top 3 Problem Cards

### 2.1. Chọn top 3

Giữ bài nào: actor cụ thể, workflow vẽ được 3-7 bước, bottleneck ở 1 bước, impact đo được. Loại bài quá rộng.

| Rank | Problem (copy từ bảng scan) | Vì sao chọn (2-3 ý) | Điều còn chưa chắc |
|---|---|---|---|
| 1 | Người đi đường đi vào đường bị ngập vào mỗi khi trời mưa ngập lụt| Đây là vấn đề khi có mưa to xảy ra ở Hà Nội mà mình hay gặp phải. Đi làm về không biết phải đi đường nào để đảm bảo xe mình có thể đi được về nhà | Chưa chắc các hệ thống cảnh báo giao thông và thiên tai hiện giờ có thể cảnh báo người dùng tới đâu |
| 2 | Mỗi ngày phải tập hợp task trên Jira về Google doc cho team | Hàng ngày mình là người tạo doc và rà soát task trong team QA của mình. Mình thấy việc này lặp lại rất nhiều và phải tổng hợp ở nhiều dashboard khác nhau | Vấn đề này có cách giải quyết khác như là làm lại cái dashboard trên Jira |
| 3 | Khi có thông báo trên khóa học thì ban tổ chức cần phải thông báo ở nhiều nền tảng | Mỗi khi thông báo 1 thay đổi mới trong khóa học, ban tổ chức phải thông báo ở rất nhiều nền tảng, có những bạn sẽ bị miss thông tin nếu không thông báo đủ nền tảng | Có thể đã có những agent giải quyết được vấn đề này 1 cách xuất sắc |

### 2.2. Problem Cards chi tiết (lặp lại cho cả 3 cards)

---

#### Problem Card #1 — [Tên problem]

```text
Problem 1 câu:
Người đi đường đi vào đường bị ngập vào mỗi khi trời mưa ngập lụt

Actor:
Người tham gia giao thông, tài xế

Thời điểm / bối cảnh:
Thời điểm mưa to dẫn đến ngập lụt trong thành phố.

Current workflow 3-7 bước: 
1. Người đi xe đi ra đường sau khi trời mưa to
2. Lái xe di chuyển theo lộ trình quen thuộc hoặc sử dụng ứng dụng bản đồ thông thường (không có dữ liệu ngập lụt theo thời gian thực).
3. Tiến đến gần đoạn đường bị ngập nhưng không nhận được cảnh báo từ trước.
4. Nếu quyết định đi qua, xe có rủi ro cao bị chết máy giữa dòng nước ngập, gây hư hỏng tài sản. Nếu không đi qua thì người tham gia giao thông sẽ tìm hướng di chuyển khác.

Bottleneck:
Bước 7 -- Nếu đi qua thì sẽ có thể hỏng xe, không đi qua thì sẽ phải mất thời gian tìm đường khác

Impact:
1 đến 2 giờ ngoài đường

Success metric:
Giảm được từ 1 đến 2 tiếng xuống còn 30 phút khi người tham gia giao thông chủ động đi đường khác

Non-AI alternative:
Nghe kênh VOV Giao thông hoặc theo dõi các nhóm cộng đồng trên mạng xã hội để cập nhật điểm ngập thủ công.

AI hypothesis:
Nếu sử dụng mô hình Computer Vision phân tích luồng camera giao thông công cộng để tự động nhận diện mức độ ngập lụt theo thời gian thực, sau đó tích hợp vào API bản đồ để tự động định tuyến lại lộ trình, thì tỷ lệ xe cộ đi vào đường ngập sẽ giảm đáng kể.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[ ] Workflow
[ ] Agent
[x] Chưa biết
```

**Draft workflow Card #1** (ASCII / Mermaid / ảnh đính kèm):

```text
CURRENT STATE — 120 phút

[1 Người đi xe đi ra đường sau khi trời mưa to: 5'] 
→ [2 Lái xe di chuyển theo lộ trình quen thuộc hoặc sử dụng ứng dụng bản đồ thông thường (không có dữ liệu ngập lụt theo thời gian thực). : 15'] 
→ [3 Tiến đến gần đoạn đường bị ngập nhưng không nhận được cảnh báo từ trước: 15'] 
→ [4 Tìm hướng di chuyển khác: 85']  <-- bottleneck

FUTURE STATE — 70 phút

[1 Người đi xe đi ra đường sau khi trời mưa to: 5'] 
→ [2 Người lái xe nhập cung đường mình muốn di chuyển: 5'] 
→ [3 AI đánh giá và gợi ý cung đường khác nếu đường đi ban đầu đang gặp tình trạng ngập lụt hoặc tắc do ngập lụt: 60']

Fallback: nếu AI sai thì người dùng mất thời gian đi đường vòng.
```

File đính kèm (nếu vẽ riêng):

---

#### Problem Card #2 — [Tên problem]
Mỗi ngày phải tập hợp task trên Jira về Google doc cho team

```text
Problem 1 câu:
Mỗi ngày sẽ phải có 1 người tập hợp task trên Jira về Google doc cho team.

Actor:
PM, Leader.

Thời điểm / bối cảnh:
Buổi sáng mỗi ngày làm việc.

Current workflow 3-7 bước:
1. Leader tạo doc.
2. Check tasks ở các dashboard khác nhau cho team.
3. Tạo Google doc
4. Tổng hợp các tasks vào Google doc

Bottleneck:
Bước 2 -- Check tasks ở các Dashboard khác nhau là 1 công việc lặp đi lặp lại.

Impact:
10 đến 15 phút mỗi ngày làm việc

Success metric: 
Giảm từ 10 đến 15 phút xuống 5 phút mỗi ngày

Non-AI alternative:
Leader tự tổng hợp task vào doc.

AI hypothesis:
Nếu thiết lập một workflow tự động kết hợp AI (ví dụ: dùng Zapier/Make kết nối Jira API với ChatGPT) để tự động đọc, lọc và tóm tắt các task đang mở/cần ưu tiên từ nhiều dashboard khác nhau trên Jira, sau đó điền sẵn vào template trên Google Docs mỗi sáng, thì PM/Leader sẽ chỉ mất dưới 5 phút để review và chỉnh sửa thay vì phải copy/paste thủ công từng mục.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #2:**

```text
CURRENT STATE — 15 phút

[1 Leader tạo doc ] 
→ [2 Check tasks ở các dashboard khác nhau cho team ] <-- bottleneck
→ [3 Tạo Google doc ]
→ [4 Tổng hợp các tasks vào Google doc ]

FUTURE STATE — 5 phút

[1 Người dùng prompt Agent] 
→ [2 Agent tổng hợp thông tin và tạo doc]

Fallback: Nếu AI sai thì người dùng phải tự thêm tasks vào doc
```

File đính kèm: 

---

#### Problem Card #3 — [Tên problem]
Khi có thông báo trên khóa học thì ban tổ chức cần phải thông báo ở nhiều nền tảng

```text
Problem 1 câu: 
Mỗi khi thông báo 1 thay đổi mới trong khóa học, ban tổ chức phải thông báo ở rất nhiều nền tảng, có những bạn sẽ bị miss thông tin nếu không thông báo đủ nền tảng

Actor: 
Ban tổ chức khóa học

Thời điểm / bối cảnh:
Khi khóa học có thông báo mới

Current workflow 3-7 bước:
1. Có thông báo mới
2. Ban tổ chức phải thông báo trên nhiều nền tảng khác nhau
3. Học viên check thông báo

Bottleneck:
Bước 2 -- Ban tổ chức phải copy thông báo đó gửi đi trên nhiều nền tảng khác nhau và đảm bảo là không bị thiếu nền tảng nào.

Impact:
10-15 phút mỗi lần thông báo

Success metric:
Giảm từ 10-15 phút xuống còn 2-3 phút mỗi lần.

Non-AI alternative: 
Ban tổ chức khóa học gửi thông báo trên các nền tảng 1 cách thủ công.

AI hypothesis:
Nếu sử dụng công cụ tự động hóa kết hợp AI (LLM) để tiếp nhận nội dung gốc từ một nguồn duy nhất (ví dụ: điền vào Google Form hoặc Notion) và tự động đăng tải đồng loạt, thì ban tổ chức sẽ chỉ mất 1-2 phút nhập liệu ban đầu mà không sợ bỏ sót nền tảng.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #3:**

```text
CURRENT STATE — 15 phút

[1 Có thông báo mới] 
→ [2 Ban tổ chức phải thông báo trên nhiều nền tảng khác nhau] <-- bottleneck
→ [3 Học viên check thông báo] 

FUTURE STATE — 3 phút

[1 Có thông báo mới] 
→ [2 Ban tổ chức cho thông báo lên Google Form] 
→ [3 AI tự động gửi thông báo đến những nền tảng được thiết lập sẵn]
→ [4 Học viên check thông báo]

Fallback: Người dùng tự gửi thông báo trên các nền tảng
```

File đính kèm: 

---

### 2.3. Card muốn pitch nhất (chuẩn bị 2 phút)

**Card tôi muốn pitch nhất:**

```text
Card 1: Người đi đường đi vào đường bị ngập vào mỗi khi trời mưa ngập lụt

``` 

**Vì sao (2-3 câu: workflow gì, số đo gì, impact gì):**

```text
Vì đấy là vấn đề thiết thực mà mình thường xuyên gặp phải.

```

**Câu hỏi tôi muốn nhóm challenge (1-2 câu hỏi đúng chỗ yếu):**

```text
Câu 1: Hiện giờ có giải pháp gì khác cho vấn đề này không?
Câu 2: Có dễ thực hiện không?
```

**AI phản biện Card (nếu có):**
- Điểm yếu AI chỉ ra:
- Tôi sửa gì:

### Self-check nộp phần 01
- [x] Có 5+ problems + top 3 Cards đủ field
- [x] Mỗi Card có workflow trước/sau + bottleneck + metric + fallback
- [x] Đã chọn 1 card pitch + câu hỏi challenge
