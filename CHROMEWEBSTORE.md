# Chrome Web Store Metadata — AutoFill

## Extension overview

**Name:** AutoFill — Form Autofill

**Single purpose:** AutoFill helps users fill supported online forms using profile information, saved answers, and files that the user provides.

## Permission justifications

| Permission | Justification |
| :--- | :--- |
| `storage` | Stores the user’s profile, Q&A bank, selected files, and extension settings locally in Chrome so AutoFill can reuse them during form filling. |
| `sidePanel` | Provides the persistent AutoFill interface for managing profile data, saved answers, files, and form-fill controls while the user browses. |
| `webNavigation` | Enumerates frames on the active page so AutoFill can reach supported fields inside embedded forms and iframes. |
| `<all_urls>` host permission | Application forms are hosted across many domains. AutoFill needs webpage access to identify supported fields, show scan highlights, fill user-provided values, and attach selected files after the user initiates an action. |

The current package does not request `activeTab` or `scripting`; those permissions are not required by the current implementation.

## Data use

AutoFill stores profile data, Q&A answers, selected files, and settings locally in Chrome. The current public version does not send this data to the developer, an AutoFill backend, an AI provider, analytics services, or advertisers.

## Privacy policy

`https://github.com/vking-ly/AutoFill/blob/main/PRIVACY.md`

## Support

`https://github.com/vking-ly/AutoFill/issues`

Use GitHub Issues for website compatibility reports, fields that are not scanned or autofilled, upload problems, and feature suggestions. Users should not post passwords, API keys, resumes, or other sensitive information in public issues.
