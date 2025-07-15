<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>สมัครสมาชิก</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background: linear-gradient(to bottom right, #000000, #000000);
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
        }
        .register-container {
            background: white;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
            width: 350px;
            text-align: center;
        }
        .register-container h2 {
            color: #3366ff;
        }
        .input-group {
            margin: 15px 0;
            text-align: left;
        }
        .input-group label {
            display: block;
            font-weight: bold;
        }
        .input-group input {
            width: 100%;
            padding: 10px;
            margin-top: 5px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        .btn {
            background: linear-gradient(to right, #ff3c7f, #5a68f5);
            color: white;
            padding: 12px;
            width: 100%;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
            margin-top: 10px;
        }
        .btn:hover {
            opacity: 0.9;
        }
        .error {
            color: red;
            font-size: 14px;
            margin-top: 5px;
        }
        .logo {
            width: 120px;
            height: auto;
            margin-bottom: 0px;
        }
    </style>
</head>
<body>

    <div class="register-container">
        <img src="logoyolo.jpg" alt="logo" class="logo">
        <h2>สมัครสมาชิก</h2>
        <p>กรุณากรอกข้อมูลเพื่อสมัครสมาชิก</p>
        <form action="register.php" method="POST">
            <div class="input-group">
                <label for="username">ชื่อผู้ใช้</label>
                <input type="text" id="username" name="username" placeholder="กรอกชื่อผู้ใช้" required>
            </div>
            <div class="input-group">
                <label for="password">รหัสผ่าน</label>
                <input type="password" id="password" name="password" placeholder="กรอกรหัสผ่าน" required>
            </div>
            <div class="input-group">
                <label for="confirm_password">ยืนยันรหัสผ่าน</label>
                <input type="password" id="confirm_password" name="confirm_password" placeholder="ยืนยันรหัสผ่าน" required>
            </div>
            <div class="input-group">
                <label for="phone">เบอร์โทรศัพท์</label>
                <input type="text" id="phone" name="phone" placeholder="กรอกเบอร์โทรศัพท์" required>
            </div>
            <button type="submit" class="btn">ยืนยัน</button>
        </form>
    </div>

</body>
</html>
