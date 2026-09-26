# Medical Visa Undertaking Generator

100% client-side web application for generating medical visa undertaking documents and parental consent forms.

## Features

- ✅ Upload invitation letter (PDF) and extract required information
- ✅ Support for patient + 1-3 attendants
- ✅ Generate Undertaking documents with optional signatures
- ✅ Generate Parental Consent forms (for applicants under 18)
- ✅ Signature editor with crop, rotate, brightness, and contrast controls
- ✅ Phone-based signature upload via QR code
- ✅ Direct camera capture for signatures
- ✅ Multi-mission support (Dhaka, Chittagong, Rajshahi, Sylhet, Khulna)
- ✅ Download all documents as PDF

## How to Deploy

### Option 1: Vercel (Recommended)

1. **Create GitHub account** (if not already): https://github.com/signup
2. **Upload to GitHub:**
   ```bash
   git init
   git add .
   git commit -m "Medical Visa Undertaking Generator"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/medical-visa-gen.git
   git push -u origin main
   ```
3. **Deploy on Vercel:** https://vercel.com
   - Click "Import Project"
   - Select your GitHub repository
   - Click Deploy
   - Your site will be live at `https://medical-visa-gen.vercel.app`

### Option 2: Netlify

1. **Upload to GitHub** (same as above)
2. **Deploy on Netlify:** https://netlify.com
   - Connect your GitHub account
   - Select the repository
   - Click Deploy
   - Your site will be live at `https://medical-visa-gen.netlify.app`

### Option 3: GitHub Pages (Free)

1. **Upload to GitHub** (same as above)
2. **Enable GitHub Pages:**
   - Go to Settings → Pages
   - Select main branch
   - Your site will be live at `https://YOUR_USERNAME.github.io/medical-visa-gen/`

### Option 4: Your Own cPanel (If you have hosting)

1. **Upload files via cPanel File Manager:**
   - Extract this folder
   - Upload to `public_html`
   - Visit your domain

## File Structure

```
medical-visa-gen/
├── index.html              # Main application
├── README.md               # This file
├── .gitignore              # Git ignore file
└── assets/
    ├── js/
    │   ├── app.js          # Main application logic
    │   └── tsaf-promo.js   # Promotional popup (disabled)
    ├── css/
    │   └── bengali.css     # Additional Bengali styling
    └── vendor/
        ├── pdf.min.js      # PDF reader
        ├── pdf-lib.min.js  # PDF generator
        └── qrcode.min.js   # QR code generator
```

## Requirements

- Modern web browser (Chrome, Firefox, Safari, Edge)
- Internet connection (for CDN fonts)
- No server-side processing required

## Features Breakdown

### Invitation Letter Upload
- Reads PDF and extracts key fields:
  - Full Name
  - Passport Number
  - Hospital Name & Address
  - Purpose of Treatment
  - Mobile Number

### Undertaking Document
- Patient/Attendant signature (optional)
- Signature editor with:
  - Cropping
  - Rotation
  - Brightness/Contrast adjustment
  - White background removal

### Parental Consent
- Only shown for applicants under 18
- Father's signature (optional)
- Mother's signature (optional)
- Same signature editing tools

### Signature Upload Methods
1. **Drag & Drop** - Upload image files
2. **Direct Camera** - Capture with device camera
3. **Phone Link** - QR code for remote upload from phone

## Technical Stack

- **Frontend**: Pure vanilla JavaScript (no frameworks)
- **PDF Processing**: 
  - PDF.js (reading/extracting)
  - PDFLib (generation/editing)
- **Canvas API**: Image editing
- **QRCode.js**: QR generation
- **Storage**: Browser localStorage (no server needed)

## Version

v2.1 - Multi-mission support with QR-based remote signature upload

## License

Free to use and modify for medical visa applications.

---

**Note:** This application is 100% client-side. All data processing happens in your browser. Nothing is uploaded to any server.
