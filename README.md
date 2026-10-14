# Assignment 4 — Forms and Validation

**Student:** Assem Tugelbay  
**Group:** SE-2540  
**Course:** Web Technologies I (Front End)

**Repository:** [asemtygelbaeva-byte/assignment4_frontend](https://github.com/asemtygelbaeva-byte/assignment4_frontend)

A student club website with contact and registration forms. Built with HTML, CSS and Bootstrap 5.3.8. 

## Run the project

Download the repository and open `index.html` in a browser. All five tasks are on this page; the links at the top jump to each task. CSS is included inside the HTML file. An internet connection is required for the Bootstrap stylesheet.

## Part 1 — Basic HTML Forms

### Task 0 — Simple Contact Form

The first form in `index.html` has Name, Email, Message and Submit. Each input has a matching label.

![Task 0 — basic contact form](https://github.com/user-attachments/assets/f2490942-2517-49e7-a766-52e05d582813)

### Task 1 — Form with HTML5 Validation

The second form adds `required`, `minlength` and `maxlength`. Name accepts 2–30 characters, Message accepts 10–500, and `type="email"` checks the email format. Empty fields and incorrect email addresses prevent submission.

![Task 1 — invalid email and browser feedback](https://github.com/user-attachments/assets/6a9c9c35-e23b-46a3-aa18-5b4e35f4d9ca)

## Part 2 — Bootstrap Forms

### Task 2 — Bootstrap Form Styling

The Bootstrap contact form uses `form-label`, `form-control`, `form-text` and `btn`. The `row g-3` grid provides spacing. Name and Email use `col-md-6` to appear side by side on larger screens and stack on mobile. The fields include placeholders and an email hint.

![Task 2 — valid Bootstrap contact form](https://github.com/user-attachments/assets/78fe1aac-1f09-4cf7-b485-c951f7642089)

### Task 3 — Bootstrap Validation Styles

The contact form uses `was-validated`, `valid-feedback` and `invalid-feedback`. Messages and borders change as valid or invalid values are entered. Empty required fields show errors from page load.

The two read-only fields below the form demonstrate `is-valid` and `is-invalid`. These examples have fixed styles; the contact form above is used to test changing input values.

![Task 3 — is-valid and is-invalid examples](https://github.com/user-attachments/assets/e0478967-49a9-470b-a86d-8e66d3f32d30)

## Part 3 — Advanced Form Project

### Task 4 — Registration Form

`index.html` includes First Name, Last Name, Email, Password, Confirm Password, Gender radio buttons, Hobbies checkboxes, Country dropdown, Submit and Reset. Only one gender option can be selected; multiple hobbies can be selected.

Names require 2–30 characters and passwords require 8–30. Email, gender and country are required; hobbies are optional. Bootstrap Grid adjusts the layout to the screen width. Feedback appears below the inputs.

![Task 4 — required fields and blocked submission](https://github.com/user-attachments/assets/e803ea39-496e-49cd-80ec-b288ef499253)

![Task 4 — valid registration fields](https://github.com/user-attachments/assets/20cdfefc-570c-4f22-b37d-03f55b00df03)

![Task 4 — mobile layout at 375px](https://github.com/user-attachments/assets/76515437-2b26-4209-8d16-9093490dcb6c)

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

All tasks are collected in one HTML file with internal CSS. The contact form was built first, then HTML validation was added. Next came the Bootstrap layout, feedback messages and registration form. Empty fields, incorrect and valid input, Reset, and mobile layouts were checked in a browser. Screenshots show the results for each task.

## Resources

- [Bootstrap form overview](https://getbootstrap.com/docs/5.3/forms/overview/)
- [Bootstrap validation](https://getbootstrap.com/docs/5.3/forms/validation/)
- [Bootstrap Grid](https://getbootstrap.com/docs/5.3/layout/grid/)
- [HTML form attributes](https://www.w3schools.com/html/html_form_attributes.asp)
- Course assignment brief and syllabus, supplied by the instructor.
