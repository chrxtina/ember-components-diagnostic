# Ember Components Diagnostic

Record your responses inside the fenced code blocks below each question.

1.  Give an example of a visual hierarchy that could be modeled with components. Explain why each piece might be it's own component.

    ```md
    A messaging system between users. The first layer would be a conversation.
    Then, a component inside of a conversation would be an individual message.
    A message would be its own component bc when a conversation iterates through
    its array of messages, each message would use a message template and actions
    for each message would be bubbled up through its respective component.js.
    ```

1.  What is the command to generate a new component called '`my-map`'?

    ```sh
    ember g component my-map
    ```

1.  What files are created and/or edited to produce a component, and what are their responsibilities?

    ```md
    A component.js file and a template.hbs file for that component. The component.js
    file is responsible for bubbling actions up like classNameBindings or delete and update actions. The template.hbs file holds the information that will be displayed in the view.
    ```

1.  Suppose you have a component '`my-contact`', which is loaded from
    '`app/contacts/template.hbs`' when visiting the `/contacts` route. What is
    the syntax (code that is written) to render this component inside that template?

    ```html
    {{contact/my-contact my-contact=my-contact}}
    ```

1.  Each contact has multiple phone numbers. Suppose you also have '`my-phone`'
    nested under '`my-contact`'. What is the code you would write in
    '`app/components/my-contact/template.hbs`' to load the nested component and
    pass it data?

    ```html
    {{my-contact/my-phone my-phone=my-phone}}
    ```
