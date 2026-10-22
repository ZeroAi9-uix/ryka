# RYKA Support Website

A clean, responsive support page for **RYKA**, an independent music project. The website allows users to voluntarily support development through UPI payments using a direct payment link and a QR code.

## Features

- **Responsive Design** — Works on desktop, tablet, and mobile.
- **Custom Logo** — Display your own RYKA logo in the header.
- **UPI Payments** — Open a compatible UPI payment app directly.
- **Copy UPI ID** — Quickly copy the payment ID.
- **QR Code Support** — Display your UPI QR code for scanning.
- **Developer Watermark** — Includes the centered credit “Developed by Himanshu”.
- **GitHub Pages Ready** — Deploy as a static website without a backend.

## Tech Stack

- HTML5
- CSS3
- Vanilla JavaScript
- UPI payment deep links
- GitHub Pages

## Project Structure

```text
ryka-support/
├── index.html
├── logo.jpeg
├── upi-qrcode.jpeg
└── README.md
```

**Files:**
- `index.html` — Main website page and styling.
- `logo.jpeg` — Your custom RYKA logo.
- `upi-qrcode.jpeg` — Your UPI payment QR image.
- `README.md` — Project documentation.

Make sure the image filenames match the paths used in `index.html`.

## Configuration

### 1. Set Your UPI ID

Open `index.html` and find:

```javascript
const UPI_ID = "auraxraj67@fam";
```

Replace the value with your correct UPI ID if it changes. Ensure the displayed UPI ID and payment link use the same ID.

### 2. Add Your Custom Logo

Place your logo image in the repository root and update this HTML line if needed:

```html
<img src="ryka-logo.jpeg" alt="RYKA Logo" class="brand-logo">
```

The logo is constrained to a small header area using CSS.

### 3. Add Your UPI QR Code

Place your QR image in the repository root and ensure the image path matches:

```html
<img id="qrImage" src="upi-qrcode.jpeg" alt="RYKA UPI payment QR code">
```

Use a valid payment QR code and verify its recipient details before publishing.

## Run Locally

1. Download or clone this repository.
2. Keep `index.html` and the image files in the correct locations.
3. Open `index.html` in a browser.

For a local development server, you can use the VS Code Live Server extension.

## Deploy with GitHub Pages

1. Create a GitHub repository, such as `ryka-support`.
2. Upload `index.html`, `logo.jpeg`, `upi-qrcode.jpeg`, and `README.md` to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Select the `main` branch and the `/ (root)` folder.
6. Click **Save**.
7. Wait for deployment and open the published URL shown in GitHub Pages settings.

## Security & Payment Notice

- This is a static website, not a payment gateway.
- Payments are handled by the user's selected UPI app.
- Always verify the recipient and amount before authorizing a payment.
- Never share your UPI PIN or OTP.
- The website does not itself confirm or track completed payments.

## Developer

**Developed by Himanshu**

Created for the RYKA independent music project.

---

Thank you for supporting RYKA and its continued development.
