<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Vista Grammar MCQ - Ôn thi vào 10 THPT</title>
  <style>
    :root {
      --orange: #f97316;
      --orange-dark: #ea580c;
      --blue: #0f172a;
      --text: #1e293b;
      --muted: #64748b;
      --card: #ffffff;
      --border: #e2e8f0;
      --green: #16a34a;
      --red: #dc2626;
      --yellow: #facc15;
      --shadow: 0 18px 45px rgba(15, 23, 42, 0.12);
    }

    * { box-sizing: border-box; }

    body {
      margin: 0;
      font-family: Arial, Helvetica, sans-serif;
      color: var(--text);
      background: radial-gradient(circle at top left, rgba(249,115,22,.18), transparent 35%), linear-gradient(135deg, #fff7ed 0%, #ffffff 45%, #eff6ff 100%);
      min-height: 100vh;
    }

    header {
      padding: 14px 18px 12px;
      border-bottom: 1px solid var(--border);
      background: rgba(255,255,255,.94);
      backdrop-filter: blur(10px);
      position: relative;
      z-index: 1;
    }

    .header-inner {
      max-width: 1180px;
      margin: auto;
      display: grid;
      grid-template-columns: 1fr 320px;
      gap: 14px;
      align-items: center;
    }

    .brand {
      display: flex;
      gap: 12px;
      align-items: center;
      margin-bottom: 6px;
    }

    .logo {
      width: 40px;
      height: 40px;
      border-radius: 16px;
      background: linear-gradient(135deg, var(--orange), #fb923c);
      color: white;
      display: grid;
      place-items: center;
      font-weight: 900;
      font-size: 20px;
      box-shadow: 0 10px 24px rgba(249,115,22,.28);
    }

    h1 {
      margin: 0;
      font-size: clamp(22px, 3vw, 34px);
      line-height: 1.12;
      letter-spacing: -1px;
      color: var(--blue);
    }

    .subtitle {
      margin: 8px 0 0;
      color: var(--muted);
      line-height: 1.45;
      max-width: 760px;
      font-size: 14px;
    }

    .hero-card {
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: 20px;
      padding: 12px;
      box-shadow: 0 8px 22px rgba(15, 23, 42, 0.08);
      font-size: 14px;
    }

    .hero-card b { color: var(--orange-dark); }

    .stats {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 8px;
      margin-top: 8px;
    }

    .stat {
      background: #fff7ed;
      border: 1px solid #fed7aa;
      border-radius: 18px;
      padding: 8px 6px;
      text-align: center;
    }

    .stat strong {
      display: block;
      font-size: 18px;
      color: var(--orange-dark);
    }

    .stat span {
      font-size: 12px;
      color: var(--muted);
    }

    main {
      max-width: 1180px;
      margin: 16px auto 50px;
      padding: 0 18px;
    }

    .layout {
      display: grid;
      grid-template-columns: 330px 1fr;
      gap: 18px;
      align-items: start;
    }

    .panel, .quiz-card, .history-card {
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: 28px;
      box-shadow: 0 12px 32px rgba(15,23,42,.08);
    }

    .panel {
      padding: 18px;
      position: sticky;
      top: 16px;
    }

    .panel h2, .history-card h2 {
      margin: 0 0 14px;
      font-size: 20px;
      color: var(--blue);
    }

    label {
      display: block;
      font-weight: 800;
      color: var(--blue);
      margin: 14px 0 8px;
      font-size: 14px;
    }

    select {
      width: 100%;
      border: 1px solid var(--border);
      border-radius: 16px;
      padding: 12px 14px;
      font-size: 15px;
      outline: none;
      background: #f8fafc;
    }

    select:focus {
      border-color: #fdba74;
      box-shadow: 0 0 0 4px rgba(249,115,22,.14);
    }

    .btn-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 10px;
      margin-top: 14px;
    }

    button {
      border: 0;
      cursor: pointer;
      border-radius: 999px;
      padding: 12px 16px;
      font-weight: 900;
      transition: .2s ease;
      font-size: 14px;
    }

    .primary {
      background: var(--orange);
      color: white;
      box-shadow: 0 10px 22px rgba(249,115,22,.24);
    }

    .primary:hover { background: var(--orange-dark); transform: translateY(-1px); }

    .secondary {
      background: #f1f5f9;
      color: var(--blue);
      border: 1px solid var(--border);
    }

    .secondary:hover { background: #e2e8f0; }

    .danger {
      background: #fee2e2;
      color: #991b1b;
      border: 1px solid #fecaca;
    }

    .score-box {
      margin-top: 16px;
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 8px;
    }

    .score-item {
      background: #f8fafc;
      border: 1px solid var(--border);
      border-radius: 16px;
      padding: 10px;
      text-align: center;
    }

    .score-item b {
      display: block;
      font-size: 20px;
      color: var(--orange-dark);
    }

    .score-item span { font-size: 12px; color: var(--muted); }

    .progress-wrap {
      margin-top: 15px;
      background: #f1f5f9;
      border-radius: 999px;
      height: 12px;
      overflow: hidden;
      border: 1px solid var(--border);
    }

    .progress-bar {
      width: 0%;
      height: 100%;
      background: linear-gradient(90deg, var(--orange), #fb923c);
      transition: .25s ease;
    }

    .mini-note {
      margin-top: 12px;
      color: var(--muted);
      font-size: 13px;
      line-height: 1.5;
    }

    .quiz-card {
      padding: 20px;
      min-height: 480px;
    }

    .top-row {
      display: flex;
      justify-content: space-between;
      gap: 12px;
      flex-wrap: wrap;
      align-items: center;
      margin-bottom: 16px;
    }

    .badges {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
    }

    .badge {
      display: inline-flex;
      align-items: center;
      gap: 5px;
      border-radius: 999px;
      padding: 7px 10px;
      font-size: 12px;
      font-weight: 900;
      background: #f1f5f9;
      color: #475569;
      border: 1px solid var(--border);
    }

    .badge.orange {
      background: #fff7ed;
      color: #c2410c;
      border-color: #fed7aa;
    }

    .badge.green {
      background: #dcfce7;
      color: #166534;
      border-color: #86efac;
    }

    .question-number {
      color: var(--muted);
      font-weight: 800;
    }

    .question-box {
      background: linear-gradient(135deg, #fff7ed, #ffffff);
      border: 1px solid #fed7aa;
      border-radius: 26px;
      padding: 18px;
      margin-bottom: 14px;
    }

    .question-type {
      color: var(--orange-dark);
      font-weight: 900;
      margin-bottom: 8px;
    }

    .question-text {
      font-size: clamp(18px, 2.4vw, 26px);
      line-height: 1.35;
      font-weight: 900;
      color: var(--blue);
      white-space: pre-line;
    }

    .prompt-vi {
      margin-top: 12px;
      color: var(--muted);
      line-height: 1.5;
      font-size: 15px;
    }

    .options {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 12px;
      margin: 16px 0;
    }

    .option-btn {
      background: #f8fafc;
      color: var(--blue);
      border: 1px solid var(--border);
      border-radius: 18px;
      padding: 16px;
      text-align: left;
      line-height: 1.45;
      font-weight: 800;
      min-height: 74px;
    }

    .option-btn:hover:not(:disabled) {
      background: #fff7ed;
      border-color: #fdba74;
      transform: translateY(-1px);
    }

    .option-btn.correct {
      background: #dcfce7;
      border-color: #86efac;
      color: #166534;
    }

    .option-btn.wrong {
      background: #fee2e2;
      border-color: #fecaca;
      color: #991b1b;
    }

    .answer-box {
      display: none;
      margin-top: 16px;
      border-radius: 24px;
      border: 1px solid #bbf7d0;
      background: #f0fdf4;
      padding: 18px;
      line-height: 1.6;
    }

    .answer-box.show { display: block; animation: fadeIn .2s ease; }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(8px); }
      to { opacity: 1; transform: translateY(0); }
    }

    .answer-title {
      font-weight: 900;
      color: #166534;
      margin-bottom: 6px;
    }

    .answer-main {
      font-size: 18px;
      font-weight: 900;
      color: var(--blue);
    }

    .explain {
      margin-top: 8px;
      color: #166534;
    }

    .action-row {
      display: flex;
      gap: 10px;
      flex-wrap: wrap;
      margin-top: 16px;
    }

    .history-card {
      padding: 18px;
      margin-top: 18px;
    }

    .history-list {
      display: grid;
      gap: 10px;
      max-height: 330px;
      overflow: auto;
      padding-right: 4px;
    }

    .history-item {
      border: 1px solid var(--border);
      border-radius: 18px;
      padding: 12px;
      background: #f8fafc;
      line-height: 1.45;
    }

    .history-item b { color: var(--orange-dark); }

    .empty {
      color: var(--muted);
      text-align: center;
      padding: 18px;
      background: #f8fafc;
      border: 1px dashed var(--border);
      border-radius: 18px;
    }

    @media (max-width: 900px) {
      .header-inner, .layout { grid-template-columns: 1fr; }
      .panel { position: static; }
      .hero-card { display: none; }
      header { padding: 12px 14px; }
      .subtitle { display: none; }
    }

    @media (max-width: 620px) {
      .btn-grid, .score-box, .stats, .options { grid-template-columns: 1fr; }
      .quiz-card { padding: 18px; }
    }
  </style>
</head>
<body>
  <header>
    <div class="header-inner">
      <div>
        <div class="brand">
          <div class="logo">V</div>
          <div>
            <strong>Vista Learning Hub</strong><br />
            <span style="color:#64748b">Grammar MCQ - Thi vào 10 THPT</span>
          </div>
        </div>
        <h1>Trắc nghiệm ngữ pháp tiếng Anh vào 10</h1>
        <p class="subtitle">Web app luyện nhanh ngữ pháp theo dạng A/B/C/D: chọn chuyên đề, random câu hỏi, chọn đáp án, xem giải thích và tính điểm tự động.</p>
      </div>
      <div class="hero-card">
        <b>Phù hợp kiểm tra đầu giờ</b>
        <p style="color:#64748b;line-height:1.55;margin-bottom:0">Giáo viên chiếu màn hình, chọn chuyên đề, bấm random. Học sinh chọn đáp án trong 10-20 giây, app tự hiện đúng/sai và giải thích.</p>
        <div class="stats">
          <div class="stat"><strong id="totalQuestions">0</strong><span>Câu hỏi</span></div>
          <div class="stat"><strong>12</strong><span>Chủ đề</span></div>
          <div class="stat"><strong>4</strong><span>Đáp án A-D</span></div>
        </div>
      </div>
    </div>
  </header>

  <main>
    <div class="layout">
      <aside class="panel">
        <h2>⚙️ Bảng điều khiển</h2>

        <label for="topicSelect">Chọn chủ đề</label>
        <select id="topicSelect">
          <option value="all">Tất cả chủ đề</option>
          <option value="Tenses">Thì động từ</option>
          <option value="Passive">Câu bị động</option>
          <option value="Reported Speech">Câu tường thuật</option>
          <option value="Conditional & Wish">Điều kiện & câu ước</option>
          <option value="Relative Clauses">Mệnh đề quan hệ</option>
          <option value="Comparison">So sánh</option>
          <option value="Conjunctions">Liên từ</option>
          <option value="Prepositions">Giới từ</option>
          <option value="Verb Forms">Dạng động từ</option>
          <option value="Modal Verbs">Động từ khuyết thiếu</option>
          <option value="Word Forms">Từ loại</option>
          <option value="Rewrite">Viết lại câu</option>
        </select>

        <label for="levelSelect">Mức độ</label>
        <select id="levelSelect">
          <option value="all">Tất cả</option>
          <option value="Nhận biết">Nhận biết</option>
          <option value="Thông hiểu">Thông hiểu</option>
          <option value="Vận dụng">Vận dụng</option>
        </select>

        <div class="btn-grid">
          <button class="primary" onclick="nextQuestion()">🎲 Random câu</button>
          <button class="secondary" onclick="speakQuestion()">🔊 Đọc câu</button>
          <button class="secondary" onclick="showAnswer()">👀 Xem đáp án</button>
          <button class="danger" onclick="resetQuiz()">↺ Làm lại</button>
        </div>

        <div class="score-box">
          <div class="score-item"><b id="correctCount">0</b><span>Đúng</span></div>
          <div class="score-item"><b id="wrongCount">0</b><span>Sai</span></div>
          <div class="score-item"><b id="accuracy">0%</b><span>Tỉ lệ đúng</span></div>
        </div>

        <div class="progress-wrap">
          <div id="progressBar" class="progress-bar"></div>
        </div>

        <p class="mini-note">Gợi ý dùng trên lớp: chọn “Tất cả chủ đề” để ôn tổng hợp, hoặc chọn từng chuyên đề để kiểm tra nhanh sau mỗi buổi học.</p>
      </aside>

      <section>
        <div class="quiz-card">
          <div class="top-row">
            <div class="badges">
              <span class="badge orange" id="topicBadge">Chủ đề</span>
              <span class="badge" id="levelBadge">Mức độ</span>
              <span class="badge green">Trắc nghiệm A/B/C/D</span>
            </div>
            <div class="question-number" id="questionNumber">Câu #1</div>
          </div>

          <div class="question-box">
            <div class="question-type" id="questionType">Mark the letter A, B, C or D</div>
            <div class="question-text" id="questionText">Bấm “Random câu” để bắt đầu luyện tập.</div>
            <div class="prompt-vi" id="promptVi">Chọn đáp án đúng nhất.</div>
          </div>

          <div id="optionsBox" class="options"></div>

          <div id="answerBox" class="answer-box">
            <div class="answer-title">Đáp án & giải thích</div>
            <div class="answer-main" id="answerMain"></div>
            <div class="explain" id="explainText"></div>
          </div>

          <div class="action-row">
            <button class="primary" onclick="nextQuestion()">Câu tiếp theo</button>
            <button class="secondary" onclick="showAnswer()">Xem đáp án</button>
          </div>
        </div>

        <div class="history-card">
          <h2>📌 Lịch sử câu đã làm</h2>
          <div id="historyList" class="history-list">
            <div class="empty">Chưa có câu hỏi nào.</div>
          </div>
        </div>
      </section>
    </div>
  </main>

  <script>
    const questionBank = [
      // TENSES
      {topic:'Tenses', level:'Nhận biết', q:'She usually ______ to school by bike.', options:['go','goes','is going','went'], answer:'B', explain:'Usually là dấu hiệu của hiện tại đơn. Chủ ngữ She nên động từ thêm -s: goes.'},
      {topic:'Tenses', level:'Nhận biết', q:'Look! The boys ______ football in the yard.', options:['play','plays','are playing','played'], answer:'C', explain:'Look! diễn tả hành động đang xảy ra tại thời điểm nói, dùng hiện tại tiếp diễn: are playing.'},
      {topic:'Tenses', level:'Nhận biết', q:'My father ______ TV every evening.', options:['watch','watches','is watching','watched'], answer:'B', explain:'Every evening là dấu hiệu hiện tại đơn. My father là chủ ngữ số ít nên dùng watches.'},
      {topic:'Tenses', level:'Thông hiểu', q:'I ______ my homework before I watched TV last night.', options:['finish','finished','had finished','have finished'], answer:'C', explain:'Hành động hoàn thành trước một hành động khác trong quá khứ dùng quá khứ hoàn thành: had finished.'},
      {topic:'Tenses', level:'Thông hiểu', q:'We ______ English for five years.', options:['learn','learned','have learned','are learning'], answer:'C', explain:'For five years dùng với hiện tại hoàn thành: have learned.'},
      {topic:'Tenses', level:'Vận dụng', q:'The last time I met him was two years ago.', options:['I met him for two years.','I have met him for two years.','I haven’t met him for two years.','I didn’t meet him since two years.'], answer:'C', explain:'The last time + S + V2 + was + time ago → S + haven’t/hasn’t + V3 + for + time.'},

      // PASSIVE
      {topic:'Passive', level:'Nhận biết', q:'English ______ all over the world.', options:['speaks','is spoken','spoke','is speaking'], answer:'B', explain:'Câu bị động hiện tại đơn: am/is/are + V3/ed. English is spoken.'},
      {topic:'Passive', level:'Nhận biết', q:'This school ______ ten years ago.', options:['built','was built','is built','has built'], answer:'B', explain:'Ten years ago là quá khứ đơn. Bị động quá khứ đơn: was/were + V3/ed.'},
      {topic:'Passive', level:'Thông hiểu', q:'People grow rice in many Asian countries.', options:['Rice grows in many Asian countries.','Rice is grown in many Asian countries.','Rice was grown in many Asian countries.','Rice has grown in many Asian countries.'], answer:'B', explain:'Chuyển sang bị động hiện tại đơn: Rice is grown.'},
      {topic:'Passive', level:'Thông hiểu', q:'They are building a new bridge now.', options:['A new bridge is built now.','A new bridge was built now.','A new bridge is being built now.','A new bridge has been built now.'], answer:'C', explain:'Hiện tại tiếp diễn bị động: am/is/are + being + V3/ed.'},
      {topic:'Passive', level:'Vận dụng', q:'My father has someone repair his car.', options:['My father has his car repair.','My father has his car repaired.','My father has repaired his car.','My father is repaired his car.'], answer:'B', explain:'Cấu trúc bị động sai khiến: have + something + V3/ed.'},
      {topic:'Passive', level:'Vận dụng', q:'People say that he is a good doctor.', options:['He says to be a good doctor.','He is said to be a good doctor.','He is said that a good doctor.','He was said being a good doctor.'], answer:'B', explain:'Bị động tường thuật: S + is/are said + to V.'},

      // REPORTED SPEECH
      {topic:'Reported Speech', level:'Nhận biết', q:'He said, “I am tired.”', options:['He said that I am tired.','He said that he is tired.','He said that he was tired.','He said that he tired.'], answer:'C', explain:'I → he; am → was khi chuyển sang câu tường thuật.'},
      {topic:'Reported Speech', level:'Nhận biết', q:'She said, “I will call you.”', options:['She said she will call me.','She said she would call me.','She said she called me.','She said she calls me.'], answer:'B', explain:'Will → would trong câu tường thuật.'},
      {topic:'Reported Speech', level:'Thông hiểu', q:'“Where do you live?” he asked me.', options:['He asked me where I lived.','He asked me where did I live.','He asked me where do I live.','He asked me where I live?'], answer:'A', explain:'Câu hỏi gián tiếp dùng trật tự câu kể: wh-word + S + V.'},
      {topic:'Reported Speech', level:'Thông hiểu', q:'“Don’t make noise,” the teacher said to us.', options:['The teacher told us don’t make noise.','The teacher told us not to make noise.','The teacher said us not make noise.','The teacher told us not making noise.'], answer:'B', explain:'Câu mệnh lệnh phủ định: told + O + not to V.'},
      {topic:'Reported Speech', level:'Vận dụng', q:'She asked me what was my name.', options:['Correct sentence','what my name was','what is my name','what my name is?'], answer:'B', explain:'Câu hỏi gián tiếp không đảo động từ: what my name was.'},

      // CONDITIONAL & WISH
      {topic:'Conditional & Wish', level:'Nhận biết', q:'If it rains tomorrow, we ______ at home.', options:['stay','will stay','stayed','would stay'], answer:'B', explain:'Điều kiện loại 1: If + hiện tại đơn, S + will + V.'},
      {topic:'Conditional & Wish', level:'Nhận biết', q:'If I ______ you, I would study harder.', options:['am','was','were','will be'], answer:'C', explain:'Câu điều kiện loại 2: If I were you, ...'},
      {topic:'Conditional & Wish', level:'Thông hiểu', q:'I don’t have enough money, so I can’t buy this bike.', options:['If I have enough money, I can buy this bike.','If I had enough money, I could buy this bike.','If I had enough money, I can buy this bike.','If I had had enough money, I could buy this bike.'], answer:'B', explain:'Tình huống trái với hiện tại dùng điều kiện loại 2: If + V2/ed, S + could/would + V.'},
      {topic:'Conditional & Wish', level:'Thông hiểu', q:'I am not good at English.', options:['I wish I am good at English.','I wish I was good at English.','I wish I were good at English.','I wish I will be good at English.'], answer:'C', explain:'Wish hiện tại: S + wish + S + V2/ed/were.'},
      {topic:'Conditional & Wish', level:'Vận dụng', q:'I didn’t go to the party last night.', options:['I wish I went to the party last night.','I wish I had gone to the party last night.','I wish I have gone to the party last night.','I wish I would go to the party last night.'], answer:'B', explain:'Wish quá khứ: S + wish + S + had + V3/ed.'},
      {topic:'Conditional & Wish', level:'Vận dụng', q:'If he will come early, we will start the meeting.', options:['Correct sentence','will come → comes','will start → start','come → came'], answer:'B', explain:'Trong mệnh đề if của điều kiện loại 1 không dùng will.'},

      // RELATIVE CLAUSES
      {topic:'Relative Clauses', level:'Nhận biết', q:'The man ______ is standing over there is my uncle.', options:['who','which','where','when'], answer:'A', explain:'Who thay cho người và làm chủ ngữ trong mệnh đề quan hệ.'},
      {topic:'Relative Clauses', level:'Nhận biết', q:'This is the book ______ I bought yesterday.', options:['who','which','where','when'], answer:'B', explain:'Which thay cho vật. Trong câu này which làm tân ngữ của bought.'},
      {topic:'Relative Clauses', level:'Thông hiểu', q:'The girl is very friendly. She sits next to me.', options:['The girl which sits next to me is very friendly.','The girl who sits next to me is very friendly.','The girl where sits next to me is very friendly.','The girl when sits next to me is very friendly.'], answer:'B', explain:'She thay cho The girl và làm chủ ngữ → dùng who.'},
      {topic:'Relative Clauses', level:'Thông hiểu', q:'The students who are studying in the library are from class 9A.', options:['The students study in the library are from class 9A.','The students studying in the library are from class 9A.','The students studied in the library are from class 9A.','The students to study in the library are from class 9A.'], answer:'B', explain:'Mệnh đề quan hệ chủ động có thể rút gọn bằng V-ing.'},
      {topic:'Relative Clauses', level:'Vận dụng', q:'The city which I was born is very beautiful.', options:['Correct sentence','which → who','which → where','which → when'], answer:'C', explain:'Chỉ nơi chốn cần dùng where hoặc in which.'},

      // COMPARISON
      {topic:'Comparison', level:'Nhận biết', q:'This exercise is ______ than that one.', options:['difficult','more difficult','most difficult','the most difficult'], answer:'B', explain:'Tính từ dài dùng more + adj + than.'},
      {topic:'Comparison', level:'Nhận biết', q:'Nam is ______ student in my class.', options:['tall','taller','the tallest','most tall'], answer:'C', explain:'So sánh nhất: the + adj-est.'},
      {topic:'Comparison', level:'Thông hiểu', q:'The more you practice, ______ you become.', options:['the good','the better','better','best'], answer:'B', explain:'Cấu trúc so sánh kép: The + comparative, the + comparative.'},
      {topic:'Comparison', level:'Thông hiểu', q:'No one in my class is taller than Nam.', options:['Nam is taller than no one in my class.','Nam is the tallest student in my class.','Nam is as tall as everyone in my class.','Nam is not the tallest student in my class.'], answer:'B', explain:'No one ... taller than Nam → Nam is the tallest.'},
      {topic:'Comparison', level:'Vận dụng', q:'He is more taller than his brother.', options:['Correct sentence','more taller → taller','than → as','brother → brothers'], answer:'B', explain:'Không dùng đồng thời more và -er.'},

      // CONJUNCTIONS
      {topic:'Conjunctions', level:'Nhận biết', q:'He was tired, ______ he finished his homework.', options:['so','but','because','and'], answer:'B', explain:'But diễn tả sự tương phản: mệt nhưng vẫn hoàn thành.'},
      {topic:'Conjunctions', level:'Nhận biết', q:'She studies hard ______ she can pass the exam.', options:['because','although','so that','but'], answer:'C', explain:'So that + S + can/could/will/would + V diễn tả mục đích.'},
      {topic:'Conjunctions', level:'Thông hiểu', q:'Although it rained heavily, we went to school.', options:['Despite it rained heavily, we went to school.','In spite of the heavy rain, we went to school.','Because of the heavy rain, we went to school.','Although the heavy rain, we went to school.'], answer:'B', explain:'Although + clause → In spite of/Despite + noun phrase/V-ing.'},
      {topic:'Conjunctions', level:'Thông hiểu', q:'The test was so difficult that many students couldn’t finish it.', options:['It was such difficult test that many students couldn’t finish it.','It was such a difficult test that many students couldn’t finish it.','It was so a difficult test that many students couldn’t finish it.','It was too difficult test that many students couldn’t finish it.'], answer:'B', explain:'So + adj + that → such + a/an + adj + noun + that.'},
      {topic:'Conjunctions', level:'Vận dụng', q:'Because he was ill, so he stayed at home.', options:['Correct sentence','Bỏ Because','Bỏ so','Bỏ stayed'], answer:'C', explain:'Không dùng đồng thời because và so trong cùng một câu phức.'},

      // PREPOSITIONS
      {topic:'Prepositions', level:'Nhận biết', q:'We have English class ______ Monday morning.', options:['in','on','at','by'], answer:'B', explain:'On dùng với ngày và buổi của một ngày cụ thể: on Monday morning.'},
      {topic:'Prepositions', level:'Nhận biết', q:'My birthday is ______ July.', options:['in','on','at','from'], answer:'A', explain:'In dùng với tháng, năm, mùa.'},
      {topic:'Prepositions', level:'Thông hiểu', q:'She is interested ______ learning English.', options:['in','on','at','for'], answer:'A', explain:'Interested in + N/V-ing.'},
      {topic:'Prepositions', level:'Thông hiểu', q:'He is good ______ Maths but bad ______ English.', options:['in/in','at/at','for/for','on/on'], answer:'B', explain:'Good at, bad at.'},
      {topic:'Prepositions', level:'Vận dụng', q:'I am looking forward to see you soon.', options:['Correct sentence','to see → seeing','to see → to seeing','looking → look'], answer:'C', explain:'Look forward to + V-ing. Từ “to” trong cụm này là giới từ.'},

      // VERB FORMS
      {topic:'Verb Forms', level:'Nhận biết', q:'She enjoys ______ books in her free time.', options:['read','to read','reading','reads'], answer:'C', explain:'Enjoy + V-ing.'},
      {topic:'Verb Forms', level:'Nhận biết', q:'My parents want me ______ harder.', options:['study','studying','to study','studied'], answer:'C', explain:'Want + O + to V.'},
      {topic:'Verb Forms', level:'Thông hiểu', q:'I stopped ______ because I was tired.', options:['work','to work','working','worked'], answer:'C', explain:'Stop V-ing = dừng việc đang làm.'},
      {topic:'Verb Forms', level:'Thông hiểu', q:'Would you mind ______ the window?', options:['open','to open','opening','opened'], answer:'C', explain:'Would you mind + V-ing?'},
      {topic:'Verb Forms', level:'Vận dụng', q:'It is necessary for you to revise the lesson.', options:['You need revise the lesson.','You need to revise the lesson.','You need revising the lesson.','You need revised the lesson.'], answer:'B', explain:'It is necessary for somebody to V → Somebody need(s) to V.'},

      // MODAL VERBS
      {topic:'Modal Verbs', level:'Nhận biết', q:'You ______ wear a helmet when riding a motorbike.', options:['can','may','must','might'], answer:'C', explain:'Must diễn tả sự bắt buộc mạnh.'},
      {topic:'Modal Verbs', level:'Nhận biết', q:'You ______ smoke here. It is not allowed.', options:['must','mustn’t','don’t have to','should'], answer:'B', explain:'Mustn’t = không được phép làm gì.'},
      {topic:'Modal Verbs', level:'Thông hiểu', q:'It ______ rain later. Look at those dark clouds!', options:['must','should','may','can’t'], answer:'C', explain:'May/might diễn tả khả năng có thể xảy ra.'},
      {topic:'Modal Verbs', level:'Thông hiểu', q:'It isn’t necessary for you to finish it today.', options:['You mustn’t finish it today.','You don’t have to finish it today.','You can’t finish it today.','You shouldn’t finish it today.'], answer:'B', explain:'It isn’t necessary → don’t/doesn’t have to.'},
      {topic:'Modal Verbs', level:'Vận dụng', q:'He can plays the guitar very well.', options:['Correct sentence','plays → play','can → cans','guitar → guitars'], answer:'B', explain:'Sau modal verbs dùng động từ nguyên thể không “to”.'},

      // WORD FORMS
      {topic:'Word Forms', level:'Nhận biết', q:'English is an ______ language.', options:['interest','interested','interesting','interestingly'], answer:'C', explain:'Trước danh từ cần tính từ. Interesting = thú vị.'},
      {topic:'Word Forms', level:'Nhận biết', q:'She sings very ______.', options:['beautiful','beauty','beautifully','beautify'], answer:'C', explain:'Sings là động từ, cần trạng từ beautifully.'},
      {topic:'Word Forms', level:'Thông hiểu', q:'We should protect the ______.', options:['environment','environmental','environmentally','environmentalist'], answer:'A', explain:'Protect + noun. The environment = môi trường.'},
      {topic:'Word Forms', level:'Thông hiểu', q:'He is a very ______ businessman.', options:['success','successful','successfully','succeed'], answer:'B', explain:'Trước danh từ businessman cần tính từ successful.'},
      {topic:'Word Forms', level:'Vận dụng', q:'The children played ______ in the park.', options:['happy','happiness','happily','unhappy'], answer:'C', explain:'Played là động từ nên cần trạng từ happily.'},

      // REWRITE
      {topic:'Rewrite', level:'Thông hiểu', q:'He is too young to drive a car.', options:['He is young enough to drive a car.','He isn’t old enough to drive a car.','He is so old that he can drive a car.','He isn’t too old to drive a car.'], answer:'B', explain:'Too + adj + to V → not + opposite adj + enough + to V.'},
      {topic:'Rewrite', level:'Thông hiểu', q:'The book was so interesting that I couldn’t put it down.', options:['It was such an interesting book that I couldn’t put it down.','It was such interesting book that I couldn’t put it down.','It was so an interesting book that I couldn’t put it down.','It was too interesting book that I couldn’t put it down.'], answer:'A', explain:'So + adj + that → such + a/an + adj + noun + that.'},
      {topic:'Rewrite', level:'Thông hiểu', q:'Because the weather was bad, we stayed at home.', options:['Because of the bad weather, we stayed at home.','Because of the weather was bad, we stayed at home.','Despite the bad weather, we stayed at home.','Although the bad weather, we stayed at home.'], answer:'A', explain:'Because + clause → Because of + noun phrase/V-ing.'},
      {topic:'Rewrite', level:'Vận dụng', q:'“Why don’t we go camping this weekend?” he said.', options:['He suggested to go camping that weekend.','He suggested going camping that weekend.','He suggested that going camping that weekend.','He suggested go camping this weekend.'], answer:'B', explain:'Suggest + V-ing. This weekend → that weekend trong câu tường thuật.'},
      {topic:'Rewrite', level:'Vận dụng', q:'I can’t speak English fluently.', options:['I wish I can speak English fluently.','I wish I could speak English fluently.','I wish I will speak English fluently.','I wish I speak English fluently.'], answer:'B', explain:'Wish hiện tại với khả năng: wish + S + could + V.'}
    ];

    let current = null;
    let questionIndex = 0;
    let answered = false;
    let history = [];
    const score = { correct: 0, wrong: 0 };

    document.getElementById('totalQuestions').textContent = questionBank.length;

    function filteredBank() {
      const topic = document.getElementById('topicSelect').value;
      const level = document.getElementById('levelSelect').value;
      return questionBank.filter(item => {
        const topicOk = topic === 'all' || item.topic === topic;
        const levelOk = level === 'all' || item.level === level;
        return topicOk && levelOk;
      });
    }

    function nextQuestion() {
      const bank = filteredBank();
      if (!bank.length) {
        alert('Không có câu hỏi phù hợp với bộ lọc hiện tại. Hãy chọn lại chủ đề hoặc mức độ.');
        return;
      }

      current = bank[Math.floor(Math.random() * bank.length)];
      questionIndex++;
      answered = false;

      document.getElementById('answerBox').classList.remove('show');
      document.getElementById('topicBadge').textContent = current.topic;
      document.getElementById('levelBadge').textContent = current.level;
      document.getElementById('questionNumber').textContent = `Câu #${questionIndex}`;
      document.getElementById('questionType').textContent = 'Mark the letter A, B, C or D to indicate the correct answer.';
      document.getElementById('questionText').textContent = current.q;
      document.getElementById('promptVi').textContent = 'Chọn đáp án đúng nhất.';
      document.getElementById('answerMain').textContent = `Đáp án đúng: ${current.answer}. ${current.options[letterToIndex(current.answer)]}`;
      document.getElementById('explainText').textContent = current.explain;
      renderOptions();
    }

    function renderOptions() {
      const box = document.getElementById('optionsBox');
      box.innerHTML = '';
      current.options.forEach((option, index) => {
        const letter = String.fromCharCode(65 + index);
        const btn = document.createElement('button');
        btn.className = 'option-btn';
        btn.textContent = `${letter}. ${option}`;
        btn.onclick = () => chooseAnswer(letter, btn);
        box.appendChild(btn);
      });
    }

    function chooseAnswer(letter, btn) {
      if (answered || !current) return;
      answered = true;

      const isCorrect = letter === current.answer;
      if (isCorrect) score.correct++;
      else score.wrong++;

      document.querySelectorAll('.option-btn').forEach((optionBtn, index) => {
        const optionLetter = String.fromCharCode(65 + index);
        optionBtn.disabled = true;
        if (optionLetter === current.answer) optionBtn.classList.add('correct');
        if (optionLetter === letter && !isCorrect) optionBtn.classList.add('wrong');
      });

      showAnswer();
      updateScore();
      addHistory(current, letter, isCorrect);
    }

    function showAnswer() {
      if (!current) {
        nextQuestion();
        return;
      }
      document.getElementById('answerBox').classList.add('show');
    }

    function updateScore() {
      const total = score.correct + score.wrong;
      const accuracy = total ? Math.round((score.correct / total) * 100) : 0;
      document.getElementById('correctCount').textContent = score.correct;
      document.getElementById('wrongCount').textContent = score.wrong;
      document.getElementById('accuracy').textContent = `${accuracy}%`;
      document.getElementById('progressBar').style.width = `${accuracy}%`;
    }

    function resetQuiz() {
      score.correct = 0;
      score.wrong = 0;
      questionIndex = 0;
      history = [];
      updateScore();
      renderHistory();
      nextQuestion();
    }

    function addHistory(item, selected, isCorrect) {
      history.unshift({
        topic: item.topic,
        q: item.q,
        selected,
        correct: item.answer,
        status: isCorrect ? 'Đúng' : 'Sai'
      });
      history = history.slice(0, 12);
      renderHistory();
    }

    function renderHistory() {
      const list = document.getElementById('historyList');
      if (!history.length) {
        list.innerHTML = '<div class="empty">Chưa có câu hỏi nào.</div>';
        return;
      }
      list.innerHTML = history.map((item, index) => `
        <div class="history-item">
          <b>${index + 1}. ${escapeHtml(item.topic)} - ${item.status}</b><br />
          ${escapeHtml(item.q)}<br />
          <span style="color:#64748b">Bạn chọn: ${item.selected} | Đáp án: ${item.correct}</span>
        </div>
      `).join('');
    }

    function letterToIndex(letter) {
      return letter.charCodeAt(0) - 65;
    }

    function escapeHtml(text) {
      return String(text)
        .replaceAll('&', '&amp;')
        .replaceAll('<', '&lt;')
        .replaceAll('>', '&gt;')
        .replaceAll('"', '&quot;')
        .replaceAll("'", '&#039;');
    }

    function speakQuestion() {
      if (!current) {
        nextQuestion();
        return;
      }
      if (!('speechSynthesis' in window)) {
        alert('Trình duyệt chưa hỗ trợ đọc tự động.');
        return;
      }
      speechSynthesis.cancel();
      const optionText = current.options.map((o, i) => `${String.fromCharCode(65 + i)}. ${o}`).join('. ');
      const text = `${current.q}. ${optionText}`.replace(/______/g, 'blank');
      const utterance = new SpeechSynthesisUtterance(text);
      utterance.lang = 'en-US';
      utterance.rate = 0.82;
      utterance.pitch = 1;
      speechSynthesis.speak(utterance);
    }

    nextQuestion();
  </script>
</body>
</html>
