<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Đăng Ký Câu Lạc Bộ</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f5f5f5;
        }
        .container {
            max-width: 600px;
            margin: 50px auto;
            background: #ffffff;
            padding: 20px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            border-radius: 8px;
        }
        h1 {
            text-align: center;
            color: #333333;
        }
        form {
            display: flex;
            flex-direction: column;
        }
        label {
            margin-bottom: 5px;
            font-weight: bold;
        }
        input, select, textarea, button {
            margin-bottom: 15px;
            padding: 10px;
            font-size: 16px;
            border: 1px solid #cccccc;
            border-radius: 4px;
        }
        button {
            background-color: #007bff;
            color: #ffffff;
            border: none;
            cursor: pointer;
        }
        button:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Đăng Ký Câu Lạc Bộ</h1>
        <form action="xu_ly_dang_ki.php" method="POST">
            <label for="name">Họ và tên:</label>
            <input type="text" id="name" name="name" required>

            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>

            <label for="phone">Số điện thoại:</label>
            <input type="tel" id="phone" name="phone" required>

            <label for="club">Chọn câu lạc bộ:</label>
            <select id="club" name="club" required>
                <option value="" disabled selected>Chọn câu lạc bộ...</option>
                <option value="clb_bong_da">Câu lạc bộ Bóng Đá</option>
                <option value="clb_bong_chuyen">Câu lạc bộ Bóng Chuyền</option>
                <option value="clb_sach">Câu lạc bộ Sách</option>
                <option value="clb_cong_nghe">Câu lạc bộ Công Nghệ</option>
            </select>

            <label for="message">Ghi chú (tùy chọn):</label>
            <textarea id="message" name="message" rows="4" placeholder="Nhập ghi chú của bạn..."></textarea>

            <button type="submit">Đăng Ký</button>
        </form>
    </div>
</body>
</html>
