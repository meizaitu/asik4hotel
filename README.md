# Aurora Hotel

## Project Overview

Aurora Hotel is a responsive hotel website developed with HTML5, CSS3, Bootstrap 5 and JavaScript. This part of the project focuses on two forms: **Contact Us** and **Guest Registration**. Both forms check user input and display clear feedback.

## Team Members

| Member                  |                                 Contribution                                    |
|                         |                                                                                 |
| Meizamkhan Zhanbyrbayev | Developed the Contact Us form and implemented HTML5 validation.                 |
| Dilnaz Toktanova        | Designed responsive layouts using Bootstrap and added validation feedback.      |
| Ayazhan Nurtaza         | Developed the Registration form and implemented JavaScript password validation. |
| Meizamkhan Zhanbyrbayev | Tested the website, checked form functionality, and prepared documentation.     |


## How to Run

1. Download and extract the project ZIP file.
2. Open **`index.html`** in a web browser.
3. Go to **Contact Us** (`contact.html`) to test the contact form.
4. Go to **Register** (`register.html`) to test the registration form.

Keep the `css/`, `js/`, `images/` and `vendor/` folders in the same project directory as the HTML files so the website loads correctly. No server or database is required for these forms.

## Implemented Features

### Contact Form (Tasks 0–2)

The Contact Us page contains Name, Email and Message fields with a Submit button. Each input has a connected label, a unique ID and a meaningful name attribute.

Validation rules:

- **Name:** required; at least 2 characters.
- **Email:** required; valid email format.
- **Message:** required; between 10 and 500 characters.

The form uses HTML5 validation attributes and Bootstrap classes such as `form-label`, `form-control`, `invalid-feedback` and `valid-feedback`. JavaScript applies the `was-validated` class after submission so that feedback reflects the actual input.

### Registration Form (Task 3)

The Guest Registration page includes:

- First and Last Name (required; minimum 2 characters each)
- Email (required; valid format)
- Password and Confirm Password (required; minimum 8 characters)
- Gender radio buttons, including **Prefer not to say** (optional)
- Interests checkboxes (optional)
- Country dropdown (required; blank default option)
- Submit and Reset buttons

JavaScript checks whether the passwords match and clears the mismatch error when corrected. Invalid data blocks submission. The Reset button clears entered values and validation feedback.

Successful submission only displays a confirmation in the browser. It does **not** send data to a server or create a real account.

## Validation Tests (Task 4)

The table below summarizes the test results recorded for the supplied Part 1 project. Recheck them if you modify the website before submission.

| Test case | Test input | Expected result | Recorded result |
|---|---|---|---|
| Empty contact form | All required fields blank | Submission blocked; errors displayed | Pass |
| Invalid email | `wrong-email` | Email marked invalid | Pass |
| Short message | `short` | Message rejected (under 10 characters) | Pass |
| Valid contact form | Name, valid email and 10–500 character message | Success confirmation displayed | Pass |
| Short password | `1234567` | Registration blocked | Pass |
| Password mismatch | `password123` and `password456` | Mismatch error displayed | Pass |
| No country | Default empty option | Registration blocked | Pass |
| Valid registration | All required inputs valid; matching passwords | Success confirmation displayed | Pass |
| Reset after errors | Trigger validation, then click Reset | Fields and feedback cleared | Pass |
| Mobile layout | 375 px wide viewport | Layout fits without horizontal scrolling | Pass |
| Desktop layout | 1440 px wide viewport | Responsive desktop layout displayed | Pass |

## Screenshots

The original project includes screenshots showing the forms in valid, invalid, mobile and desktop states. Keep these files in the `screenshots/` folder when submitting your project:

| Evidence | File |
|---|---|
| Contact — invalid | `screenshots/contact-invalid-768.png` |
| Contact — valid | `screenshots/contact-valid-768.png` |
| Contact — mobile | `screenshots/contact-mobile-375.png` |
| Contact — desktop | `screenshots/contact-desktop-1440.png` |
| Registration — invalid | `screenshots/registration-invalid-768.png` |
| Registration — valid | `screenshots/registration-valid-768.png` |
| Registration — mobile | `screenshots/registration-mobile-375.png` |
| Registration — desktop | `screenshots/registration-desktop-1440.png` |

## Website Link

[Add the live website URL here]

## Conclusion

The Aurora Hotel project demonstrates responsive form layouts, HTML5 input validation, Bootstrap feedback and JavaScript password matching. Both forms provide user-friendly error messages and confirmation feedback without requiring a backend.
