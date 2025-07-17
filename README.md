# ☕ Coffee UID – Sign-Up, Login, Personal Info & Ordering System

A responsive front-end web application for a coffee ordering service with complete user authentication (sign-up/login), personal info capture, and ordering workflow. Built using HTML, CSS, and vanilla JavaScript.

---

## 🔐 Authentication System

### ✅ Sign-Up
- Input fields: First Name, Last Name, Username, Password
- Password validation: must start with a **capital letter**
- Valid users are stored in a temporary array (in-memory storage)
- JS alert confirms success

### ✅ Login
- Validates username/password against the stored users array
- On successful match → redirects to `info.html`
- On failure → shows inline error message

---

## 🧾 Personal Information Form (info.html)

- Captures personal data: Name, Email, Phone, Address, Postal Code
- **POSTs data to SheetDB API** (`https://sheetdb.io/api/v1/zrbsnimsdc9r0`)
- After submission, auto-redirects to `home.html`
- Includes form validation and styled checkboxes
- External JS (`info.js`) handles async POST request

---

## 🛒 Ordering System (order.html + cart.html)

- Users can:
  - Browse coffee items
  - Add to cart
  - View cart in `cart.html`
- Dynamic JavaScript handles:
  - Cart management (add/remove)
  - Quantity updates
  - Total price calculation
  - Simple localStorage to preserve cart state (optional)

---

## 🎨 UI Features

| Feature             | Description                                              |
|---------------------|----------------------------------------------------------|
| Responsive Design   | CSS media queries for mobile/tablet                      |
| Blurred Backgrounds | `backdrop-filter` for frosted-glass effect               |
| Clean Form Design   | Margin/padding consistency for UX                        |
| Hover Effects       | Buttons and input highlights                            |
| Central Containers  | Centered layout using flexbox and margins                |

---

## 🛠 Tech Stack

- HTML5, CSS3, Vanilla JavaScript
- SheetDB API (for form data storage)
- Responsive CSS for various screen sizes



