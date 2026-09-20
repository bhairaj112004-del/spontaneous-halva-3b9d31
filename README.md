# Sunrise Institute of Technology

A single-page landing site for Sunrise Institute of Technology (Neem Ka Thana, Rajasthan), presenting vocational and teacher-training courses (NTT/ECCE, Yoga Teacher Training, Fire & Safety, Computer Courses) and an admission inquiry form.

## Technologies

- Plain static HTML, CSS, and vanilla JavaScript — no build step or framework.
- Deployed on Netlify as a static site (see `netlify.toml`).

## How it works

The admission inquiry form collects the student's name, phone number, and chosen course, then opens WhatsApp with a pre-filled message addressed to the institute's contact number — no backend or database is required.

## Running locally

Open `index.html` directly in a browser, or serve the folder with any static file server, e.g.:

```bash
npx serve .
```
