# ielts-phuongg-iuu
trang web học IELTS của phuongg iu
// File: index.html

<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>IELTS của vợgg 💖</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <div class="container">
    <h1>🎀 Trang học IELTS màu hường của Vợgg 🎀</h1>

    <img src="https://i.pinimg.com/564x/fb/b0/93/fbb0934a2975f0703496d85db166c040.jpg" alt="Hình học cute" class="main-img"/>

    <div class="tabs">
      <button onclick="showTab('roadmap')">📘 Lộ trình</button>
      <button onclick="showTab('vocab')">📗 Từ vựng</button>
      <button onclick="showTab('grammar')">📙 Ngữ pháp</button>
      <button onclick="showTab('ai')">🤖 AI hỗ trợ</button>
    </div>

    <div class="tab-content" id="roadmap">
      <h2>Lộ trình học từ 0 → 6.0+</h2>
      <ul>
        <li>Giai đoạn 1: Học phát âm, từ vựng cơ bản</li>
        <li>Giai đoạn 2: Luyện 4 kỹ năng từng phần</li>
        <li>Giai đoạn 3: Luyện đề + tăng band điểm</li>
      </ul>
    </div>

    <div class="tab-content" id="vocab" style="display:none">
      <h2>Từ vựng chủ đề Môi trường 🌱</h2>
      <p><strong>Pollution</strong> /pəˈluː.ʃən/ – ô nhiễm</p>
      <img src="https://i.pinimg.com/564x/c2/aa/f9/c2aaf96dba4166f0eea1be4f9c7e922e.jpg" class="mini-img"/>
    </div>

    <div class="tab-content" id="grammar" style="display:none">
      <h2>Thì hiện tại đơn</h2>
      <p>Cấu trúc: S + V(s/es)</p>
      <p>Ví dụ: She studies English every day.</p>
    </div>

    <div class="tab-content" id="ai" style="display:none">
      <h2>AI hỗ trợ học tập</h2>
      <ul>
        <li>Sửa lỗi phát âm 🗣️</li>
        <li>Sửa bài viết Task 1 & 2 ✍️</li>
        <li>Gợi ý từ vựng/ngữ pháp phù hợp 📚</li>
      </ul>
    </div>
  </div>

  <script>
    function showTab(id) {
      document.querySelectorAll('.tab-content').forEach(el => el.style.display = 'none');
      document.getElementById(id).style.display = 'block';
    }
  </script>
</body>
</html>

// File: style.css

body {
  background-color: #ffe4f2;
  font-family: 'Comic Sans MS', cursive, sans-serif;
  color: #d63384;
  text-align: center;
  padding: 20px;
}

.container {
  max-width: 800px;
  margin: auto;
}

h1 {
  font-size: 2rem;
  margin-bottom: 1rem;
}

.tabs button {
  background-color: #ffb3d9;
  border: none;
  padding: 10px 15px;
  margin: 5px;
  border-radius: 10px;
  cursor: pointer;
  font-weight: bold;
}

.tabs button:hover {
  background-color: #ff66a3;
  color: white;
}

.tab-content {
  background: #fff0f5;
  border-radius: 10px;
  padding: 15px;
  margin-top: 15px;
}

.main-img {
  width: 250px;
  border-radius: 20px;
  margin: 15px 0;
}

.mini-img {
  width: 150px;
  margin-top: 10px;
}
