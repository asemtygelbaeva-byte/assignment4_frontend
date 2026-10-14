# Assignment 4 — Forms and Validation

**Student:** Assem Tugelbay  
**Group:** SE-2540  
**Course:** Web Technologies I (Front End)

**Repository:** [asemtygelbaeva-byte/assignment4_frontend](https://github.com/asemtygelbaeva-byte/assignment4_frontend)

A student club website with contact and registration forms. Built with HTML, CSS and Bootstrap 5.3.8. No JavaScript is used.

## Run the project

Download the repository and open `index.html` in a browser. Use the three navigation links to visit every part. An internet connection is required for the Bootstrap stylesheet. The basic HTML page uses only the local stylesheet.

| File | Purpose |
| --- | --- |
| `basic.html` | Part 1: Tasks 0 and 1 |
| `bootstrap.html` | Part 2: Tasks 2 and 3 |
| `index.html` | Part 3: Task 4 |
| `styles.css` | Shared appearance and basic form styling |
| `complete.html` | Destination after a permitted form submission |
| `screenshots/` | Screenshots for every task |

## Part 1 — Basic HTML Forms

### Task 0 — Simple Contact Form

The first form in `basic.html` has Name, Email, Message and Submit. Each input has a matching label.

![Task 0 — basic contact form](screenshots/task-0-basic.jpg)

### Task 1 — Form with HTML5 Validation

The second form adds `required`, `minlength` and `maxlength`. Name accepts 2–30 characters, Message accepts 10–500, and `type="email"` checks the email format. Empty fields and incorrect email addresses prevent submission.

![Task 1 — invalid email and browser feedback](screenshots/task-1-validation.jpg)

## Part 2 — Bootstrap Forms

### Task 2 — Bootstrap Form Styling

`bootstrap.html` uses `form-label`, `form-control`, `form-text` and `btn`. The `row g-3` grid provides spacing. Name and Email use `col-md-6` to appear side by side on larger screens and stack on mobile. The fields include placeholders and an email hint.

![Task 2 — valid Bootstrap contact form](screenshots/task-2-bootstrap.jpg)

### Task 3 — Bootstrap Validation Styles

The contact form uses `was-validated`, `valid-feedback` and `invalid-feedback`. Messages and borders change as valid or invalid values are entered. Empty required fields show errors from page load.

The two read-only fields below the form demonstrate `is-valid` and `is-invalid`. These examples have fixed styles; the contact form above is used to test changing input values.

![Task 3 — invalid input and the two explicit validation classes](screenshots/task-3-feedback.jpg)

## Part 3 — Advanced Form Project

### Task 4 — Registration Form

`index.html` includes First Name, Last Name, Email, Password, Confirm Password, Gender radio buttons, Hobbies checkboxes, Country dropdown, Submit and Reset. Only one gender option can be selected; multiple hobbies can be selected.

Names require 2–30 characters and passwords require 8–30. Email, gender and country are required; hobbies are optional. Bootstrap Grid adjusts the layout to the screen width. Feedback appears below the inputs.

![Task 4 — required fields and blocked submission](screenshots/task-4-invalid.jpg)

![Task 4 — valid registration fields](screenshots/task-4-valid.jpg)

![Task 4 — mobile layout at 375px](screenshots/task-4-mobile.jpg)

## Notes

- Password fields are checked for length, but their values are not compared.
- Submit opens `complete.html`; the form does not create an account or send email. Passwords are excluded from the submission URL.
- Reset clears the registration form. Empty required fields then show error feedback again.

## Test results

| Check | Observed result |
| --- | --- |
| Empty required fields | Browser blocks submission and focuses the first invalid field |
| Email `student` | Rejected; corrected `student@example.com` is accepted |
| Five-character message | Rejected by the 10-character minimum when typed |
| Three-character password | Rejected by the 8-character minimum when typed |
| Valid contact and registration fields | Feedback turns green; Submit opens the demo completion page |
| Reset | Text inputs, country, radios and checkboxes return to their initial values |
| Registration submission URL | Passwords are absent |
| Mobile widths 320px and 375px | No horizontal overflow; columns stack |

## Work process summary

The contact form was built first, then HTML validation was added. Next came the Bootstrap layout, feedback messages and registration form. Empty fields, incorrect and valid input, Reset, and mobile layouts were checked in a browser. Screenshots show the results for each task.

## Resources

- [Bootstrap form overview](https://getbootstrap.com/docs/5.3/forms/overview/)
- [Bootstrap validation](https://getbootstrap.com/docs/5.3/forms/validation/)
- [Bootstrap Grid](https://getbootstrap.com/docs/5.3/layout/grid/)
- [HTML form attributes](https://www.w3schools.com/html/html_form_attributes.asp)
- Course assignment brief and syllabus, supplied by the instructor.
