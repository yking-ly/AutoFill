# AutoFill — local-first form assistant

AutoFill is a privacy-first Chrome extension for job seekers, students, hackathon participants, and anyone who repeatedly types the same information into online forms.

It stores your profile, saved answers, and selected files locally in Chrome. There is no AutoFill backend, analytics, tracking, or AI service in the current public version.

## Features

- **One-click autofill:** Fill supported fields such as name, email, phone, country code, GitHub, LinkedIn, portfolio, Discord, and custom profile fields.
- **Smart scan:** Highlight detected fields before filling them:
  - Green — structured fields AutoFill can complete.
  - Blue — a matching answer from your local Q&A bank.
  - Amber — a new or unsupported question that needs manual review.
- **Personal Q&A bank:** Save reusable answers for open-ended questions. Suggestions use local fuzzy matching and are never inserted without your review.
- **File vaults:** Store one resume, cover letter, and profile photo locally. Files are limited to 5 MB each and are attached only when you click AutoFill.
- **Custom profile fields:** Add fields for information specific to your applications.
- **Backup:** Export and import your local profile, answers, and files as JSON.
- **Persistent side panel:** Keep the AutoFill controls open while browsing a form.
- **Multi-step form support:** Scan again after a form reveals additional fields.

## Privacy

AutoFill is local-first. Profile data, Q&A answers, settings, and selected files are stored in Chrome’s local extension storage. The extension does not send this data to an AutoFill server or third-party AI service.

Read the complete [Privacy Policy](PRIVACY.md).

## Install for development

1. Open `chrome://extensions` in Chrome.
2. Enable **Developer mode**.
3. Click **Load unpacked** and select the extension folder.
4. Pin AutoFill, open the side panel, and complete your Profile.
5. Open a supported application form and click **AutoFill** or **Scan page**.

## Reporting a problem or suggesting an improvement

Please [open a GitHub Issue](https://github.com/vking-ly/AutoFill/issues) if:

- A website or webpage is not scanned correctly.
- A field is detected but is not autofilled correctly.
- The wrong file is selected or an upload field is not recognized.
- You have a feature request, compatibility report, or usability suggestion.

When reporting a website issue, include the site name, the type of field that failed, and the steps to reproduce it. Do not include passwords, API keys, resumes, personal contact details, or screenshots containing sensitive information.

Contributions are welcome. Fork the repository, make your change, and open a [pull request](https://github.com/vking-ly/AutoFill/pulls).

## Future scope

Planned directions include:

- Optional AI-assisted drafting with explicit user controls and privacy disclosures.
- Visa and government forms.
- College and scholarship applications.
- Medical and insurance forms.
- E-commerce checkout profiles.
- Multiple profiles for personal, work, and freelance use.
- Form history and fill review.

## Project structure

```text
manifest.json
background.js
content.js
content.css
popup/popup.html
popup/popup.js
popup/popup.css
icons/
```

## License

AutoFill is proprietary software. All rights reserved.

This repository is public for documentation, issue tracking, and collaboration.
The code may not be copied, modified, redistributed, or used commercially
without written permission from the copyright holder.
