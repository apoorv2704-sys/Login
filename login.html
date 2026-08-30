<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Sign In</title>
<style>
  :root {
    --ink: #1c2b2d;
    --paper: #eef3f2;
    --card: #ffffff;
    --accent: #2f6f5e;
    --accent-dark: #234f42;
    --line: #d8e2e0;
    --error: #c04a3d;
  }

  * { box-sizing: border-box; }

  body {
    margin: 0;
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    background: var(--paper);
    font-family: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
    color: var(--ink);
    padding: 24px;
  }

  .card {
    background: var(--card);
    width: 100%;
    max-width: 380px;
    border-radius: 14px;
    padding: 40px 32px;
    box-shadow: 0 20px 40px rgba(28, 43, 45, 0.08);
    border: 1px solid var(--line);
  }

  .card h1 {
    margin: 0 0 6px;
    font-size: 24px;
    letter-spacing: -0.02em;
  }

  .card p.sub {
    margin: 0 0 28px;
    color: #61716f;
    font-size: 14px;
  }

  label {
    display: block;
    font-size: 13px;
    font-weight: 600;
    margin-bottom: 6px;
    color: #3d4a49;
  }

  .field { margin-bottom: 18px; }

  input {
    width: 100%;
    padding: 11px 13px;
    border: 1px solid var(--line);
    border-radius: 8px;
    font-size: 15px;
    background: #fafcfb;
    color: var(--ink);
    transition: border-color 0.15s ease, box-shadow 0.15s ease;
  }

  input:focus {
    outline: none;
    border-color: var(--accent);
    box-shadow: 0 0 0 3px rgba(47, 111, 94, 0.15);
    background: #fff;
  }

  .error-msg {
    color: var(--error);
    font-size: 12px;
    margin-top: 5px;
    min-height: 14px;
  }

  button.login-btn {
    width: 100%;
    padding: 12px;
    background: var(--accent);
    color: #fff;
    border: none;
    border-radius: 8px;
    font-size: 15px;
    font-weight: 600;
    cursor: pointer;
    margin-top: 8px;
    transition: background 0.15s ease, transform 0.05s ease;
  }

  button.login-btn:hover { background: var(--accent-dark); }
  button.login-btn:active { transform: scale(0.98); }

  .success-box {
    display: none;
    text-align: center;
    padding: 10px 0 4px;
  }

  .success-box.show { display: block; }

  .checkmark {
    width: 56px;
    height: 56px;
    border-radius: 50%;
    background: var(--accent);
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 0 auto 16px;
  }

  .checkmark svg { width: 28px; height: 28px; }

  .success-box h2 { margin: 0 0 6px; font-size: 20px; }
  .success-box p { margin: 0 0 4px; color: #61716f; font-size: 14px; }

  .success-box .detail {
    font-size: 13px;
    color: var(--ink);
    background: var(--paper);
    border-radius: 8px;
    padding: 12px 14px;
    margin-top: 18px;
    text-align: left;
  }

  .success-box .detail div {
    display: flex;
    justify-content: space-between;
    padding: 4px 0;
    font-size: 13px;
  }

  .success-box .detail span:first-child { color: #61716f; }

  .form-wrap.hide { display: none; }
</style>
</head>
<body>

<div class="card">

  <div class="form-wrap" id="formWrap">
    <h1>Welcome</h1>
    <p class="sub">Sign in with your details to continue</p>

    <form id="loginForm" novalidate>
      <div class="field">
        <label for="fullName">Full Name</label>
        <input type="text" id="fullName" placeholder="John Doe">
        <div class="error-msg" id="nameError"></div>
      </div>

      <div class="field">
        <label for="email">Email</label>
        <input type="email" id="email" placeholder="john@example.com">
        <div class="error-msg" id="emailError"></div>
      </div>

      <div class="field">
        <label for="mobile">Mobile Number</label>
        <input type="tel" id="mobile" placeholder="9876543210">
        <div class="error-msg" id="mobileError"></div>
      </div>

      <button type="submit" class="login-btn">Login</button>
    </form>
  </div>

  <div class="success-box" id="successBox">
    <div class="checkmark">
      <svg viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="3" stroke-linecap="round" stroke-linejoin="round">
        <polyline points="20 6 9 17 4 12"></polyline>
      </svg>
    </div>
    <h2>Login Successfully</h2>
    <p>You're signed in. Welcome aboard!</p>
    <div class="detail" id="userDetail"></div>
  </div>

</div>

<script>
  const form = document.getElementById('loginForm');
  const formWrap = document.getElementById('formWrap');
  const successBox = document.getElementById('successBox');
  const userDetail = document.getElementById('userDetail');

  const nameInput = document.getElementById('fullName');
  const emailInput = document.getElementById('email');
  const mobileInput = document.getElementById('mobile');

  const nameError = document.getElementById('nameError');
  const emailError = document.getElementById('emailError');
  const mobileError = document.getElementById('mobileError');

  function isValidEmail(value) {
    return /^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(value);
  }

  function isValidMobile(value) {
    return /^[0-9]{10}$/.test(value);
  }

  form.addEventListener('submit', function (e) {
    e.preventDefault();

    let valid = true;
    nameError.textContent = '';
    emailError.textContent = '';
    mobileError.textContent = '';

    const name = nameInput.value.trim();
    const email = emailInput.value.trim();
    const mobile = mobileInput.value.trim();

    if (name.length < 2) {
      nameError.textContent = 'Please enter your full name.';
      valid = false;
    }

    if (!isValidEmail(email)) {
      emailError.textContent = 'Please enter a valid email address.';
      valid = false;
    }

    if (!isValidMobile(mobile)) {
      mobileError.textContent = 'Please enter a valid 10-digit mobile number.';
      valid = false;
    }

    if (!valid) return;

    userDetail.innerHTML = `
      <div><span>Name</span><span>${name}</span></div>
      <div><span>Email</span><span>${email}</span></div>
      <div><span>Mobile</span><span>${mobile}</span></div>
    `;

    formWrap.classList.add('hide');
    successBox.classList.add('show');
  });
</script>

</body>
</html>



