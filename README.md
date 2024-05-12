HTML Template (<template>):
        It contains the structure of the login form.
        There's a title "Login" (<h2>) followed by a form element.
        Inside the form, there are input fields for username and password, along with a checkbox for "Remember Me" and a login button.
        Additionally, there's a link for "Forgot Password?".

    JavaScript Logic (<script>):
        It defines a Vue.js component.
        The data function initializes the component's data properties:
            username, password: Strings representing the values entered in the username and password input fields.
            rememberMe: Boolean representing the state of the "Remember Me" checkbox.
        The methods object contains two functions:
            login(): This function is called when the form is submitted. For now, it logs the username, password, and "Remember Me" status to the console.
            forgotPassword(): This function is called when the "Forgot Password?" link is clicked. It displays an alert message.

    CSS Styles (<style scoped>):
        The styles are scoped to the component.
        body: Sets the background image of the entire page to a Milky Way image from Pixabay. The image is centered and covers the entire background.
        .login-container: Styles the container for the login form. It has a maximum width, margin, padding, and a semi-transparent white background to improve readability against the background image.
        .form-group: Adds margin below each form group.
        label: Displays labels as blocks.
        input, button, a: Styles form elements and links with consistent padding, font size, and colors.

This code creates a simple login form with Vue.js. Users can enter their username, password, and choose whether to remember their login. The form has basic validation and styling, The "Forgot Password?" link triggers an alert message.
