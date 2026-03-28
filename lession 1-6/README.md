# 🎓 Claude 101 — Ghi Chú Học Tập

> **Nguồn:** [Anthropic Academy](https://anthropic.skilljar.com/claude-101) — Khóa học miễn phí dành cho người mới bắt đầu  
> **Tác giả ghi chú:** Tự học & tổng hợp từ tài liệu chính thức của Anthropic  
> **Cập nhật:** Tháng 3/2026

---

## 📋 Mục Lục

| Bài | Chủ đề | Mô tả |
|-----|--------|-------|
| [Bài 1](#-bài-1--what-is-claude) | What is Claude? | Claude là gì, ai tạo ra, hoạt động như thế nào |
| [Bài 2](#-bài-2--your-first-conversation--getting-better-results) | First Conversation + Getting Better Results | 6 kỹ thuật prompt cốt lõi |
| [Bài 3](#-bài-3--claude-desktop-app-chat-cowork-code) | Claude Desktop App | 3 chế độ: Chat, Cowork, Code |
| [Bài 4](#-bài-4--introduction-to-projects) | Introduction to Projects | Workspace có tổ chức, knowledge base |
| [Bài 5](#-bài-5--creating-with-artifacts) | Creating with Artifacts | Tạo sản phẩm có thể chia sẻ |
| [Bài 6](#-bài-6--working-with-skills) | Working with Skills | Dạy Claude làm việc theo phong cách của bạn |

---

## 🟢 Bài 1 — What is Claude?

### Claude là gì?

Claude là một **AI assistant thế hệ mới** được tạo ra bởi **Anthropic** — công ty nghiên cứu AI tập trung vào an toàn, được thành lập bởi các cựu nhân viên OpenAI. Claude được thiết kế để hữu ích, trung thực và vô hại trong mọi tương tác.

> 💡 Tên "Claude" được lấy cảm hứng từ **Claude Shannon** — nhà toán học thế kỷ 20 đặt nền tảng cho lý thuyết thông tin.

---

### Triết lý cốt lõi — "Constitutional AI"

Claude được huấn luyện bằng kỹ thuật **Constitutional AI (CAI)** với bộ nguyên tắc tích hợp sẵn. Ba nguyên tắc cốt lõi — thường gọi là **"3H"**:

| Nguyên tắc | Ý nghĩa |
|------------|---------|
| 🟢 **Helpful** (Hữu ích) | Giúp bạn hoàn thành công việc thực sự |
| 🔵 **Harmless** (Vô hại) | Tránh tạo ra nội dung gây hại |
| 🟡 **Honest** (Trung thực) | Thừa nhận khi không biết, không bịa đặt |

---

### Cách Claude hoạt động

Claude là **Generative Pre-trained Transformer (GPT)** — sử dụng cơ chế attention để hiểu ngữ cảnh và mối quan hệ giữa các từ. Được huấn luyện trên:
- Lượng lớn dữ liệu internet công khai
- Nội dung bên thứ ba được cấp phép
- Dữ liệu từ người dùng và crowd workers

---

### Các phiên bản Claude hiện tại (2026)

| Model | Đặc điểm | Dùng tốt cho |
|-------|----------|-------------|
| **Haiku 4.5** | Nhanh, nhẹ, rẻ nhất | Tác vụ đơn giản, cần tốc độ |
| **Sonnet 4.6** | Cân bằng tốt nhất | Hầu hết công việc hàng ngày |
| **Opus 4.6** | Mạnh nhất, sâu nhất | Phân tích phức tạp, lý luận cao |

---

### Claude có thể làm gì?

| Lĩnh vực | Khả năng |
|----------|---------|
| ✍️ **Viết lách** | Email, báo cáo, bài viết, nội dung marketing |
| 🔍 **Nghiên cứu** | Tóm tắt tài liệu, so sánh, phân tích dữ liệu |
| 💻 **Lập trình** | Viết code, debug, giải thích, review |
| 🧠 **Tư duy** | Brainstorm, lên kế hoạch, giải quyết vấn đề |
| 📄 **Tài liệu** | Đọc và tóm tắt PDF, hợp đồng, báo cáo dài |
| 🌐 **Dịch thuật** | Đa ngôn ngữ với ngữ cảnh chính xác |

---

### Cách truy cập Claude

```
🌐 Web/Mobile  →  claude.ai
🖥️ Desktop App →  claude.com/download  (Mac / Windows)
📱 Mobile App  →  iOS & Android
🔧 API         →  Dành cho developer xây dựng ứng dụng
```

---

## 🟡 Bài 2 — Your First Conversation + Getting Better Results

### Prompt Engineering là gì?

**Prompt Engineering** là nghệ thuật cấu trúc các chỉ dẫn để nhận được kết quả tốt hơn từ AI. Sự khác biệt giữa một chỉ dẫn mơ hồ và một prompt được thiết kế tốt có thể là khoảng cách giữa kết quả chung chung và **chính xác những gì bạn cần**.

---

### 6 Kỹ Thuật Cốt Lõi (Theo tài liệu chính thức Anthropic)

---

#### 🟢 Kỹ thuật 1 — Be Explicit & Clear (Nói rõ ràng)

Đừng giả định Claude tự suy ra ý bạn — **nói thẳng vào vấn đề**.

| ❌ Vague | ✅ Explicit |
|---------|-----------|
| *"Viết email cho tôi"* | *"Viết email chuyên nghiệp xin lỗi khách hàng vì trễ deadline 2 ngày, đề xuất giải pháp bù đắp, giọng điệu lịch sự, dưới 150 từ"* |
| *"Tạo dashboard"* | *"Tạo analytics dashboard. Bao gồm nhiều tính năng và tương tác liên quan nhất có thể. Vượt qua những điều cơ bản để tạo sản phẩm đầy đủ tính năng."* |

**Quy tắc vàng:**
- Bắt đầu bằng **động từ hành động**: *"Viết", "Phân tích", "Tạo", "Giải thích"*
- Bỏ phần dẫn nhập dài dòng — đi thẳng vào yêu cầu
- Nêu rõ kết quả muốn trông như thế nào

---

#### 🟡 Kỹ thuật 2 — Provide Context (Cung cấp ngữ cảnh)

Giải thích **tại sao** điều gì đó quan trọng giúp Claude hiểu mục tiêu sâu hơn.

| ❌ Thiếu lý do | ✅ Có ngữ cảnh & lý do |
|--------------|----------------------|
| *"ĐỪNG dùng bullet points"* | *"Tôi muốn văn xuôi tự nhiên thay vì bullet points vì tôi thấy dễ đọc và mang tính trò chuyện hơn. Bullet points cảm thấy quá trang trọng với phong cách học tập thông thường của tôi."* |

**Khi nào cần cung cấp ngữ cảnh:**
- Giải thích mục đích hoặc đối tượng của nội dung
- Làm rõ tại sao có những ràng buộc nhất định
- Mô tả nội dung sẽ được sử dụng như thế nào

---

#### 🟠 Kỹ thuật 3 — Be Specific (Cụ thể hóa)

Bạn càng cụ thể về những gì muốn, kết quả càng tốt hơn.

| ❌ Mơ hồ | ✅ Cụ thể |
|---------|---------|
| *"Tạo thực đơn ăn kiêng"* | *"Thiết kế thực đơn ăn kiêng Địa Trung Hải cho tiền tiểu đường. 1.800 calo/ngày, thực phẩm chỉ số glycemic thấp. Liệt kê bữa sáng, trưa, tối và một bữa phụ kèm thông tin dinh dưỡng đầy đủ."* |

**Checklist prompt đủ cụ thể:**
- ✅ Ràng buộc rõ ràng (số từ, định dạng, thời hạn)
- ✅ Ngữ cảnh liên quan (đối tượng là ai, mục tiêu là gì)
- ✅ Cấu trúc kết quả mong muốn (bảng, danh sách, đoạn văn)
- ✅ Yêu cầu hoặc hạn chế cụ thể

---

#### 🔵 Kỹ thuật 4 — Use Examples (Dùng ví dụ)

**"Chỉ ra thay vì chỉ mô tả"** — ví dụ làm rõ các yêu cầu tinh tế mà mô tả thuần túy không diễn đạt được.

```
Đây là ví dụ về kiểu tóm tắt tôi muốn:

Bài báo: [link về quy định AI của EU]
Tóm tắt: EU thông qua Đạo luật AI toàn diện nhắm vào hệ thống rủi ro cao.
Điều khoản chính: yêu cầu minh bạch và giám sát của con người. Hiệu lực từ 2026.

Bây giờ hãy tóm tắt bài báo này theo cùng phong cách: [link bài báo mới]
```

> 💡 **Lời khuyên:** Bắt đầu với 1 ví dụ (one-shot). Chỉ thêm nhiều hơn nếu kết quả chưa đúng.

---

#### 🔴 Kỹ thuật 5 — Permit Uncertainty (Cho phép không chắc chắn)

Cho Claude phép rõ ràng để thừa nhận khi không biết — giúp **giảm hallucination** và tăng độ tin cậy.

```
"Phân tích dữ liệu tài chính này và xác định xu hướng.
Nếu dữ liệu không đủ để đưa ra kết luận, hãy nói rõ
thay vì suy đoán."
```

---

#### 🟣 Kỹ thuật 6 — Chain of Thought (Suy luận từng bước)

Yêu cầu AI lý luận theo từng bước trước khi trả lời — đặc biệt hiệu quả với tác vụ phức tạp.

**3 cách áp dụng:**

```markdown
# Cách 1 — Đơn giản
"[Yêu cầu của bạn]. Hãy suy nghĩ từng bước."

# Cách 2 — Có hướng dẫn
"Hãy suy nghĩ trước khi trả lời. Đầu tiên, phân tích X.
Sau đó, xem xét Y. Cuối cùng, đưa ra kết luận."

# Cách 3 — Có cấu trúc tag
"Hãy suy nghĩ trong thẻ <thinking>. Phân tích tình huống.
Sau đó viết kết quả trong thẻ <answer>."
```

---

### Bảng Chọn Kỹ Thuật Phù Hợp

| Nếu bạn cần... | Dùng kỹ thuật... |
|----------------|-----------------|
| Định dạng kết quả cụ thể | Ví dụ (examples) hoặc chỉ dẫn định dạng |
| Lý luận từng bước | Extended Thinking hoặc Chain of Thought |
| Tác vụ phức tạp nhiều giai đoạn | Prompt Chaining (chia nhỏ thành nhiều prompt) |
| Tránh bịa đặt thông tin | Cho phép nói "Tôi không biết" |

---

### ❌ Lỗi Phổ Biến Cần Tránh

| ❌ Lỗi | ✅ Cách sửa |
|--------|-----------|
| Over-engineer prompt quá dài | Prompt ngắn gọn thường tốt hơn |
| Bỏ qua kỹ thuật cơ bản | Nâng cao không giúp ích nếu nền tảng yếu |
| Kỳ vọng AI đọc được suy nghĩ | Nói rõ ràng những gì bạn muốn |
| Dùng tất cả kỹ thuật cùng lúc | Chọn đúng kỹ thuật cho đúng vấn đề |
| Không lặp lại và tinh chỉnh | Prompt đầu tiên hiếm khi hoàn hảo |
| AI gợi ý thay vì thực hiện | Thêm: *"Hãy thực hiện thay đổi"* |

---

## 🔵 Bài 3 — Claude Desktop App: Chat, Cowork, Code

### Tổng quan

Claude Desktop App (tải tại **claude.com/download**) tích hợp **3 chế độ** trong một giao diện:

```
┌─────────────────────────────────────────┐
│          CLAUDE DESKTOP APP             │
│  ┌─────────┬───────────┬─────────────┐  │
│  │  CHAT   │  COWORK   │    CODE     │  │
│  │ Hội thoại│Thực thi   │ Lập trình  │  │
│  └─────────┴───────────┴─────────────┘  │
└─────────────────────────────────────────┘
```

---

### 🟢 Chế độ CHAT

**Dùng cho:** Hỏi đáp, viết lách, brainstorm, học tập, phân tích

Claude phản hồi tin nhắn của bạn nhưng **không truy cập trực tiếp file** trên máy tính — chỉ làm việc với nội dung bạn paste vào chat.

---

### 🟡 Chế độ COWORK ⭐

**Tính năng đột phá nhất** — biến Claude từ "người tư vấn" thành **"người thực thi"**.

#### Sự khác biệt Chat vs Cowork

| Tiêu chí | Chat | Cowork |
|----------|------|--------|
| **Bản chất** | Hội thoại | Phiên làm việc |
| **Khả năng** | Trả lời, gợi ý | **Thực thi, tạo ra sản phẩm** |
| **File** | Không truy cập trực tiếp | Đọc, sửa, tạo file thực |
| **Kết quả** | Lời khuyên, hướng dẫn | **Deliverable hoàn chỉnh** |

#### Cowork có thể làm gì?

```
📂 Tổ chức file      → Sắp xếp, đổi tên, dọn dẹp thư mục tự động
📊 Bảng tính          → Chuyển ảnh chụp màn hình/biên lai thành Excel
📝 Báo cáo            → Tổng hợp từ nhiều file thành báo cáo có định dạng
⏰ Tác vụ định kỳ    → Tự động chạy hàng ngày/tuần theo lịch
📱 Từ điện thoại      → Nhắn lệnh từ phone, desktop thực hiện, bạn lấy kết quả
```

#### Tính năng Scheduled Tasks

Đặt lịch một lần — Claude xử lý mãi:
- ✅ Kiểm tra email mỗi buổi sáng
- ✅ Kéo metrics từ dashboard
- ✅ Chạy digest Slack hàng tuần

#### Bạn luôn kiểm soát

> ⚠️ Trước khi thực hiện hành động quan trọng, Claude luôn **hiển thị kế hoạch và chờ bạn phê duyệt**. Bạn có thể redirect, tinh chỉnh hoặc dừng lại bất kỳ lúc nào.

---

### 🔵 Chế độ CODE

Dành cho **developer** — tích hợp với terminal, GitHub, và codebase:

| Khả năng | Chi tiết |
|----------|---------|
| Viết & debug code | Mọi ngôn ngữ lập trình |
| Context management | Hiểu toàn bộ codebase |
| Custom commands | Tạo slash commands tái sử dụng |
| GitHub integration | Automated code review |
| MCP servers | Kết nối browser automation, databases |

---

### 💰 Các Gói Giá

| Gói | Giá | Cowork |
|-----|-----|--------|
| **Free** | Miễn phí | ❌ |
| **Pro** | $17/tháng | ✅ Tác vụ thông thường |
| **Max 5x** | $100/tháng | ✅ Dùng hàng ngày |
| **Max 20x** | $200/tháng | ✅ Power user |

---

### 📂 Định dạng File Cowork Hỗ Trợ

```
📄 Documents: .docx, .pdf, .txt, .md, .html
📊 Spreadsheets: .xlsx, .xls, .xlsm
📑 Presentations: .pptx, .ppt
🖼️ Images: .png, .jpg, .jpeg, .gif, .svg, .webp
📋 Data: .csv, .json, .yaml, .xml
💻 Code: .py, .js, .ts, .jsx, .tsx, .java, .go, .rs, .rb, .php, .sql...
```

---

## 🟠 Bài 4 — Introduction to Projects

### Projects là gì?

**Projects** là các **không gian làm việc độc lập (self-contained workspaces)** với lịch sử chat và knowledge base riêng. Giống như những "văn phòng riêng biệt" — mỗi văn phòng có tủ hồ sơ, quy trình và mục tiêu riêng.

---

### Chat Thông Thường vs Projects

| Tiêu chí | Chat thường | Projects |
|----------|------------|---------|
| **Bộ nhớ** | Bắt đầu lại từ đầu | Nhớ xuyên suốt project |
| **Tài liệu** | Upload lại mỗi lần | Upload một lần, dùng mãi |
| **Hướng dẫn** | Phải nhắc lại mỗi lần | Cài đặt một lần, áp dụng tất cả |
| **Tổ chức** | Chat rải rác | Nhóm theo chủ đề |
| **Cộng tác** | Chỉ mình bạn | Chia sẻ với team (gói trả phí) |

---

### Knowledge Base — Bộ Não Của Project

Upload tài liệu vào project — Claude sẽ sử dụng chúng làm ngữ cảnh cho **tất cả** các cuộc chat trong project đó:

| Loại Project | Nên upload |
|-------------|-----------|
| 📝 Marketing | Style guide, brand guidelines, tone of voice |
| 💻 Development | Codebase, docs kỹ thuật, coding standards |
| 📚 Nghiên cứu | Papers, bài báo, dữ liệu thống kê |
| 🏢 Sales | Pitch deck, case studies, danh sách khách hàng |
| 🎓 Học tập | Giáo trình, bài giảng, ghi chú |

---

### RAG — Siêu Năng Lực Của Gói Trả Phí

Khi knowledge base tiếp cận giới hạn, Claude tự động bật **Retrieval Augmented Generation (RAG)** để mở rộng dung lượng **lên đến 10 lần** trong khi vẫn duy trì chất lượng phản hồi.

| Gói | Số Projects | RAG |
|-----|-------------|-----|
| **Free** | Tối đa 5 | ❌ |
| **Pro/Max** | Không giới hạn | ✅ ×10 |
| **Team/Enterprise** | Không giới hạn | ✅ ×10 + chia sẻ |

---

### Hướng Dẫn Tạo Project — Từng Bước

```
1. Vào claude.ai/projects
2. Nhấn "+ New Project" (góc trên bên phải)
3. Đặt tên và mô tả project
4. Nhấn "+" để upload tài liệu vào Knowledge Base
5. Nhấn "Set project instructions" → viết hướng dẫn → Save
6. Bắt đầu chat trong project!
```

---

### Ví dụ Project Instructions Hiệu Quả

```
- Luôn trả lời bằng tiếng Việt
- Giọng điệu chuyên nghiệp nhưng thân thiện
- Khi viết email: Kính gửi / Trân trọng
- Khi phân tích dữ liệu, luôn đưa ra 3 insight quan trọng nhất
- Nếu không chắc chắn, hãy nói rõ thay vì đoán
```

---

### Quản Lý Projects

| Tính năng | Cách dùng |
|-----------|----------|
| ⭐ **Đánh dấu sao** | Truy cập nhanh từ sidebar |
| 📦 **Di chuyển chat** | Click dropdown → "Add to project" |
| 🗄️ **Archive** | Lưu project đã hoàn thành (giữ quyền xem) |
| 🗑️ **Xóa** | Click "..." → Delete (phải unarchive trước) |

---

### Chia Sẻ Projects (Team & Enterprise)

| Quyền | Được làm gì |
|-------|------------|
| **Can use** | Xem nội dung, knowledge, chat trong project |
| **Can edit** | Chỉnh sửa hướng dẫn, knowledge, quản lý thành viên |

**Các tùy chọn chia sẻ:**
- Individual sharing — chia sẻ với người cụ thể qua email
- Bulk sharing — thêm nhiều người qua danh sách email
- Organization-wide — chia sẻ với toàn tổ chức

---

## 🔴 Bài 5 — Creating with Artifacts

### Artifacts là gì?

**Artifacts** là nội dung độc lập được Claude tạo ra trong một **cửa sổ riêng biệt** — không chỉ là văn bản trong chat, mà là thứ bạn có thể chỉnh sửa, chia sẻ, tải về và dùng lại.

---

### Khi nào Claude tạo Artifacts?

Claude tạo artifact khi nội dung:
- Có quy mô đáng kể và độc lập (**thường >15 dòng**)
- Là thứ bạn có thể muốn **chỉnh sửa, lặp lại, hoặc tái sử dụng**
- Đại diện cho nội dung phức tạp có thể **đứng một mình**
- Là nội dung bạn muốn **tham chiếu lại hoặc dùng sau này**

---

### Các Loại Artifacts

| Loại | Ví dụ thực tế |
|------|--------------|
| 📄 **Documents** | Báo cáo, bài viết blog, email template, hợp đồng |
| 💻 **Code snippets** | Script Python, hàm JavaScript, SQL query |
| 🌐 **HTML pages** | Landing page, portfolio, form liên hệ |
| 🖼️ **SVG images** | Logo, icon, biểu đồ vector |
| 📊 **Diagrams** | Flowchart, mindmap, ERD, sequence diagram |
| ⚛️ **React components** | Dashboard, calculator, game, quiz tương tác |

---

### Làm Việc Với Artifacts

#### Edit & Iterate (Chỉnh sửa và lặp lại)

```
"Làm cho các nút to hơn"
"Đổi màu sang xanh lá"
"Thêm tính năng timer"
"Rút gọn xuống còn 200 từ"
"Dịch sang tiếng Anh"
```

Mỗi yêu cầu **build on previous versions** — Claude giữ ngữ cảnh về những gì đã xây dựng.

#### View & Export

Góc dưới bên phải cửa sổ artifact:
- 👁️ Xem **code gốc** của artifact
- 📋 **Sao chép** nội dung vào clipboard
- ⬇️ **Tải file xuống** để dùng ngoài cuộc trò chuyện

#### Forking — Thử nghiệm không lo mất bản gốc

> Quay lại bất kỳ tin nhắn trước đó → Click **"Edit"** → Tạo nhánh hội thoại mới → Thử hướng đi khác → Luôn có thể quay lại bản gốc.

#### Fix Errors Tự Động

Khi artifact có lỗi → Click **"Try fixing with Claude"** → Claude tự chẩn đoán và đề xuất cách sửa.

---

### AI-Powered Artifacts ⭐

Bạn có thể xây dựng artifacts **nhúng khả năng AI**, biến chúng thành ứng dụng thực sự:

```
Bước 1: Mô tả những gì bạn muốn với Claude
Bước 2: Claude viết code
Bước 3: Ứng dụng chạy trên cơ sở hạ tầng Anthropic
Bước 4: Người dùng xác thực bằng tài khoản Claude và tương tác
```

> 💰 **Chi phí chia sẻ: MIỄN PHÍ** — Dù artifact của bạn giúp 10 người hay 10.000 người, mức sử dụng tính vào giới hạn subscription của từng người dùng, không phải của bạn.

---

### MCP Integration

Artifacts có thể kết nối với dịch vụ bên ngoài qua **Model Context Protocol (MCP)**:
- 📋 Asana — quản lý task
- 📅 Google Calendar — lịch hẹn
- 💬 Slack — tin nhắn
- + Bất kỳ custom MCP server nào bạn đã cấu hình

---

### Persistent Storage

| Loại | Đặc điểm | Ví dụ |
|------|----------|-------|
| **Personal** | Mỗi người có dữ liệu riêng tư | Nhật ký cá nhân |
| **Shared** | Tất cả người dùng thấy cùng dữ liệu | Bảng xếp hạng game |

**Thông số:** Giới hạn 20 MB/artifact · Text/JSON only · Chỉ khả dụng sau khi publish

---

### Chia Sẻ & Xuất Bản Artifacts

```
Publish → Nhấn nút "Publish" → Nhận link chia sẻ
Embed   → Nhấn "Get embed code" → Copy vào website của bạn
Unpublish → Xóa quyền truy cập (lưu ý: không publish lại được!)
```

---

### Ý Tưởng Artifacts Theo Lĩnh Vực

| Lĩnh vực | Artifact gợi ý |
|----------|---------------|
| 🎓 Giáo dục | Quiz tương tác, flashcard, sơ đồ chu trình |
| 💼 Kinh doanh | Dashboard KPI, báo cáo tự động |
| 🛒 Marketing | Landing page, email template |
| 💻 Dev | API explorer, code playground |
| 🎮 Cá nhân | Game đơn giản, habit tracker, meal planner |
| 📊 Phân tích | Data visualizer, calculator, biểu đồ |

---

### Bật/Tắt Artifacts

```
Settings → Capabilities → Artifacts → Toggle On/Off
```

---

## 🟣 Bài 6 — Working with Skills

### Skills là gì?

**Skills** là các thư mục chứa hướng dẫn, script và tài nguyên mà Claude **tải động** để cải thiện hiệu suất trên các tác vụ chuyên biệt. Skills dạy Claude cách hoàn thành các tác vụ cụ thể theo cách **lặp lại có thể tái tạo** — một lần viết xong, Claude làm đúng theo cách đó mỗi khi cần.

---

### Cách Skills Hoạt Động — Progressive Disclosure

```
Bạn gửi yêu cầu
        ↓
Claude scan tất cả Skills có sẵn
        ↓
Xác định Skills nào liên quan
        ↓
Tải và áp dụng hướng dẫn từ Skills đó
        ↓
Thực hiện tác vụ đúng theo quy trình của bạn
```

> ✅ Skills chỉ tải **khi cần** — giúp tránh quá tải context window.

---

### 4 Loại Skills

| Loại | Mô tả | Ví dụ |
|------|-------|-------|
| 🔵 **Anthropic Skills** | Do Anthropic tạo, tự động kích hoạt | Excel, Word, PowerPoint, PDF |
| 🟢 **Custom Skills** | Do bạn tạo cho workflow riêng | Brand guidelines, email template |
| 🟡 **Organization Skills** | Admin phân phối cho toàn team | Quy trình chuẩn công ty |
| 🟠 **Partner Skills** | Từ Notion, Figma, Atlassian... | Notion workflow, Figma export |

---

### Skills vs Các Tính Năng Khác

| | Skills | Projects | Custom Instructions | MCP |
|---|--------|----------|--------------------|----|
| **Phạm vi** | Kích hoạt **khi cần** | **Luôn tải** trong project | **Mọi cuộc chat** | Kết nối **dịch vụ ngoài** |
| **Mục đích** | Quy trình & thủ tục | Kiến thức nền tảng | Sở thích cá nhân | Truy cập công cụ |
| **Hoạt động** | Động (dynamic) | Tĩnh (static) | Luôn bật | Theo yêu cầu |

---

### Cách Bật và Dùng Skills

```
Bước 1: Settings → Capabilities → Bật "Code execution and file creation"
Bước 2: Customize → Skills (claude.ai/customize/skills)
Bước 3: Toggle bật/tắt Skills muốn dùng
```

> 💡 **Trong Excel & PowerPoint:** Gõ `/` để xem Skills có sẵn, hoặc mô tả tác vụ tự nhiên — Claude tự nhận biết khi Skills phù hợp.

---

### Cách Tạo Custom Skill — Từng Bước

#### Bước 1: Tạo file `Skill.md`

```markdown
## Metadata
name: Tên Skill (tối đa 64 ký tự)
description: Mô tả rõ ràng khi nào dùng Skill này (tối đa 200 ký tự)

## [Nội dung hướng dẫn chi tiết]
```

#### Bước 2: Đóng gói đúng cách

```
✅ Cấu trúc đúng:
my-skill.zip
└── my-skill/
    ├── Skill.md
    └── resources/ (nếu có)

❌ Cấu trúc sai:
my-skill.zip
└── Skill.md  (file trực tiếp trong ZIP root)
```

#### Bước 3: Upload

```
Customize → Skills → Nhấn "+" → "Upload a skill" → Upload ZIP
```

---

### 5 Ví Dụ Custom Skill Thực Tế

#### 📧 Email Template Công Ty

```markdown
## Metadata
name: Company Email Template
description: Generate professional emails following company tone and 
format for client communications

## Email Structure
- Subject: [Action/FYI/Update] - Topic - [Date]
- Opening: Kính gửi [Tên], / Dear [Name],
- Body: Tối đa 3 đoạn, bullet points cho action items
- Closing: Trân trọng, / Best regards,

## Tone: Chuyên nghiệp, thân thiện, active voice
```

#### 📋 Meeting Notes

```markdown
## Metadata
name: Meeting Notes Format
description: Structure meeting notes with decisions, action items, 
owners and deadlines in company format

## Template
**Ngày:** [DD/MM/YYYY] | **Người tham dự:** [Tên]
**Mục tiêu:** [...]

**Quyết định chính:**
- [Quyết định]

**Action Items:**
| Công việc | Người phụ trách | Deadline |

**Cuộc họp tiếp theo:** [Ngày]
```

#### 📊 Data Analysis Report

```markdown
## Metadata
name: Data Analysis Report
description: Analyze data producing reports with executive summary,
key findings, chart recommendations and next steps

## Report Structure
1. Executive Summary (3-5 bullet points)
2. Key Findings (kèm dữ liệu cụ thể)
3. Visualizations (gợi ý loại biểu đồ)
4. Recommendations (ưu tiên theo mức độ tác động)
5. Next Steps
```

#### 💻 Code Review Checklist

```markdown
## Metadata
name: Code Review
description: Review code for quality, security, performance following 
engineering standards with structured checklist

## Checklist
- [ ] Naming conventions đúng chuẩn
- [ ] Error handling được implement
- [ ] Không có hardcoded credentials
- [ ] Tests đã viết
- [ ] Documentation cập nhật
- [ ] Performance impact được đánh giá
```

#### 📱 Social Media Content

```markdown
## Metadata
name: Social Media Content
description: Create social posts matching brand voice for LinkedIn, 
Facebook and Twitter with appropriate format per platform

## Brand Voice: Professional, educational, insightful

## Per Platform
- LinkedIn: 150-300 từ, chuyên nghiệp, tối đa 5 hashtags
- Facebook: 50-100 từ, thân thiện, conversational
- Twitter: ≤280 ký tự, ngắn gọn, có call-to-action
```

---

### Best Practices Khi Tạo Skills

| ✅ Nên làm | ❌ Không nên làm |
|-----------|----------------|
| Tạo Skills tập trung một mục đích | Một Skill cố làm mọi thứ |
| Viết description rõ ràng, cụ thể | Description mơ hồ |
| Bắt đầu đơn giản, mở rộng dần | Build phức tạp ngay từ đầu |
| Include ví dụ input/output | Chỉ có hướng dẫn, không có ví dụ |
| Test sau mỗi thay đổi | Build xong mới test |

---

### Bảo Mật Khi Dùng Skills

> ⚠️ **Quan trọng:** Chỉ cài Skills từ **nguồn tin cậy**.

```
✅ Đọc kỹ nội dung file trước khi bật
✅ Kiểm tra code dependencies
❌ Không hardcode API keys hay mật khẩu trong Skill
❌ Cẩn thận với Skills yêu cầu kết nối mạng ngoài
```

---

### Khám Phá Skills Directory

Truy cập **claude.com/connectors** để tìm partner skills từ:
- 📝 Notion
- 🎨 Figma  
- 🔧 Atlassian (Jira, Confluence)
- + Nhiều nền tảng khác

---

## 🗺️ Lộ Trình Học Toàn Bộ Khóa Học

```
✅ Bài 1: What is Claude?
✅ Bài 2: Your First Conversation + Getting Better Results
✅ Bài 3: Claude Desktop App: Chat, Cowork, Code
✅ Bài 4: Introduction to Projects
✅ Bài 5: Creating with Artifacts
✅ Bài 6: Working with Skills

⏳ Bài 7: Connecting your Tools (MCP, Connectors)
⏳ Bài 8: Enterprise Search
⏳ Bài 9: Research Mode for Deep Dives
⏳ Bài 10: Claude in Action — Use Cases by Role
⏳ Bài 11: Other Ways to Work with Claude
⏳ Certificate of Completion
```

---

## 🔗 Tài Nguyên Hữu Ích

| Tài nguyên | Link |
|-----------|------|
| 🎓 Anthropic Academy | [anthropic.skilljar.com](https://anthropic.skilljar.com) |
| 📖 Documentation | [docs.anthropic.com](https://docs.anthropic.com) |
| ❓ Support Center | [support.claude.com](https://support.claude.com) |
| 🔧 Claude Platform | [platform.claude.com](https://platform.claude.com) |
| 💡 Prompt Engineering Guide | [claude.com/blog/best-practices-for-prompt-engineering](https://claude.com/blog/best-practices-for-prompt-engineering) |
| 🛠️ Skills Directory | [claude.com/connectors](https://claude.com/connectors) |
| 🎯 Example Skills (GitHub) | [github.com/anthropics/skills](https://github.com/anthropics/skills) |
| 📐 Agent Skills Standard | [agentskills.io](https://agentskills.io) |

---

## 📊 Tổng Hợp Nhanh — Khi Nào Dùng Tính Năng Gì?

| Tình huống | Dùng tính năng |
|-----------|---------------|
| Hỏi đáp, brainstorm nhanh | **Chat** |
| Muốn Claude thực sự *làm việc* với file của bạn | **Cowork** |
| Lập trình, debug, GitHub | **Code** |
| Tổ chức công việc theo chủ đề, upload tài liệu 1 lần | **Projects** |
| Tạo nội dung có thể chỉnh sửa, chia sẻ, tải về | **Artifacts** |
| Dạy Claude quy trình/phong cách làm việc của bạn | **Skills** |
| Cài đặt giọng điệu/sở thích cho mọi cuộc chat | **Custom Instructions** |
| Kết nối Claude với Google Drive, Slack, Jira... | **MCP Connectors** |

---

> 📝 **Ghi chú:** Tài liệu này được tổng hợp từ khóa học Claude 101 trên [Anthropic Academy](https://anthropic.skilljar.com/claude-101).  
> Nội dung dựa trên tài liệu chính thức của Anthropic — cập nhật tháng 3/2026.

---

*Happy learning! 🚀*
