# AngularJS Research - Group E

## References
- [What is AngularJS?](#what-is-angularjs)
- [MVC Architecture](#mvc-architecture)
- [AngularJS Directives](#angularjs-directives)
- [Dependency Injection](#dependency-injection)
- [Routing](#routing)
- [Angular Expressions](#angular-expressions)
- [Angular DOM Directive](#angular-dom-directive)
- [Angular Form Validation](#angular-form-validation)
- [Data Binding](#data-binding)
- [Ternary Operator in Angular](#ternary-operator-in-angular)
- [Angular Integration with Backend](#angular-integration-with-backend)
- [Angular Pros](#angular-pros)
- [Angular Cons](#angular-cons)
- [Companies Using AngularJS](#companies-using-angularjs)
- [Popularity of AngularJS](#popularity-of-angularjs)

---

## Presentation of Angular

![What is AngularJS](images/slide1.jpg)

## What is AngularJS?

![What is AngularJS](images/slide2.jpg)
AngularJS is a popular framework developed by Google, designed to create dynamic, single-page applications (SPAs). It’s open-source, which means it’s free to use and continuously updated by the community. AngularJS allows developers to build applications that load a single HTML page and update the content dynamically as users interact, without reloading the whole page. This makes the user experience faster and more seamless.

One of the key features is that AngularJS is component-based, meaning that the application is divided into reusable components, making development more organized and maintainable. Another important aspect is that AngularJS uses TypeScript, a superset of JavaScript that enhances the language with features like type checking, which leads to fewer bugs and more robust applications.

AngularJS is not just for small projects—it’s enterprise-level, used by large-scale applications for its scalability and high performance.

## MVC Architecture

![MVC Architecture](images/slide3.jpg)
Angular uses the Model-View-Controller (MVC) architecture to organize and separate different parts of an application, making it more structured and easier to maintain.

- **Model**: This represents the data and business logic. In Angular, services handle the model by retrieving and managing data, often using APIs to communicate with a backend.
- **View**: The user interface, defined by HTML templates and styled with CSS. The view interacts with the model through two-way data binding, allowing for real-time dynamic updates in the UI whenever the underlying data changes.
- **Controller**: In Angular, the controller role is managed by components. These components handle user interactions, update the model or the view accordingly, and control how data flows between the two.

## AngularJS Directives

![AngularJS Directives](images/slide4.jpg)
Angular has three main types of directives:

- **Component Directives**: Custom elements that define a section of the user interface (UI). They use templates, styles, and logic to create reusable views (e.g., `<app-header></app-header>`).
- **Structural Directives**: These modify the structure of the DOM by adding or removing elements (e.g., `*ngIf`, `*ngFor`).
- **Attribute Directives**: These modify the behavior or appearance of an existing element without altering the DOM structure (e.g., `ngClass`, `ngStyle`).

## Dependency Injection

![Dependency Injection](images/slide5.jpg)
In Angular, Dependency Injection (DI) is a design pattern that provides components with their required dependencies, such as services, instead of having the components create these dependencies themselves. This approach enhances the modularity, testability, and maintainability of the code.

When a component or service requires a dependency, Angular's DI system automatically finds the needed instance in the injector and provides it. This makes the process of managing dependencies easier and reduces code duplication across the application.

## Routing

![Routing](images/slide6.jpg)
In Angular, routing enables navigation between different pages or views in a single-page application (SPA) without reloading the entire page.

- **Route Configuration**: The `$routeProvider` is used to define different routes within the application.
  - `/ (Home route)`: This is the default route, which loads the `home.htm` template when the URL is `/`.
  - `/registration`: This route loads the `registration.htm` template when the URL is `/registration`.
  - `/login`: This route loads the `login.htm` template when the URL is `/login`.
- **Navigation Links**: The `<a>` elements in the HTML use `href="#/path"` to link to different routes.
  - `href="#!/"`: Navigates to the home page.
  - `href="#!/registration"`: Navigates to the registration page.
  - `href="#!/login"`: Navigates to the login page.
- **ng-view**: The `<div ng-view></div>` acts as a placeholder where the content of the routed templates (e.g., `home.htm`, `registration.htm`, `login.htm`) will be dynamically loaded based on the current route the user navigates to.

This setup allows AngularJS to load different templates dynamically, ensuring that the page does not reload while switching between views, providing a smooth user experience in SPAs.

## Angular Expressions

![Angular Expressions](images/slide7.jpg)
Angular expressions are used to bind dynamic data from the component to the view. They allow you to display variables, perform simple calculations, or manipulate data directly within the HTML. Unlike JavaScript, Angular expressions are designed to be simple, without supporting loops or conditionals, and they don’t produce side effects. Their primary role is to make the view responsive by dynamically rendering data and values from the component in a lightweight and efficient way.

## Angular DOM Directive

![Angular DOM Directive](images/slide8.jpg)
The `ng-show` directive in AngularJS is used to conditionally display or hide an element based on a boolean expression. When the expression evaluates to `true`, the element is visible, and when it is `false`, the element is hidden but still remains in the DOM.

## Angular Form Validation

![Angular Form Validation](images/slide9.jpg)
In AngularJS, form validation is automatically handled when input fields are given specific types, such as "email". The validity of the input is tracked using the built-in `$valid` property. When an invalid email (like "kaszapnagyp") is entered, AngularJS marks the input as invalid, and `$valid` becomes `false`. When a valid email (like "szapnagyp@gmail.com") is entered, the `$valid` property becomes `true`, indicating the input is correct.

## Data Binding

![Data Binding](images/slide10.jpg)
Data binding in AngularJS can occur in two ways:

- **One-way data binding**: Data flows in a single direction, either from the component (model) to the view or from the view to the component. It requires an event to trigger data flow.
- **Two-way data binding**: Data flows in both directions. Changes in the view (e.g., typing in an input field) are automatically reflected in the component, and changes in the component are reflected in the view.

## Ternary Operator in Angular

![Ternary Operator in Angular](images/slide11.jpg)
The ternary operator in AngularJS allows conditional rendering based on a true/false condition. For example, checking if a user is logged in (`isLoggedIn`). If true, a welcome message like "Welcome, Peter Kaszap-Nagy!" is displayed along with a "Logout" button; if false, the user is prompted to log in.

## Angular Integration with Backend

![Angular Integration with Backend](images/slide12.jpg)
Angular integrates with the backend using HTTP requests to retrieve or send data. Angular uses the `$http` service to send a GET request to a server endpoint, and the data returned from the server is stored and displayed in the view.

## Angular Pros

![Angular Pros](images/slide13.jpg)
- **Two-Way Data Binding**: Simplifies the synchronization between the model and the view, reducing boilerplate code.
- **MVC Architecture**: Separates concerns, making the application more organized and maintainable.
- **Directives**: Enable the creation of reusable components and extend HTML's functionality.
- **Dependency Injection**: Facilitates better modularity and easier testing by managing dependencies efficiently.
- **Community and Support**: Angular has extensive documentation, tutorials, and a large community for support and resources.
- **Integration Capabilities**: Easily integrates with other libraries and frameworks.

## Angular Cons

![Angular Cons](images/slide14.jpg)
- **Performance Issues**: Two-way data binding can lead to performance bottlenecks in large applications.
- **Steep Learning Curve**: Concepts like directives and dependency injection can be challenging for beginners.
- **Deprecated Features**: AngularJS (1.x) is considered legacy, with official support ending in December 2021.
- **SEO Challenges**: Single-page applications can face search engine optimization issues.
- **Verbosity**: Writing AngularJS code can be more verbose, leading to increased development time.
- **Limited Mobile Support**: AngularJS is not inherently optimized for mobile development.

## Companies Using AngularJS

![Companies Using AngularJS](images/slide15.jpg)
Major companies like Google, Microsoft, PayPal, Upwork, Forbes, IBM, and The Guardian use AngularJS for building their applications due to its flexibility and scalability.

## Popularity of AngularJS

![Popularity of AngularJS](images/slide16.jpg)
According to Stack Overflow's data from 2023, AngularJS remains one of the most popular frameworks despite the emergence of newer technologies like React and Vue.js. AngularJS continues to maintain a strong presence in the developer community.

## Thank You

![Thank You](images/slide17.jpg)
Group E Presentation: 
- Aaron McAvoy
- Douglas McGregor
- Peter Kaszap-Nagy
- Balint Kaszap-Nagy

---

## External References
- [AngularJS Official Website](https://angularjs.org/)
- [AngularJS API Documentation](https://docs.angularjs.org/api)
- [W3Schools AngularJS Guide](https://www.w3schools.com/angular/)
- [TutorialsPoint AngularJS](https://www.tutorialspoint.com/angularjs/index.htm)
- [Codecademy Learn AngularJS](https://www.codecademy.com/learn/learn-angularjs)
