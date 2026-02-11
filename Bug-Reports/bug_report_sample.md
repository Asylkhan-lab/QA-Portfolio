# BUG-001: Login button remains disabled after invalid credentials (requires page refresh)

**Environment:** Windows 10, Chrome 121, Web app build 1.0.12

**Preconditions:** User account exists

**Steps to Reproduce:**
1. Open Login page
2. Enter valid email: `test.user@example.com`
3. Enter invalid password: `WrongPass!`
4. Click **Log in**
5. Observe error message
6. Correct the password to a valid one
7. Try clicking **Log in** again

**Actual Result:**
- The **Log in** button stays disabled and cannot be clicked until the page is refreshed.

**Expected Result:**
- After correcting credentials, the **Log in** button becomes enabled and user can retry login.

**Severity:** Major  
**Priority:** High

**Attachments:**
- (add screenshot/video)

**Notes:**
- Reproduces 3/3 times
- Possible front-end state not reset after failed request
