### IONIC
- What is Ionic?

    Ionic is Open Source frameworks for building cross platform application using HTML,CSS,JavaScript, Angular, React or Vue.

- What is Standalone?
    
    1. In Angular , a stnadalone components is a new featur(Introduce in Angular 14) that allows you create components without putting them into a module.
    2. Components does not need to part of NgModule
    3. I can import it directly where I want to use.
    4. It's self-contained and manages it's own dependencies.

    ```ts
    //Tradational Way before v14
    @NgModule({
        declarations:[MyComponents]
    })
    export class MyModule{}
    ```

    ```ts
    //Standalone Way
    @Components({
        selector:'app-my',
        standalone: true,
        template:`<p>Hello</p>`
    })
    exports class MyComponent {}
    ```


- ionic start modern-app blank --type angular
    
    This command tells IONIC CLI to create new project.Let's break it one by one and understand.
    
    🧩 ionic start 
    -
    This is the basic command to create a new Ionic app.

    🧩 modern-app
    -
    This is the name of your app.

    🧩 blank
    -
    This is the template you're using.IONIC give template options like, 

        1. blank: a minimal app with just a single page
        2. tabs: a tabbed interface
        3. sidemenu: side navigation menu
     🧩 --type angular
     -
     This tells Ionic to use Angular as the frontend framework. You could also choose:

    --type=react

    --type=vue

    - Generate Components
        ```bash
        ionic generate component components/product-card
        ```



- What is Services?

    A service is typescript class that provides reusable buisness logic,data,or functinality to components in app.


- Forms
    
    Two types of Forms are there for form handling, Template form and Reactive form.
    - Reactive Form:
        -  The validations and other form controls are written in the component class.
        - It offers more flexibility as it is easier to integrate with the backend services.
        - Reactive forms provide the features of dynamically add or remove form controls.
        - Since, we have more programmatically code in our component class. So, we can have more custom validation functions to provide validations in the angular form state.

    - Template Form:
        - Template Driven Forms is the most simplest way through which we can build a form in Angular.
        - The logic related to form is present in the template itself. So there is less or no requirement to write logic related to form in the component file. So it is less complicated and easy to understand.
        

 
    - Standalone Vs ngModule
    
