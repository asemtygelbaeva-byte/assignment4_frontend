# Assignment 4 — Forms and Validation

**Student:** Assem Tugelbay  
**Group:** SE-2540  
**Course:** Web Technologies I (Front End)

**Website:** [Open the Student Club website](https://asemtygelbaeva-byte.github.io/assignment4_frontend/)

A student club website with contact and registration forms. Built with HTML, CSS and Bootstrap 5.3.8. 

The design uses a warm background, dark green buttons, serif headings and rounded form cards. The first two forms use a two-column CSS Grid on desktop and stack on mobile.

## Run the project

Open the website using the link above, or download `index.html` and open it in a browser. All five tasks are on this page; the links at the top jump to each task. CSS is included inside the HTML file. Colours, fonts, sizes and spacing are controlled by CSS variables in `:root`. An internet connection is required for the Bootstrap stylesheet.

## Part 1 — Basic HTML Forms

### Task 0 — Simple Contact Form

The first form in `index.html` has Name, Email, Message and Submit. Each input has a matching label.

![Task 0 — basic contact form](https://github.com/user-attachments/assets/5ac29ddd-0a1d-4487-9cba-b0421a052724)

### Task 1 — Form with HTML5 Validation

The second form adds `required`, `minlength` and `maxlength`. Name accepts 2–30 characters, Message accepts 10–500, and `type="email"` checks the email format. Empty fields and incorrect email addresses prevent submission.

![Task 1 — invalid email and browser feedback](https://github.com/user-attachments/assets/fdee7021-4ed4-464e-bf79-8d86b965e4f2)

## Part 2 — Bootstrap Forms

### Task 2 — Bootstrap Form Styling

The Bootstrap contact form uses `form-label`, `form-control`, `form-text` and `btn`. The `row g-3` grid provides spacing. Name and Email use `col-md-6` to appear side by side on larger screens and stack on mobile. The fields include placeholders and an email hint.

![Task 2 — valid Bootstrap contact form](https://github.com/user-attachments/assets/26665f9f-4fe1-44e5-80dd-c0c31927339a)

### Task 3 — Bootstrap Validation Styles

The contact form uses `was-validated`, `valid-feedback` and `invalid-feedback`. Messages and borders change as valid or invalid values are entered. Empty required fields show errors from page load.

The two read-only fields below the form demonstrate `is-valid` and `is-invalid`. These examples have fixed styles; the contact form above is used to test changing input values.

![Task 3 — is-valid and is-invalid examples](https://github.com/user-attachments/assets/35f4bcca-5444-4518-9ebf-312d587d523b)

## Part 3 — Advanced Form Project

### Task 4 — Registration Form

`index.html` includes First Name, Last Name, Email, Password, Confirm Password, Gender radio buttons, Hobbies checkboxes, Country dropdown, Submit and Reset. Only one gender option can be selected; multiple hobbies can be selected.

Names require 2–30 characters and passwords require 8–30. Email, gender and country are required; hobbies are optional. Bootstrap Grid adjusts the layout to the screen width. Feedback appears below the inputs.

![Task 4 — required fields and blocked submission](https://github.com/user-attachments/assets/bca695de-0fbf-4db0-a194-26c52dc8bd4c)

![Task 4 — valid registration fields](https://github.com/user-attachments/assets/7c139d88-6a56-40c0-b3d4-584da373690b)

![Task 4 — mobile layout at 375px](https://github.com/user-attachments/assets/d27c3e16-96c3-4603-9960-cd64b852902d)

## Notes

- Password fields are checked for length, but their values are not compared.
- Submit reloads the same page at the corresponding task; the form does not create an account or send email. Passwords are excluded from the submission URL.
- Reset clears the registration form. Empty required fields then show error feedback again.

## Test results

| Check | Observed result |
| --- | --- |
| Empty required fields | Browser blocks submission and focuses the first invalid field |
| Email `student` | Rejected; corrected `student@example.com` is accepted |
| Five-character message | Rejected by the 10-character minimum when typed |
| Three-character password | Rejected by the 8-character minimum when typed |
| Valid contact and registration fields | Feedback turns green; Submit reloads the page at the same task |
| Reset | Text inputs, country, radios and checkboxes return to their initial values |
| Registration submission URL | Passwords are absent |
| Mobile widths 320px and 375px | No horizontal overflow; columns stack |

## Work process summary

All tasks are collected in one HTML file with internal CSS. The contact form was built first, then HTML validation was added. Next came the Bootstrap layout, feedback messages and registration form. Colours, fonts, spacing and responsive cards were styled with CSS. Empty fields, incorrect and valid input, Reset, and mobile layouts were checked in a browser. Screenshots show the results for each task.

## Resources

- [Bootstrap form overview](https://getbootstrap.com/docs/5.3/forms/overview/)
- [Bootstrap validation](https://getbootstrap.com/docs/5.3/forms/validation/)
- [Bootstrap Grid](https://getbootstrap.com/docs/5.3/layout/grid/)
- [HTML form attributes](https://www.w3schools.com/html/html_form_attributes.asp)
- Course assignment brief and syllabus, supplied by the instructor.
