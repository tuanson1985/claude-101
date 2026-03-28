# 🎓 Claude 101 — Ghi Chú Học Tập Đầy Đủ

> **Nguồn:** [Anthropic Academy](https://anthropic.skilljar.com/claude-101) — Khóa học miễn phí dành cho người mới bắt đầu
> **Cập nhật:** Tháng 3/2026 | **Tác giả:** Tự học & tổng hợp từ tài liệu chính thức của Anthropic

---

## 📋 Mục Lục

| # | Bài học | Chủ đề |
|---|---------|--------|
| [Bài 1](#-bài-1--what-is-claude) | What is Claude? | Claude là gì, ai tạo ra, hoạt động như thế nào |
| [Bài 2](#-bài-2--your-first-conversation--getting-better-results) | First Conversation + Getting Better Results | 6 kỹ thuật prompt cốt lõi |
| [Bài 3](#-bài-3--claude-desktop-app-chat-cowork-code) | Claude Desktop App | 3 chế độ: Chat, Cowork, Code |
| [Bài 4](#-bài-4--introduction-to-projects) | Introduction to Projects | Workspace có tổ chức, knowledge base |
| [Bài 5](#-bài-5--creating-with-artifacts) | Creating with Artifacts | Tạo sản phẩm có thể chia sẻ |
| [Bài 6](#-bài-6--working-with-skills) | Working with Skills | Dạy Claude làm việc theo phong cách của bạn |
| [Bài 7](#-bài-7--connecting-your-tools) | Connecting Your Tools | MCP Connectors, kết nối công cụ |
| [Bài 8](#-bài-8--enterprise-search) | Enterprise Search | Tìm kiếm thống nhất toàn tổ chức |
| [Bài 9](#-bài-9--research-mode-for-deep-dives) | Research Mode | Nghiên cứu chuyên sâu đa nguồn |
| [Bài 10](#-bài-10--claude-in-action-use-cases-by-role) | Use Cases by Role | Ứng dụng theo từng vai trò |
| [Bài 11](#-bài-11--other-ways-to-work-with-claude) | Other Ways to Work | Toàn bộ hệ sinh thái Claude |
| [Bài 12](#-bài-12--conclusion--certificate) | Conclusion & Certificate | Tổng kết & lộ trình tiếp theo |

---

## 🟢 Bài 1 — What is Claude?

### Claude là gì?

Claude là **AI assistant thế hệ mới** được tạo ra bởi **Anthropic** — công ty nghiên cứu AI tập trung vào an toàn, được thành lập bởi các cựu nhân viên OpenAI. Tên "Claude" được lấy cảm hứng từ **Claude Shannon** — nhà toán học đặt nền tảng cho lý thuyết thông tin.

### Triết lý cốt lõi — "Constitutional AI" & 3H

Claude được huấn luyện bằng kỹ thuật **Constitutional AI (CAI)** với 3 nguyên tắc nền tảng:

| Nguyên tắc | Ý nghĩa |
|------------|---------|
| 🟢 **Helpful** | Giúp bạn hoàn thành công việc thực sự |
| 🔵 **Harmless** | Tránh tạo ra nội dung gây hại |
| 🟡 **Honest** | Thừa nhận khi không biết, không bịa đặt |

### Các phiên bản Claude (2026)

| Model | Đặc điểm | Dùng tốt cho |
|-------|----------|-------------|
| **Haiku 4.5** | Nhanh, nhẹ, rẻ nhất | Tác vụ đơn giản, cần tốc độ |
| **Sonnet 4.6** | Cân bằng tốt nhất | Hầu hết công việc hàng ngày |
| **Opus 4.6** | Mạnh nhất, sâu nhất | Phân tích phức tạp, lý luận cao |

### Claude có thể làm gì?

| Lĩnh vực | Khả năng |
|----------|---------|
| ✍️ Viết lách | Email, báo cáo, bài viết, nội dung marketing |
| 🔍 Nghiên cứu | Tóm tắt tài liệu, so sánh, phân tích dữ liệu |
| 💻 Lập trình | Viết code, debug, giải thích, review |
| 🧠 Tư duy | Brainstorm, lên kế hoạch, giải quyết vấn đề |
| 📄 Tài liệu | Đọc và tóm tắt PDF, hợp đồng, báo cáo dài |
| 🌐 Dịch thuật | Đa ngôn ngữ với ngữ cảnh chính xác |

### Cách truy cập Claude

```
🌐 Web/Mobile  → claude.ai
🖥️ Desktop App → claude.com/download  (Mac / Windows)
📱 Mobile App  → iOS & Android
🔧 API         → Dành cho developer xây dựng ứng dụng
```

---

## 🟡 Bài 2 — Your First Conversation + Getting Better Results

### Prompt Engineering là gì?

**Prompt Engineering** là nghệ thuật cấu trúc chỉ dẫn để nhận kết quả tốt hơn từ AI. Sự khác biệt giữa một chỉ dẫn mơ hồ và prompt được thiết kế tốt có thể là khoảng cách giữa kết quả chung chung và chính xác những gì bạn cần.

### 6 Kỹ Thuật Cốt Lõi

#### 🟢 Kỹ thuật 1 — Be Explicit & Clear

| ❌ Vague | ✅ Explicit |
|---------|-----------|
| *"Viết email cho tôi"* | *"Viết email chuyên nghiệp xin lỗi khách hàng vì trễ deadline 2 ngày, đề xuất giải pháp bù đắp, giọng điệu lịch sự, dưới 150 từ"* |
| *"Tạo dashboard"* | *"Tạo analytics dashboard. Bao gồm nhiều tính năng và tương tác liên quan nhất có thể. Vượt qua những điều cơ bản để tạo sản phẩm đầy đủ tính năng."* |

**Quy tắc vàng:** Bắt đầu bằng động từ hành động: *"Viết", "Phân tích", "Tạo", "Giải thích"*

#### 🟡 Kỹ thuật 2 — Provide Context

Giải thích **tại sao** — giúp Claude hiểu mục tiêu sâu hơn và đưa ra phản hồi chính xác hơn.

```
❌ "ĐỪNG dùng bullet points"
✅ "Tôi muốn văn xuôi tự nhiên thay vì bullet points vì tôi thấy
    dễ đọc và mang tính trò chuyện hơn với phong cách học của tôi."
```

#### 🟠 Kỹ thuật 3 — Be Specific

Checklist prompt đủ cụ thể:
- ✅ Ràng buộc rõ ràng (số từ, định dạng, thời hạn)
- ✅ Ngữ cảnh liên quan (đối tượng là ai, mục tiêu là gì)
- ✅ Cấu trúc kết quả mong muốn (bảng, danh sách, đoạn văn)

#### 🔵 Kỹ thuật 4 — Use Examples

**"Chỉ ra thay vì chỉ mô tả"** — ví dụ làm rõ yêu cầu tinh tế.

```
Đây là ví dụ về kiểu tóm tắt tôi muốn:
Bài báo: [link về quy định AI của EU]
Tóm tắt: EU thông qua Đạo luật AI toàn diện nhắm vào hệ thống rủi ro cao.
Điều khoản chính: yêu cầu minh bạch và giám sát của con người. Hiệu lực từ 2026.

Bây giờ hãy tóm tắt bài báo này theo cùng phong cách: [link bài báo mới]
```

#### 🔴 Kỹ thuật 5 — Permit Uncertainty

Cho phép Claude thừa nhận khi không biết — giảm hallucination:
> *"Phân tích dữ liệu này. Nếu không đủ dữ liệu để kết luận, hãy nói rõ thay vì suy đoán."*

#### 🟣 Kỹ thuật 6 — Chain of Thought

```markdown
# Cách 1 — Đơn giản
"[Yêu cầu]. Hãy suy nghĩ từng bước."

# Cách 2 — Có cấu trúc tag
"Hãy suy nghĩ trong thẻ <thinking>. Phân tích tình huống.
Sau đó viết kết quả trong thẻ <answer>."
```

### Bảng Chọn Kỹ Thuật

| Nếu bạn cần... | Dùng kỹ thuật... |
|----------------|-----------------|
| Định dạng kết quả cụ thể | Examples + chỉ dẫn định dạng |
| Lý luận từng bước | Extended Thinking hoặc Chain of Thought |
| Tác vụ nhiều giai đoạn | Prompt Chaining |
| Tránh bịa đặt | Permit Uncertainty |

### Lỗi Phổ Biến Cần Tránh

| ❌ Lỗi | ✅ Cách sửa |
|--------|-----------|
| Over-engineer prompt | Ngắn gọn thường tốt hơn |
| Kỳ vọng AI đọc suy nghĩ | Nói rõ những gì bạn muốn |
| Dùng tất cả kỹ thuật cùng lúc | Chọn đúng kỹ thuật cho đúng vấn đề |
| AI gợi ý thay vì thực hiện | Thêm: *"Hãy thực hiện thay đổi"* |

---

## 🔵 Bài 3 — Claude Desktop App: Chat, Cowork, Code

### Tổng quan — 3 Chế Độ

```
┌─────────────────────────────────────────┐
│          CLAUDE DESKTOP APP             │
│  ┌─────────┬───────────┬─────────────┐  │
│  │  CHAT   │  COWORK   │    CODE     │  │
│  │ Hội thoại│Thực thi   │ Lập trình  │  │
│  └─────────┴───────────┴─────────────┘  │
└─────────────────────────────────────────┘
```

### 🟢 Chế độ CHAT
- Hỏi đáp, viết lách, brainstorm, học tập
- Claude phản hồi nhưng **không truy cập trực tiếp file**

### 🟡 Chế độ COWORK ⭐

**Cowork = Giao việc thực sự** — biến Claude từ "người tư vấn" thành "người thực thi".

| | Chat | Cowork |
|---|------|--------|
| **Bản chất** | Hội thoại | Phiên làm việc |
| **Khả năng** | Trả lời, gợi ý | **Thực thi, tạo ra sản phẩm** |
| **File** | Không truy cập trực tiếp | Đọc, sửa, tạo file thực |

**Cowork có thể làm:**
- 📂 Tổ chức file — sắp xếp, đổi tên, dọn dẹp thư mục
- 📊 Bảng tính — chuyển ảnh chụp/biên lai thành Excel
- 📝 Báo cáo — tổng hợp từ nhiều file thành tài liệu có định dạng
- ⏰ Tác vụ định kỳ — tự động chạy hàng ngày/tuần theo lịch
- 📱 Từ điện thoại — nhắn lệnh từ phone, desktop thực hiện

> ⚠️ **Bảo mật:** Trước khi thực hiện hành động quan trọng, Claude luôn **hiển thị kế hoạch và chờ phê duyệt**.

### 🔵 Chế độ CODE
Dành cho **developer** — terminal, GitHub integration, codebase-level tasks.

### 💰 Giá & Gói

| Gói | Giá | Cowork |
|-----|-----|--------|
| **Free** | Miễn phí | ❌ |
| **Pro** | $17/tháng | ✅ Tác vụ thông thường |
| **Max 5x** | $100/tháng | ✅ Dùng hàng ngày |
| **Max 20x** | $200/tháng | ✅ Power user |

### Định dạng File Cowork Hỗ Trợ

```
📄 Documents: .docx, .pdf, .txt, .md, .html
📊 Spreadsheets: .xlsx, .xls
📑 Presentations: .pptx
🖼️ Images: .png, .jpg, .jpeg, .gif, .svg, .webp
📋 Data: .csv, .json, .yaml, .xml
💻 Code: .py, .js, .ts, .jsx, .tsx, .java, .go, .rs, .php, .sql...
```

---

## 🟠 Bài 4 — Introduction to Projects

### Projects là gì?

**Projects** là các **không gian làm việc độc lập (self-contained workspaces)** với lịch sử chat và knowledge base riêng — giống như "văn phòng riêng biệt" cho từng dự án.

### Chat Thông Thường vs Projects

| | Chat thường | Projects |
|---|------------|---------|
| **Bộ nhớ** | Bắt đầu lại từ đầu | Nhớ xuyên suốt project |
| **Tài liệu** | Upload lại mỗi lần | Upload một lần, dùng mãi |
| **Hướng dẫn** | Phải nhắc lại mỗi lần | Cài đặt một lần, áp dụng tất cả |
| **Cộng tác** | Chỉ mình bạn | Chia sẻ với team (gói trả phí) |

### Knowledge Base — Upload Tài Liệu

| Loại Project | Nên upload |
|-------------|-----------|
| 📝 Marketing | Style guide, brand guidelines, tone of voice |
| 💻 Development | Codebase, docs kỹ thuật, coding standards |
| 📚 Nghiên cứu | Papers, bài báo, dữ liệu thống kê |
| 🏢 Sales | Pitch deck, case studies, danh sách khách hàng |

### RAG — Tự Động Mở Rộng (Gói Trả Phí)

Khi knowledge base tiếp cận giới hạn, Claude tự động bật **RAG** để mở rộng dung lượng **x10**.

| Gói | Số Projects | RAG |
|-----|-------------|-----|
| **Free** | Tối đa 5 | ❌ |
| **Pro/Max** | Không giới hạn | ✅ ×10 |
| **Team/Enterprise** | Không giới hạn | ✅ ×10 + chia sẻ |

### Hướng Dẫn Tạo Project

```
1. Vào claude.ai/projects
2. Nhấn "+ New Project"
3. Đặt tên và mô tả project
4. Nhấn "+" để upload tài liệu vào Knowledge Base
5. Nhấn "Set project instructions" → viết hướng dẫn → Save
6. Bắt đầu chat trong project!
```

### Ví dụ Project Instructions

```
- Luôn trả lời bằng tiếng Việt
- Giọng điệu chuyên nghiệp nhưng thân thiện
- Khi phân tích dữ liệu, luôn đưa ra 3 insight quan trọng nhất
- Nếu không chắc chắn, hãy nói rõ thay vì đoán
```

### Chia Sẻ Projects (Team & Enterprise)

| Quyền | Được làm gì |
|-------|------------|
| **Can use** | Xem nội dung, knowledge, chat trong project |
| **Can edit** | Chỉnh sửa hướng dẫn, knowledge, quản lý thành viên |

---

## 🔴 Bài 5 — Creating with Artifacts

### Artifacts là gì?

**Artifacts** là nội dung độc lập được Claude tạo ra trong **cửa sổ riêng biệt** — không chỉ là văn bản trong chat mà là thứ bạn có thể chỉnh sửa, chia sẻ, tải về và dùng lại.

### Khi nào Claude tạo Artifacts?
- Có quy mô đáng kể và độc lập (**thường >15 dòng**)
- Là thứ bạn có thể muốn **chỉnh sửa, lặp lại, hoặc tái sử dụng**
- Đại diện cho nội dung phức tạp có thể **đứng một mình**

### Các Loại Artifacts

| Loại | Ví dụ thực tế |
|------|--------------|
| 📄 **Documents** | Báo cáo, bài viết, email template, hợp đồng |
| 💻 **Code snippets** | Script Python, hàm JavaScript, SQL query |
| 🌐 **HTML pages** | Landing page, portfolio, form liên hệ |
| 🖼️ **SVG images** | Logo, icon, biểu đồ vector |
| 📊 **Diagrams** | Flowchart, mindmap, ERD |
| ⚛️ **React components** | Dashboard, calculator, game, quiz tương tác |

### Làm Việc Với Artifacts

**Edit & Iterate:**
```
"Làm cho các nút to hơn"
"Đổi màu sang xanh lá"
"Thêm tính năng timer"
"Dịch sang tiếng Anh"
```

**Forking:** Go back → Click "Edit" → Tạo nhánh → Thử hướng khác → Luôn quay lại bản gốc được.

**Fix Errors:** Khi artifact lỗi → Click **"Try fixing with Claude"** → Claude tự chẩn đoán.

### AI-Powered Artifacts ⭐

Artifacts có thể **nhúng khả năng AI** — biến thành ứng dụng thực sự:
1. Mô tả những gì bạn muốn → Claude viết code → App chạy trên Anthropic infra → User xác thực bằng Claude account
2. **Chi phí chia sẻ: MIỄN PHÍ** — mức sử dụng tính vào giới hạn của từng user, không phải bạn

### MCP Integration & Persistent Storage

- **MCP:** Kết nối với Asana, Google Calendar, Slack...
- **Personal storage:** Mỗi user có dữ liệu riêng (ví dụ: nhật ký)
- **Shared storage:** Tất cả thấy cùng dữ liệu (ví dụ: game leaderboard)
- **Giới hạn:** 20 MB/artifact, Text/JSON only

### Chia Sẻ & Xuất Bản

```
Publish   → Nhận link chia sẻ
Embed     → Nhận embed code cho website
Unpublish → Xóa quyền truy cập (không publish lại được!)
```

---

## 🟣 Bài 6 — Working with Skills

### Skills là gì?

**Skills** là các thư mục chứa hướng dẫn, script và tài nguyên mà Claude **tải động** để thực hiện các tác vụ chuyên biệt theo cách **lặp lại có thể tái tạo** — một lần viết, Claude làm đúng mãi mãi.

### Progressive Disclosure — Cách Skills Hoạt Động

```
Bạn gửi yêu cầu
        ↓
Claude scan Skills có sẵn → Xác định Skills liên quan
        ↓
Tải và áp dụng hướng dẫn từ Skills đó
        ↓
Thực hiện tác vụ đúng theo quy trình của bạn
```

### 4 Loại Skills

| Loại | Mô tả | Ví dụ |
|------|-------|-------|
| 🔵 **Anthropic Skills** | Do Anthropic tạo, tự động kích hoạt | Excel, Word, PowerPoint, PDF |
| 🟢 **Custom Skills** | Do bạn tạo cho workflow riêng | Brand guidelines, email template |
| 🟡 **Organization Skills** | Admin phân phối cho toàn team | Quy trình chuẩn công ty |
| 🟠 **Partner Skills** | Từ Notion, Figma, Atlassian... | Notion workflow, Figma export |

### Skills vs Các Tính Năng Khác

| | Skills | Projects | Custom Instructions | MCP |
|---|--------|----------|--------------------|----|
| **Phạm vi** | Kích hoạt **khi cần** | **Luôn tải** trong project | **Mọi cuộc chat** | Kết nối **dịch vụ ngoài** |
| **Hoạt động** | Động (dynamic) | Tĩnh (static) | Luôn bật | Theo yêu cầu |

### Cách Tạo Custom Skill

**Bước 1: Tạo file `Skill.md`**

```markdown
## Metadata
name: Company Email Template
description: Generate professional emails following company tone and
format for client communications

## Email Structure
- Subject: [Action/FYI/Update] - Topic - [Date]
- Opening: Kính gửi [Tên],
- Body: Tối đa 3 đoạn, bullet points cho action items
- Closing: Trân trọng,

## Tone: Chuyên nghiệp, thân thiện, active voice
```

**Bước 2: Đóng gói**

```
✅ Cấu trúc đúng:
my-skill.zip
└── my-skill/
    ├── Skill.md
    └── resources/ (nếu có)
```

**Bước 3: Upload**

```
Customize → Skills → Nhấn "+" → "Upload a skill" → Upload ZIP
```

### 5 Ví Dụ Custom Skill Thực Tế

```markdown
# 1. Email Template
name: Company Email Template
description: Generate professional emails following company tone for clients

# 2. Meeting Notes
name: Meeting Notes Format
description: Structure meeting notes with decisions, action items, deadlines

# 3. Data Analysis Report
name: Data Analysis Report
description: Analyze data producing reports with executive summary, findings

# 4. Code Review
name: Code Review
description: Review code for quality, security, performance following standards

# 5. Social Media Content
name: Social Media Content
description: Create social posts matching brand voice for LinkedIn, Facebook
```

### Bảo Mật Khi Dùng Skills

- ✅ Chỉ cài Skills từ **nguồn tin cậy**
- ✅ Đọc kỹ nội dung file trước khi bật
- ❌ Không hardcode API keys hay mật khẩu trong Skill
- ❌ Cẩn thận với Skills yêu cầu kết nối mạng ngoài

---

## 🔌 Bài 7 — Connecting Your Tools

### Tại Sao Cần Kết Nối Công Cụ?

Không có Connector:
> *"Viết release notes cho tính năng mới nhất"* → Claude tạo **template chung chung**

Có Connector (Linear):
> *"Viết release notes từ sprint Linear vừa rồi"* → Claude **kéo tickets thực** và tạo release notes chuyên nghiệp

### Nền Tảng Kỹ Thuật — MCP

**MCP (Model Context Protocol)** là tiêu chuẩn mở do Anthropic phát triển:

```
BẠN → CLAUDE → MCP SERVER (Asana, Jira...) → Thực thi hành động
```

### Danh Sách Connectors Chính Thức

| Connector | Làm được gì |
|-----------|------------|
| 📋 **Asana** | Tạo, tìm kiếm và giao task |
| 🔵 **Atlassian** | Track issues, quản lý sprints Jira, tạo docs Confluence |
| 💬 **Intercom** | Phân tích xu hướng support, phân loại issues |
| 📐 **Linear** | Tìm kiếm và tạo issues, projects, comments |
| 💰 **PayPal** | Tạo và quản lý invoices, phân tích sales |
| 🐛 **Sentry** | Tìm kiếm, query và debug errors |
| 💬 **Slack** | Gửi tin nhắn, tạo canvasses (Team/Enterprise) |
| ⚡ **Zapier** | Tự động hóa workflow qua hàng nghìn ứng dụng |

### 2 Loại Connectors

| | Web Connectors (Remote MCP) | Desktop Extensions (Local) |
|---|---|---|
| **Chạy ở** | Máy chủ nhà cung cấp | Máy tính của bạn |
| **Auth** | OAuth | Cài trực tiếp |
| **Gói** | Trả phí | Tất cả users |

### Cách Kết Nối

```
Pro/Max: Settings > Connectors → "Connect"
Team/Enterprise: Admin bật trước → User "Connect"
Trong chat: Nhấn "+" hoặc gõ "/" để chọn connector
```

### 4 Quy Tắc Bảo Mật

1. **Xem xét kỹ quyền** được yêu cầu trong quá trình OAuth
2. **Cảnh giác prompt injections** từ MCP server độc hại
3. **Theo dõi thay đổi** trong hành vi tool
4. **Kiểm soát quyền truy cập** — Claude chỉ truy cập những gì bạn cấp phép

---

## 🏢 Bài 8 — Enterprise Search

### Enterprise Search là gì?

**"Ask Your Org"** project — tìm kiếm thống nhất qua toàn bộ kiến thức tổ chức. Là **"Google nội bộ"** của công ty, vận hành bởi Claude.

> 📌 **Availability:** Chỉ Team và Enterprise plans

### 4 Giá Trị Cốt Lõi

- **Guided setup:** Onboarding dễ dàng kết nối work apps
- **Organization-wide availability:** Tất cả thành viên sau khi Owner cài đặt
- **Optimized instructions:** System prompts do Anthropic duy trì
- **Unified access:** Tìm kiếm qua Slack, Microsoft 365, Google Drive...

### Cài Đặt — Cho Admin (Owner)

```
Bước 1: Click "Ask Your Org" trong sidebar
Bước 2: Click "Set up for your org"
Bước 3: Kết nối connectors
         → Bắt buộc: Documents + Chat
         → Tùy chọn: Email
Bước 4: Đặt tên và mô tả → "Finish set up"
```

### Ví Dụ Câu Hỏi Thực Tế

```
📋 Briefing:  "Chuyện gì đã xảy ra hôm qua khi tôi vắng mặt?"
🔧 Project:   "Blocker hiện tại của dự án Infrastructure là gì?"
📖 Policy:    "Chính sách nghỉ phép của chúng ta là gì?"
🚀 Onboard:   "Hệ thống authentication của chúng ta hoạt động thế nào?"
📊 Review:    "Tóm tắt đóng góp của team cho Platform initiative"
```

### Bảo Mật — Permission-Aware

- Bạn chỉ thấy kết quả từ dữ liệu bạn **có quyền truy cập** trong hệ thống gốc
- Mỗi user xác thực với **thông tin đăng nhập riêng**
- Không có dữ liệu nào được index trong hệ thống Anthropic

### Projects vs Enterprise Search vs Research

| | **Projects** | **Enterprise Search** | **Research** |
|---|---|---|---|
| **System prompt** | User tùy chỉnh | Managed by Anthropic | Managed by Anthropic |
| **Mục đích** | Workspace đa năng | Quick knowledge retrieval | Nghiên cứu sâu, nhiều bước |
| **Tốc độ** | Nhanh | Nhanh | 5–45 phút |

---

## 🔬 Bài 9 — Research Mode for Deep Dives

### Research Mode là gì?

Claude hoạt động theo kiểu **agentic multi-agent** — thực hiện nhiều tìm kiếm xây dựng dựa trên nhau trong khi tự xác định điều gì cần điều tra tiếp theo. Cung cấp câu trả lời **toàn diện trong vài phút**, kèm **trích dẫn dễ kiểm tra**.

> 📌 **Availability:** Pro, Max, Team, Enterprise | **Yêu cầu:** Web Search phải ON

### Kiến Trúc Multi-Agent

```
BẠN gửi query
        ↓
LEAD AGENT (Claude Opus)
  → Phân tích → Phát triển chiến lược → Phân chia subtasks
        ↓          ↓          ↓
  SUBAGENT 1  SUBAGENT 2  SUBAGENT 3
  (tìm web)   (tìm GDrive) (tìm Slack)
        ↓          ↓          ↓
        └──────────┴──────────┘
                   ↓
        BÁO CÁO + TRÍCH DẪN NGUỒN
```

> Multi-agent vượt trội **90.2%** so với single-agent trên internal evaluations của Anthropic.

### 3 Nguồn Dữ Liệu

| Nguồn | Mô tả | Cần thiết lập |
|-------|-------|---------------|
| 🌐 **Web** | Internet công khai | Chỉ cần bật Web Search |
| 📁 **Google Workspace** | Gmail, Drive, Calendar | Kết nối Google Workspace |
| 🔌 **Integrations** | Slack, Jira, Asana... | Kết nối Connectors |

### Thời Gian Research

| Loại query | Thời gian | Ví dụ |
|-----------|-----------|-------|
| Đơn giản | 2–5 phút | "Ai là CEO của Anthropic?" |
| Trung bình | 5–15 phút | "So sánh 5 framework PHP phổ biến nhất 2025" |
| Phức tạp | 15–45 phút | "Phân tích thị trường AI toàn cầu, xu hướng, đối thủ" |

### Khi Nào Dùng Gì?

```
Câu hỏi đơn giản, fact nhanh?         → WEB SEARCH (giây)
Cần suy luận sâu, không cần web?       → EXTENDED THINKING
Cần báo cáo toàn diện từ nhiều nguồn?  → RESEARCH (5-45 phút)
Tìm kiếm nhanh trong tài liệu nội bộ?  → ENTERPRISE SEARCH
```

### Tips Sử Dụng Hiệu Quả

```
# Chỉ định nguồn cụ thể
"Research trong Slack và Google Drive về Q4 product launch"

# Dùng date ranges
"Tóm tắt email từ tuần trước về budget review"

# Kết hợp nhiều nguồn
"Tổng hợp từ SharePoint, Slack và meeting notes về hiring process"

# Nếu Research chưa hoạt động đúng
"Claude, please use the Research tool to..."
```

> ⚠️ Research tự động bật **Extended Thinking** và dùng usage **nhanh hơn** thông thường.

---

## 💼 Bài 10 — Claude in Action: Use Cases by Role

### 💻 Developer / Engineer

**Số liệu thực tế:**
- **60x** phản hồi code review nhanh hơn
- **95%** giảm thời gian chạy tests
- **75%** engineers tiết kiệm 8–10+ giờ/tuần

**Use Cases cụ thể:**

```php
// 1. Code Generation (Laravel example)
"Tạo Repository Pattern hoàn chỉnh cho User model trong Laravel,
bao gồm interface, concrete class, service provider binding,
và unit tests với PHPUnit. Tuân theo SOLID principles và PSR-12."

// 2. Debugging (Claude tự examine files và fix)
"claude fix the authentication error in our login flow"

// 3. Code Review (với GitHub Connector)
"Review PR #247: security, performance, code quality, suggest improvements"

// 4. Documentation
"Đọc file UserController.php và tạo PHPDoc, README section, Postman JSON"

// 5. Architecture Decision
"So sánh WebSockets vs Redis Pub/Sub cho 30,000 concurrent users với Laravel"
```

### 📝 Marketing

| Tác vụ | Prompt mẫu |
|--------|-----------|
| Content Creation | *"Viết 5 biến thể headline cho campaign [X], mỗi cái nhắm pain point khác nhau"* |
| Competitive Intelligence | *"Research chiến lược marketing của [đối thủ]: messaging, channels, pricing"* |
| SEO Content | *"Viết bài blog 1500 từ về [chủ đề], target keyword [X], include H2/H3"* |

### 💼 Sales

```
# Prospect Research
"Research [công ty X] trước demo:
 business model, tech stack, recent news, key decision makers"

# Personalized Outreach
"Viết cold email cho [tên], [chức danh] tại [công ty]
 dựa trên LinkedIn profile, đề cập achievement gần đây"
```

### 📦 Product Management

```
# PRD Writing
"Viết PRD cho tính năng [X]: problem statement, success metrics,
user stories, acceptance criteria, technical requirements"
```

### 👥 HR

```
# JD Creation
"Viết Job Description cho Senior PHP Developer, tránh bias language"

# Interview Framework
"Tạo interview guide: 5 technical questions + rubric,
3 behavioral questions (STAR format), scoring guide 1-5"
```

### ⚖️ Legal

```
# Contract Review
"Review NDA đính kèm: điều khoản bất lợi, missing protections,
red flags về IP ownership. Tạo redlined version với comments"
```

### Prompt Patterns Theo Vai Trò

```
# Developer
"[Context về tech stack] + [Tác vụ cụ thể] +
[Constraints: language version, framework] +
[Output format: code + explanation + tests]"

# Analyst
"[Data/document đính kèm] + [Phân tích theo framework] +
[Audience: executive/technical] + [Output: report/recommendations]"

# Content Creator
"[Target audience] + [Goal: awareness/conversion] +
[Constraints: tone, length, platform] + [Variations: A/B test]"
```

---

## 🌐 Bài 11 — Other Ways to Work with Claude

### Toàn Bộ Hệ Sinh Thái

```
┌─────────────────────────────────────────────────────────┐
│                    HỆ SINH THÁI CLAUDE                  │
├─────────────┬──────────────┬──────────────┬─────────────┤
│  👤 NGƯỜI   │  💻 DEVELOPER│  🏢 DOANH    │  ☁️ CLOUD   │
│   DÙNG     │             │   NGHIỆP     │   PROVIDER  │
├─────────────┼──────────────┼──────────────┼─────────────┤
│ claude.ai   │ Claude Code  │ Team/Enterprise│ AWS Bedrock│
│ Desktop App │ VS Code Ext  │ Enterprise   │Google Vertex│
│ Mobile App  │ JetBrains    │ Search       │MS Foundry  │
│ Chrome Ext  │ API          │ Audit Logs   │            │
│ Excel/PPT   │ Slack        │ SSO/SAML     │            │
└─────────────┴──────────────┴──────────────┴─────────────┘
```

### 🔵 Claude Code — Quan Trọng Nhất Cho Developer

**5 Surfaces của Claude Code:**

| Surface | Cài đặt |
|---------|---------|
| **Terminal CLI** | `curl -fsSL https://claude.ai/install.sh \| bash` (Mac/Linux) |
| **VS Code** | Cài từ VS Code Marketplace |
| **JetBrains** | Cài từ JetBrains Marketplace |
| **Web & iOS** | claude.ai/code (Research Preview) |
| **Slack** | Claude App từ Slack App Directory |

**Tính năng cốt lõi:**
- **CLAUDE.md** — File trong project root, Claude đọc mỗi session
- **Auto memory** — Tự build memory khi làm việc
- **Code onboarding** — Map entire codebase trong vài giây
- **Issues → PRs** — Đọc GitHub issues, viết code, submit PR
- **Auto mode** — Long-running tasks an toàn (2026)

**CLAUDE.md mẫu cho PHP Laravel:**

```markdown
# Project: [Tên dự án]

## Tech Stack
- Laravel 11 + PHP 8.3
- TypeScript + Node.js
- MySQL 8.0

## Coding Standards
- PSR-12 for PHP
- ESLint for TypeScript

## Architecture
- Repository Pattern
- Service Layer
- Event-driven where appropriate

## Testing
- PHPUnit minimum 80% coverage
```

**Cài đặt:**

```bash
# macOS/Linux
curl -fsSL https://claude.ai/install.sh | bash
claude  # Start session đầu tiên
```

### 🌐 Claude in Chrome
Browser extension — Claude trong side panel khi browse web. Cài từ Chrome Web Store.

### 📊 Claude for Excel & PowerPoint
- **Excel Add-in:** Phân tích data, formulas, charts
- **PowerPoint Add-in:** Tạo slides, format, brand templates

### 🔧 Anthropic API — Cho Developer

```typescript
// TypeScript/Node.js
import Anthropic from "@anthropic-ai/sdk";
const client = new Anthropic({ apiKey: process.env.ANTHROPIC_API_KEY });
const message = await client.messages.create({
  model: "claude-sonnet-4-6",
  max_tokens: 1024,
  messages: [{ role: "user", content: "Hello, Claude!" }],
});
```

```php
// PHP (Laravel)
$client = Anthropic::client(config('services.anthropic.key'));
$response = $client->messages()->create([
    'model' => 'claude-sonnet-4-6',
    'max_tokens' => 1024,
    'messages' => [['role' => 'user', 'content' => 'Xin chào!']]
]);
echo $response->content[0]->text;
```

**Tính năng API nổi bật:**

| Feature | Mô tả |
|---------|-------|
| **Streaming** | Real-time text generation |
| **Tool Use** | Function calling, web search |
| **Vision** | Phân tích hình ảnh |
| **Extended Thinking** | Lý luận sâu hơn |
| **Prompt Caching** | Giảm latency và cost |
| **Batch Processing** | Xử lý nhiều request song song |

### Bảng Tóm Tắt — Khi Nào Dùng Surface Nào?

| Surface | Dùng khi | Link |
|---------|---------|------|
| **claude.ai** | Hàng ngày, chat, projects | claude.ai |
| **Mobile App** | On-the-go, voice input | iOS/Android |
| **Claude Code Terminal** | Coding, codebase tasks | `claude` CLI |
| **VS Code Extension** | Inline diffs, IDE integration | VS Code Marketplace |
| **Claude in Chrome** | Browse + Claude side-by-side | Chrome Web Store |
| **Claude for Excel** | Spreadsheet analysis | Office Add-ins |
| **Anthropic API** | Build custom integrations | platform.claude.com |
| **AWS Bedrock** | Deploy on AWS infra | AWS Console |

---

## 🏆 Bài 12 — Conclusion & Certificate

### ✅ Checklist Hoàn Thành Claude 101

```
MEET CLAUDE
☑️ Bài 1: What is Claude?
☑️ Bài 2: Your first conversation + Getting better results
☑️ Bài 3: Claude Desktop App: Chat, Cowork, Code

ORGANIZING YOUR WORK
☑️ Bài 4: Introduction to Projects
☑️ Bài 5: Creating with Artifacts
☑️ Bài 6: Working with Skills

EXPANDING CLAUDE'S REACH
☑️ Bài 7: Connecting your Tools
☑️ Bài 8: Enterprise Search
☑️ Bài 9: Research Mode for Deep Dives

PUTTING IT ALL TOGETHER
☑️ Bài 10: Claude in Action — Use Cases by Role
☑️ Bài 11: Other Ways to Work with Claude
☑️ Bài 12: Conclusion & Certificate
```

### 🎖️ Cách Lấy Chứng Chỉ

```
Bước 1: Đăng ký tại https://anthropic.skilljar.com/claude-101
         → Nhấn "Register | FREE"
Bước 2: Hoàn thành tất cả video lessons
Bước 3: Làm Final Assessment → Đạt điểm pass
Bước 4: Download PDF Certificate
         → Chia sẻ lên LinkedIn (Licenses & Certifications)
```

### 🆕 Claude Certified Architect (3/2026)

Anthropic vừa launch **Claude Certified Architect, Foundations (CCA)**:

| | **Course Completion** | **Claude Certified Architect** |
|---|---|---|
| **Loại** | Hoàn thành khóa học | Thi chuyên nghiệp |
| **Yêu cầu** | Xem video + quiz | Thi proctored, điểm 720/1000 |
| **Phí** | Miễn phí | Trả phí |
| **Giá trị** | Cơ bản, beginner | Production-grade, enterprise |

**5 bước chuẩn bị CCA:**
1. Hoàn thành Claude 101 + AI Fluency
2. Học Building with the Claude API
3. Build ít nhất 2 production projects
4. Hoàn thành Introduction to MCP + Claude Code + Agent Skills
5. Đăng ký thi qua Claude Partner Network

### 🗺️ Lộ Trình Học Tiếp Theo

```
✅ Claude 101 ← ĐÃ HOÀN THÀNH!

🟢 GIAI ĐOẠN 2 — AI Fluency
  ② AI Fluency: Framework & Foundations
     → anthropic.skilljar.com/ai-fluency-framework-foundations

🔵 GIAI ĐOẠN 3 — Developer Track (Ưu tiên cho bạn)
  ③ Building with the Claude API
     → anthropic.skilljar.com/claude-with-the-anthropic-api
  ④ Introduction to Model Context Protocol
     → anthropic.skilljar.com/introduction-to-model-context-protocol
  ⑤ Claude Code in Action
     → anthropic.skilljar.com/claude-code-in-action

🟡 GIAI ĐOẠN 4 — Advanced Developer
  ⑥ MCP: Advanced Topics
     → anthropic.skilljar.com/model-context-protocol-advanced-topics
  ⑦ Introduction to Agent Skills
     → anthropic.skilljar.com/introduction-to-agent-skills
  ⑧ Introduction to Subagents
     → anthropic.skilljar.com/introduction-to-subagents

🟠 GIAI ĐOẠN 5 — Cloud Deployment
  ⑨ Claude with Amazon Bedrock
     → anthropic.skilljar.com/claude-in-amazon-bedrock
  ⑩ Claude with Google Cloud's Vertex AI
     → anthropic.skilljar.com/claude-with-google-vertex
```

### 💡 10 Bài Học Quan Trọng Nhất

```
1.  Claude là AI partner, không chỉ là chatbot
2.  Prompt tốt = kết quả tốt (Be Explicit, Context, Specific)
3.  Projects + Knowledge Base = nhân viên AI biết công ty bạn
4.  Artifacts = sản phẩm thực, không chỉ text trong chat
5.  Skills = dạy Claude làm đúng theo phong cách của bạn
6.  Connectors (MCP) = Claude truy cập công cụ thực của bạn
7.  Research Mode = research chuyên sâu 5-45 phút, có trích dẫn
8.  Enterprise Search = "Google nội bộ" cho cả tổ chức
9.  Claude Code = AI coding agent trong terminal/IDE của bạn
10. Hệ sinh thái rộng = Web, Mobile, API, Cloud, Slack, Excel...
```

---

## 🗺️ Khi Nào Dùng Tính Năng Gì — Master Reference

| Tình huống | Tính năng |
|-----------|----------|
| Hỏi đáp, brainstorm nhanh | **Chat** |
| Muốn Claude *làm việc thực sự* với file | **Cowork** |
| Lập trình, debug, GitHub | **Claude Code** |
| Tổ chức công việc, upload tài liệu 1 lần | **Projects** |
| Tạo nội dung có thể edit/share/download | **Artifacts** |
| Dạy Claude quy trình/phong cách của bạn | **Skills** |
| Cài đặt sở thích cho mọi cuộc chat | **Custom Instructions** |
| Kết nối Claude với Google Drive, Slack... | **MCP Connectors** |
| Tìm kiếm thống nhất toàn tổ chức | **Enterprise Search** |
| Nghiên cứu chuyên sâu, nhiều nguồn | **Research Mode** |
| Tích hợp Claude vào ứng dụng | **API** |
| Deploy trên cloud | **Bedrock / Vertex AI** |

---

## 🔗 Tài Nguyên Hữu Ích

| Tài nguyên | Link |
|-----------|------|
| 🎓 Anthropic Academy | [anthropic.skilljar.com](https://anthropic.skilljar.com) |
| 📖 Documentation | [docs.anthropic.com](https://docs.anthropic.com) |
| ❓ Support Center | [support.claude.com](https://support.claude.com) |
| 🔧 Claude Platform | [platform.claude.com](https://platform.claude.com) |
| 💡 Prompt Engineering | [claude.com/blog/best-practices-for-prompt-engineering](https://claude.com/blog/best-practices-for-prompt-engineering) |
| 🛠️ Skills & Connectors | [claude.com/connectors](https://claude.com/connectors) |
| 💻 Claude Code Docs | [code.claude.com/docs](https://code.claude.com/docs) |
| 🎯 Example Skills GitHub | [github.com/anthropics/skills](https://github.com/anthropics/skills) |
| 📐 Agent Skills Standard | [agentskills.io](https://agentskills.io) |
| 🏆 Partner Network / CCA | [anthropic.com/news/claude-partner-network](https://www.anthropic.com/news/claude-partner-network) |

---

> 📝 **Ghi chú:** Tài liệu này được tổng hợp từ khóa học Claude 101 trên [Anthropic Academy](https://anthropic.skilljar.com/claude-101).
> Nội dung dựa trên tài liệu chính thức của Anthropic — cập nhật tháng 3/2026.
>
> **Tiếp theo:** Khóa học **Building with the Claude API** — dành riêng cho developer PHP Laravel / TypeScript / Node.js.

---

*Happy learning! Chúc bạn sớm lấy được Certificate và tiến lên các khóa tiếp theo! 🚀*
