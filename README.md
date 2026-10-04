# Track 1 — Day 17 — Case A: AI Tutor: Diagnostic Refresher

## 1. Thông tin cá nhân và nhóm

- MHV: 2A202602554
- Họ và tên: Nguyễn Anh Dũng
- Tên nhóm: FinTech
- Thành viên nhóm (họ tên và MHV): Tạ Việt Cường - Nguyễn Văn Thăng 
- Lớp / học phần: Track 1
- Case đã chọn: Case A — AI Tutor: Diagnostic Refresher.
- Người thực hiện lượt phỏng vấn: Nguyễn Anh Dũng
- Người được phỏng vấn / mã ẩn danh: Ẩn Danh

Biên bản của lượt phỏng vấn nằm trong [interview/notes.md](interview/notes.md). Bản ghi gốc được đính kèm tại [interview/recording.m4a](interview/recording.m4a), thời lượng khoảng 3 phút 37 giây. Không nộp riêng transcript.

## 2. Problem Hypothesis Brief

### 1. Mô tả giải pháp ban đầu

Một AI tutor có thể cho learner báo rằng họ vẫn chưa hiểu một bài học, sau đó dùng một trao đổi chẩn đoán ngắn để xác định lỗ hổng kiến thức nền có thể có và hướng learner đến phần ôn lại phù hợp trước khi họ thử lại nội dung hiện tại.

Đây là **starting solution**, không phải finding hay feature để kiểm chứng trong problem interview.

### 2. Năng lực trung tính

Capability là hỗ trợ learner khôi phục sau khi bị đứt mạch hiểu bài: làm rõ điều đang cản trở tiến độ và kết nối họ với tài liệu học trước đó có liên quan.

### 3. Chuỗi thay đổi

| Thành phần solution | Thay đổi có thể xảy ra với learner | Assumption cần kiểm chứng |
| --- | --- | --- |
| Learner báo đang bối rối | Dừng lại đúng điểm không hiểu | Họ nhận ra và hành động khi bối rối thay vì tiếp tục hoặc bỏ cuộc |
| Trao đổi chẩn đoán ngắn | Phân biệt khó khăn ở bài hiện tại với lỗ hổng kiến thức nền | Xác định nguồn gốc khó khăn hiện đang tốn công |
| Lộ trình ôn lại có mục tiêu | Xem lại khái niệm phù hợp thay vì tìm kiếm lan man | Nguồn lực hiện tại không chỉ đúng phần cần học |
| Quay lại bài hiện tại | Tiếp tục tự tin hơn | Giải quyết lỗ hổng giúp cải thiện bước học tiếp theo |

### 4. Actor mục tiêu

**Primary actor:** learner tự học bằng tài liệu số/online, gần đây đã gặp bài học hoặc nhiệm vụ không hiểu đủ để tiếp tục.

**Không phải primary actor:** giảng viên, mentor, phụ huynh hoặc quản trị viên. Họ có thể xuất hiện trong workaround của learner, nhưng không phải đối tượng phỏng vấn chính.

### 5. Tình huống và giả thuyết việc cần hoàn thành

**Situation:** Trong khi học một khái niệm online, learner gặp điểm mà phần giải thích, ví dụ hoặc bài tập không đủ rõ để họ tiếp tục tự tin.

**Functional job:** Khi bị mắc ở một bài học, hãy giúp tôi xác định điều cần hiểu hoặc xem lại để tôi có thể tiếp tục nhiệm vụ học hiện tại.

**Bối cảnh cảm xúc/xã hội cần khám phá:** Learner có thể không chắc chắn, bực bội, ngại hỏi hoặc bị áp lực deadline. Đây là hướng cần khám phá, không phải evidence.

### 6. Giả thuyết về pain point

**Pain hypothesis A — diagnosis:** Learner nhận ra mình bị mắc nhưng không xác định đáng tin cậy được vấn đề nằm ở phần giải thích hiện tại, thuật ngữ lạ hay kiến thức nền bị thiếu.

**Pain hypothesis B — recovery:** Khi cố khắc phục, learner phải tìm kiếm, xem lại, hỏi người khác hoặc đoán qua nhiều nguồn; điều này làm chậm tiến độ hoặc khiến họ bỏ qua khi chưa hiểu.

### 7. Bản đồ evidence

| Thành phần giả thuyết | Evidence thuận mạnh cần tìm | Evidence có thể phản bác | Không xem là evidence |
| --- | --- | --- | --- |
| Learner bị mắc trong tình huống cụ thể | Câu chuyện gần đây, chi tiết, có bối cảnh và trình tự | Không nhớ được sự kiện phù hợp hoặc sự kiện rất hiếm | “Học có thể khó” |
| Learner không chẩn đoán được lỗ hổng | Mô tả sự không chắc chắn và nỗ lực cụ thể để tìm ra | Biết ngay phần bị thiếu và có cách xử lý tin cậy | Đồng ý rằng chẩn đoán nghe hữu ích |
| Recovery hiện tại tốn công | Timeline, nhiều nguồn/lần thử, chậm trễ hoặc hệ quả cụ thể | Đọc lại giải quyết nhanh, ít tốn công | Ý kiến rằng AI tutor sẽ hay |
| Pain đủ quan trọng | Dành thời gian/công sức, đi hỏi, chậm việc hoặc chịu hệ quả | Thường bỏ qua mà không ảnh hưởng đáng kể | Nói sẽ dùng feature tương lai |
| Vấn đề lặp lại | Có thêm sự kiện gần đây hoặc bối cảnh lặp lại rõ ràng | Chỉ là sự cố đơn lẻ/bất thường | Assumption của interviewer về tần suất |

### 8. Giả thuyết vấn đề

Với learner tự học online gần đây bị mắc ở một bài học, khó khăn trong việc xác định phần cần ôn lại có thể khiến quá trình khắc phục chậm hoặc không đáng tin cậy. Họ có thể đọc lại, tìm nguồn bên ngoài, hỏi người khác hoặc bỏ qua; nếu việc học quan trọng hoặc gấp, điều này có thể làm chậm tiến độ hay giảm sự tự tin.

**Falsifiable prediction:** Trong câu chuyện gần đây và cụ thể, participant sẽ mô tả hành động thực tế sau khi bị mắc. Giả thuyết yếu đi nếu họ luôn xác định được lỗ hổng và khắc phục nhanh nhờ cách ít tốn công sẵn có, hoặc nếu hệ quả không đáng kể.

### 9. Điều kiện biên cần kiểm tra

- Loại môn học, nội dung hoặc bài tập nào gây ra vấn đề?
- Vấn đề khác nhau thế nào giữa tự học và môn có deadline?
- Khi nào chỉ cần đọc lại là đủ?
- Khi nào learner muốn hỏi người thay vì tìm tài liệu?
- Khi nào bỏ qua một điểm chưa hiểu là hợp lý?

### 10. Các hướng giải pháp tạm để lại

Không pitch các hướng này trong problem interview. Chúng chỉ được lưu lại để tránh chốt solution quá sớm.

| Hướng | Dạng có thể có | Assumption được giải quyết |
| --- | --- | --- |
| Diagnostic prompts | Câu hỏi ngắn thu hẹp misconception hoặc prerequisite | Learner cần giúp xác định lỗ hổng |
| Concept map / prerequisite path | Lộ trình trực quan từ điểm mắc đến khái niệm trước đó | Learner cần định hướng giữa các khái niệm liên quan |
| Targeted refresher | Bài ôn/ví dụ minh họa ngắn được chọn lọc | Learner cần đúng tài liệu, không phải thêm tài liệu |
| Explain-back / practice check | Learner giải thích lại hoặc làm bài kiểm tra ngắn | Learner cần phản hồi xem đã khôi phục hiểu biết chưa |
| Human-help routing | Cách đặt và gửi câu hỏi rõ ràng đến bạn bè/thầy cô/mentor | Trong vài bối cảnh, người thật là kênh đáng tin nhất |

### 11. Quy tắc ra quyết định ở Chặng 1

Sau interview thật, chỉ phân loại giả thuyết là **được ủng hộ, hỗn hợp hoặc bị làm yếu** từ evidence có thể truy vết. Không coi một câu chuyện là bằng chứng về mức độ phổ biến. Ghi cả evidence thuận và nghịch trong Interview Record.

### 12. Đối chiếu sau phỏng vấn Day17

Giữ nguyên các giả thuyết trước phỏng vấn ở trên để thể hiện quá trình kiểm chứng. Kết quả từ bản chép lời được trình bày đầy đủ trong file 03:

- Có evidence tự thuật về nội dung chưa hiểu khi xem video và slide trong bài Job to be Done (01:13–01:34).
- Có cách xử lý hiện tại bằng trợ lý AI và hỏi người hỗ trợ khi cần (00:55–01:05; 02:02–02:08).
- Chưa có evidence cho thấy participant không xác định được kiến thức nền cần ôn. Không đồng nhất kiến thức mới với lỗ hổng prerequisite.
- Thời gian thường 1–2 phút, đôi khi 4–5 phút (02:29–02:32), làm yếu giả định rằng việc xử lý thường tốn nhiều thời gian.
- Hệ quả “để lại và tiếp tục” được hỏi theo giả định (02:45–03:01), nên chưa được xem là hành vi thực tế.

**Giả thuyết cần nghiên cứu tiếp:** Khi gặp khái niệm mới trong lúc xem video hoặc slide, learner muốn làm rõ ý nghĩa để tiếp tục theo dõi bài. Với những câu hỏi mà nguồn giải thích hiện tại chưa giải quyết được hoặc chưa đủ đáng tin, cần tìm hiểu cách họ kiểm tra câu trả lời và tìm hỗ trợ tiếp theo.

Đây là hướng nghiên cứu điều chỉnh, chưa phải kết luận rằng cần triển khai Diagnostic Refresher. Một lần phỏng vấn ngắn chưa đủ để đánh giá độ phổ biến hoặc mức độ nghiêm trọng.

## 3. Conversation Guide phiên bản cuối

Bản dưới được chỉnh sau phân tích lượt luyện Day17; chưa được thử trong lượt phỏng vấn tiếp theo. Nguồn điều chỉnh là bản chép lời có mốc thời gian do người thực hiện cung cấp.

### Nhật ký thay đổi

| Quan sát từ Day17 | Thay đổi | Mục đích |
| --- | --- | --- |
| 00:43–01:05: câu hỏi về lần gần nhất dẫn sang trả lời cách xử lý thông thường | Dùng thì quá khứ, nhắc “trong lần đó” | Thu được chuỗi hành vi của một sự kiện thật |
| 01:13–01:34: có bài học cụ thể nhưng chưa rõ điểm mắc | Hỏi đoạn/khái niệm nào và dấu hiệu nhận ra chưa hiểu | Tách thiếu giải thích hiện tại khỏi thiếu kiến thức nền |
| 02:24–02:38: có ước lượng thời gian nhưng chưa rõ lần gần nhất | Hỏi số lần thử, kết quả và thời gian trong sự kiện chính | Làm rõ công sức thay vì chỉ lấy số chung |
| 02:45–03:01: hỏi hệ quả theo giả định | Hỏi một lần thất bại đã xảy ra, nếu có | Thu hệ quả thực tế |
| 02:29 và 03:24: workaround có thể đã hiệu quả | Thêm câu hỏi về trường hợp xử lý nhanh và không cần hỏi thêm | Chủ động tìm phản chứng |
| 03:02–03:20: hội thoại lệch luồng | Chuẩn bị câu đưa trở lại mạch kể | Giữ tập trung mà không gây áp lực |

### Ba câu hỏi học hỏi chính

1. Khi gặp nội dung chưa hiểu trong một lần học gần đây, learner đã làm gì và có tiếp tục được không?
2. Rào cản nằm ở ý nghĩa khái niệm, cách giải thích, độ tin cậy của câu trả lời hay kiến thức nền? Dữ liệu nào trong câu chuyện cho phép phân biệt?
3. Cách xử lý hiện tại hiệu quả đến đâu, và khi nào vấn đề gây công sức hoặc hệ quả đáng kể?

### Tiêu chí tuyển người

Người ở ngoài nhóm, đang học bằng tài liệu số/online, có một sự kiện chưa hiểu nội dung trong 7 ngày qua và đồng ý ghi lại phỏng vấn. Không yêu cầu phải sử dụng AI; không tuyển dựa trên mức yêu thích giải pháp.

### Kịch bản khoảng 15 phút

#### Mở đầu và kiểm tra tiêu chí — 2 phút

“Cảm ơn bạn đã tham gia. Mình muốn hiểu cách bạn xử lý khi gặp nội dung khó hiểu trong lúc học. Không có câu trả lời đúng hay sai. Mình xin phép ghi âm để xem lại và làm bài lab; bạn có đồng ý không?”

“Trong 7 ngày qua, bạn có một lần cụ thể gặp nội dung chưa hiểu không? Lần gần nhất là khi nào?”

#### Một câu chuyện cụ thể — 3 phút

“Kể mình nghe lần đó từ lúc bạn bắt đầu gặp phần chưa hiểu nhé.”

- “Lúc đó bạn học nội dung gì, bằng tài liệu nào?”
- “Cụ thể đoạn hoặc khái niệm nào khiến bạn mắc?”
- “Bạn đang cố làm gì tiếp theo?”
- “Điều gì cho bạn biết mình chưa hiểu?”

#### Hành vi và kết quả — 4 phút

“Trong lần đó, việc đầu tiên bạn đã làm là gì?”

- “Sau đó chuyện gì xảy ra?”
- “Bạn đã hỏi hoặc tìm bằng nội dung nào?”
- Nếu họ kể dùng AI: “Câu trả lời đầu tiên giúp được gì? Bạn có hỏi lại không?”
- “Lúc đó bạn biết cần xem lại phần nào chưa? Bạn tìm ra bằng cách nào?”
- “Cuối cùng bạn tiếp tục được chưa? Bạn biết mình đã hiểu bằng cách nào?”
- “Lần đó mất khoảng bao lâu và bao nhiêu lần thử?”

#### Cách khác và hệ quả thực tế — 3 phút

“Có lần gần đây nào cách đầu tiên không giải quyết được không? Kể mình lần đó nhé.”

- Nếu có: “Bạn làm gì tiếp? Người hoặc nguồn khác giúp được thế nào?”
- “Cuối cùng chuyện gì xảy ra với việc học hoặc bài tập?”
- Nếu không có: ghi nhận các trường hợp đã được xử lý tốt; không ép kể thất bại.

#### Mẫu lặp lại, phản chứng và kết thúc — 3 phút

“Có lần nào bạn xử lý rất nhanh mà không cần hỏi thêm không? Lần đó khác gì?”

“Có lần nào bạn bỏ qua phần chưa hiểu mà vẫn tiếp tục được không? Chuyện gì xảy ra sau đó?”

“Trong lần chính vừa kể, phần mất công nhất là gì?”

“Có điều gì quan trọng mình chưa hỏi không? Cảm ơn bạn.”

### Câu hỏi đào sâu dùng linh hoạt

- “Trong lần đó cụ thể là thế nào?”
- “Bạn đã làm gì tiếp?”
- “Bạn có thể kể một ví dụ thật không?”
- “Bạn chọn cách đó vì điều gì?”
- “Kết quả cuối cùng là gì?”
- “Đó là điều đã xảy ra hay điều bạn nghĩ sẽ làm?”

Nếu lệch luồng: “Mình quay lại lần học bạn vừa kể nhé. Sau bước đó, bạn đã làm gì?”

### Nguyên tắc sử dụng

Ưu tiên một câu chuyện đầy đủ thay vì hỏi hết danh sách. Để participant tự nêu công cụ và rào cản trước. Không gợi ý họ bị hổng kiến thức nền, không pitch AI tutor và không coi câu trả lời giả định là hành vi thật. Thời gian là định hướng để có đủ chiều sâu.

### Checklist sau lần phỏng vấn tiếp theo

- [ ] Có một sự kiện cụ thể với chuỗi hành vi và kết quả.
- [ ] Có evidence về mức công sức và hệ quả thực tế.
- [ ] Đã hỏi phản chứng hoặc ghi nhận workaround hiệu quả.
- [ ] Quote được đối chiếu với bản ghi.
- [ ] Người thực hiện tự nghe lại và viết reflection.

## 4. Practice Reflection

Phần phản tư dưới đây dựa trên bản chép lời có mốc thời gian của lượt phỏng vấn Day17. Nhận xét tập trung vào cách đặt câu hỏi và dữ liệu thu được; không đánh giá giọng điệu hoặc khoảng lặng khi chưa đối chiếu âm thanh.

### 4.1. Điều làm tốt và giá trị của lượt luyện

Lượt phỏng vấn có phần mở đầu rõ ràng: giới thiệu mục đích tìm hiểu trải nghiệm, giải thích không có câu trả lời đúng hay sai và xin phép ghi lại. Participant đồng ý tại 00:19. Câu hỏi về 7 ngày gần đây giúp kiểm tra mức phù hợp; các câu hỏi tiếp theo xác định trải nghiệm liên quan đến bài Job to be Done, trong lúc xem video và slide (01:13–01:34).

Một điểm có ích là hỏi về cách xử lý hiện tại và thời gian cần bỏ ra. Lời kể về việc hỏi trợ lý AI, chuyển sang hỏi người hỗ trợ và thời gian thường 1–2 phút cho thấy learner đã có phương án khắc phục. Dữ liệu này giúp kiểm tra giả thuyết thay vì chỉ tìm câu trả lời thuận chiều. Cuộc phỏng vấn cũng không giới thiệu tính năng Diagnostic Refresher, nên không thu ý kiến về một giải pháp được gợi sẵn.

### 4.2. Điều chưa tốt và bài học rút ra

Hạn chế chính là chưa tái dựng đầy đủ một sự kiện. Câu hỏi tại 00:43 vừa nhắc “lần gần nhất” vừa dùng “sẽ giải quyết”, khiến participant chuyển sang kể cách làm thông thường. Sau khi xác định bài học ở 01:13–01:34, lượt phỏng vấn chưa làm rõ chính xác khái niệm chưa hiểu, câu hỏi đã gửi cho AI, câu trả lời nhận được và cách participant biết mình đã hiểu.

Câu hỏi tại 02:45 đưa ra giả định rằng cả hai cách đều thất bại. Vì vậy, câu trả lời về việc tiếp tục học và để lại nội dung chưa hiểu chỉ thể hiện phương án dự kiến, chưa chứng minh hệ quả thực tế. Ngoài ra, chưa có câu hỏi phản chứng yêu cầu kể một lần xử lý nhanh hoặc một lần bỏ qua mà không ảnh hưởng. Đoạn 03:02–03:20 lệch luồng, nhưng bản chép lời chưa đủ rõ để xác định người nói.

Thời lượng khoảng 3 phút 37 giây khiến nhiều thông tin còn thiếu. Bài học rút ra là cần theo sát một câu chuyện đến kết quả, đồng thời phân biệt hành vi đã xảy ra, cách làm thông thường và câu trả lời giả định. Sự xuất hiện của nội dung mới chưa đủ để kết luận learner bị hổng kiến thức nền.

### 4.3. Thay đổi cụ thể cho lượt tiếp theo

Bản guide cuối đã đổi câu mở sang “Kể mình nghe lần đó từ lúc bạn bắt đầu gặp phần chưa hiểu nhé”, sau đó dùng “Trong lần đó, việc đầu tiên bạn đã làm là gì?” và “Sau đó chuyện gì xảy ra?”. Các câu này giúp giữ lời kể trong một sự kiện quá khứ cụ thể.

Sau phần hành vi, cần hỏi kết quả: learner có tiếp tục được không, đã thử bao nhiêu lần và biết mình hiểu bằng cách nào. Với trường hợp chưa giải quyết được, hỏi một lần thật đã xảy ra thay vì đặt giả định. Cuối cùng, dành thời gian cho một trường hợp xử lý nhanh hoặc không cần xử lý để tìm evidence phản bác.

Ưu tiên thực hành là hoàn thành chuỗi **tình huống → hành động → cách xử lý → kết quả** trước khi chuyển sang tần suất. Mục tiêu của lần tiếp theo là có dữ liệu sâu hơn về một sự kiện, từ đó đánh giá liệu rào cản nằm ở kiến thức nền, cách giải thích hay độ tin cậy của câu trả lời.

## 5. AI Support Log

| Công việc | AI đã hỗ trợ | Điểm sai, hời hợt hoặc giới hạn | Cách xử lý trong bản hiện tại |
| --- | --- | --- | --- |
| Chuẩn bị trước interview | Soạn khung Chặng 1, giả thuyết, guide và mẫu báo cáo | Bản đầu bằng tiếng Anh và chia thành 6 file theo cách AI đề xuất | Người thực hiện yêu cầu tiếng Việt và cung cấp cấu trúc nộp; bộ hiện tại được gom thành README, notes và recording |
| Phân tích interview | Sắp xếp evidence, timestamp, quote và kết luận từ bản chép lời được cung cấp | AI không trực tiếp nghe audio; bản chép lời có từ nhận dạng sai | Ghi rõ nguồn; không tự đổi tên công cụ/người chưa rõ; đánh dấu quote cần đối chiếu bản ghi |
| Đánh giá giả thuyết | So sánh dữ liệu với giả thuyết trước interview | Khung ban đầu thiên về khó chẩn đoán kiến thức nền, trong khi dữ liệu chưa chứng minh điều này | Kết luận hỗn hợp/chưa đủ; giữ evidence nghịch về thời gian xử lý ngắn và workaround hiệu quả |
| Chỉnh guide | Đổi câu giả định thành câu hỏi sự kiện thật, bổ sung câu hỏi kết quả và phản chứng | Bản mới chưa được thử lại | Ghi đúng trạng thái phiên bản và dùng cho lần phỏng vấn tiếp theo |
| Reflection | Gợi ý điểm cần xem lại có timestamp | Không thể thay người thực hiện tự nghe lại và tự phản tư | Hoàn thiện nhận xét từ bản chép lời, ghi rõ nguồn và không tuyên bố đã tự nghe lại |

**Các điều chỉnh theo yêu cầu của người thực hiện:** Chuyển bộ nộp sang tiếng Việt; thay cấu trúc 6 file Markdown bằng README và thư mục interview; đưa dữ liệu Day17 vào báo cáo; giữ các ô thông tin định danh để người thực hiện điền. Việc chỉnh sửa câu chữ và phân tích evidence do AI hỗ trợ đã được nêu trong bảng trên.

AI không tạo participant, recording, câu trả lời, transcript hay quote. Nội dung sau interview dựa trên bản chép lời do người thực hiện cung cấp. Quote vẫn cần được người thực hiện đối chiếu với recording để bảo đảm nguyên văn.
