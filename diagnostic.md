# Ember Components Diagnostic

Record your responses inside the fenced code blocks below each question.

1.  Give an example of a visual hierarchy that could be modeled with components. Explain why each piece might be it's own component.

    ```md
    
    Main content -> Sidebar with list of emails & primary section with content of single email

    The sidebar and the single email view could each be a component. Each email within the sidebar list might also be a component.

    Components are good for reusable elements on the page.

    ```

1.  What is the command to generate a new component called '`my-map`'?

    ```sh
    ember g component my-map

    ```

1.  What files are created and/or edited to produce a component, and what are their responsibilities?

    ```md
    
    The component consists of a directory containing a template (for display) and a component.js file that handles properties and actions of the component.

    ```

1.  Suppose you have a component '`my-contact`', which is loaded from
    '`app/contacts/template.hbs`' when visiting the `/contacts` route. What is
    the syntax (code that is written) to render this component inside that template?

    ```html
    
    {{my-contact contact=contact}}


    ```

1.  Each contact has multiple phone numbers. Suppose you also have '`my-phone`'
    nested under '`my-contact`'. What is the code you would write in
    '`app/components/my-contact/template.hbs`' to load the nested component and
    pass it data?

    ```html
    {{my-phone number=number}}
    
    ```
