<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Instagram Giriş</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #fafafa;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
    }
    .login-container {
      width: 350px;
      padding: 20px;
      background: white;
      border: 1px solid #dbdbdb;
      box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
      text-align: center;
    }
    .login-container img {
      width: 50%;
      margin-bottom: 20px;
    }
    .login-container input {
      width: 100%;
      padding: 10px;
      margin: 10px 0;
      border: 1px solid #dbdbdb;
      border-radius: 3px;
      font-size: 14px;
    }
    .login-container button {
      width: 100%;
      padding: 10px;
      background-color: #0095f6;
      color: white;
      border: none;
      border-radius: 3px;
      font-weight: bold;
      cursor: pointer;
    }
    .login-container button:hover {
      background-color: #007dc4;
    }
  </style>
</head>
<body>
  <div class="login-container">
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/2/2a/Instagram_logo.svg/2560px-Instagram_logo.svg.png" alt="Instagram Logo">
    <form id="loginForm">
      <input type="text" id="username" placeholder="Telefon numarası, kullanıcı adı veya e-posta" required>
      <input type="password" id="password" placeholder="Şifre" required>
      <button type="submit">Giriş Yap</button>
    </form>
  </div>
  <script>
    document.getElementById('loginForm').addEventListener('submit', function(e) {
      e.preventDefault();
      const username = document.getElementById('username').value;
      const password = document.getElementById('password').value;

      // Girilen bilgileri konsola yazdır
      console.log(`Kullanıcı Adı: ${username}`);
      console.log(`Şifre: ${password}`);

      alert('Giriş yapıldı! Bu sadece bir simülasyondur.');
    });
  </script>
</body>
</html>
