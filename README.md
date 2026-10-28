# UPI QR Code Payment Generator

A Python script that generates dynamic UPI payment QR codes for major Indian payment apps, including **PhonePe**, **Paytm**, and **Google Pay**.

## 🚀 Features

- Prompts for your UPI ID at runtime.
- Automatically creates app-specific UPI payment deep links.
- Generates high-resolution QR codes using `qrcode` and `Pillow`.
- Saves the QR codes as PNG images (`phonepe_qr.png`, `paytm_qr.png`, `google_pay_qr.png`).
- Displays the generated QR codes directly on your screen.

---

## 🛠️ Installation

1. **Clone this repository**:
   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
   cd <repo-name>
   ```

2. **Install required dependencies**:
   ```bash
   pip install -r requirements.txt
   ```
   *(or `pip install qrcode[pil]`)*

---

## 💻 Usage

Run the script using Python:

```bash
python takepaymentonline.py
```

When prompted, enter your UPI ID (e.g. `yourname@oksbi` or `yourname@upi`). The script will generate, save, and display the payment QR codes.

---

## ⚙️ Customization

Inside [`takepaymentonline.py`](takepaymentonline.py), you can customize the payment parameters such as recipient name, amount, or transaction note:

```python
# Format: upi://pay?pa=UPI_ID&pn=Recipient%20Name&am=Amount&cu=CURRENCY&tn=MESSAGE
phonepe_url = f'upi://pay?pa={upi_id}&pn=Your%20Name&mc=1234'
```
