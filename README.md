# Instruction

## How to open "md" (markdown) files.

Use your preferable Text Editor (f.e. VSCode or Atom). Open a required file there. Now open "Preview mode" (Ctrl + Shift + V on Win VSCode). The same you can do in your preferable IDE using a Markdown preview plugin.

An alternative way. Open https://dillinger.io/ and copy-paste a required text there.

## Story

Abibos team worked hard to meat a deadline, but suddenly one of their Frontend developers have got terrible cough and lay down. The situation is terrible.

You are a Frontend Developer. You worked on another project but your Functional Manager asked you to help Abibos team with their task. You need to catch up on-going project and finish Product Details Page.

Save the day!

## Description

Please, create markup and styles for components according requirements. Implement JavaScript functionality according requirements. Requirements are incomplete, you're free to implement your ideas.

Links to Design

- [Mobile Design](https://bitbucket.org/ast_amerezhanyi/ast_test_task/raw/2d0cbe6d076be0a5675e8bec6b99db6a3c54f4b1/Design_mobile.png)
- [Tablet Design](https://bitbucket.org/ast_amerezhanyi/ast_test_task/raw/2d0cbe6d076be0a5675e8bec6b99db6a3c54f4b1/Design_tablet.png)
- [Desktop Design](https://bitbucket.org/ast_amerezhanyi/ast_test_task/raw/2d0cbe6d076be0a5675e8bec6b99db6a3c54f4b1/Design_desktop.png)

## Functional Requirements

1.  Product image

    ![](https://bitbucket.org/ast_amerezhanyi/ast_test_task/raw/7e87788e6acd3aff08d7f145bfb61555c15e70aa/product-image.png)

    1.  Fetch data https://bitbucket.org/ast_amerezhanyi/ast_test_task/raw/c9e0d3ec2d9c4dc6d8e131f927277d15526f6ac4/products.json
    1.  Display first "image" in "color" array: `[item].color[0].image`
    1.  Image size: Desktop `398x398`, Tablet `362x362`, Mobile width `100%`

1.  Product title

    ![](https://bitbucket.org/ast_amerezhanyi/ast_test_task/raw/7e87788e6acd3aff08d7f145bfb61555c15e70aa/product-title.png)

    1.  Fetch data https://bitbucket.org/ast_amerezhanyi/ast_test_task/raw/c9e0d3ec2d9c4dc6d8e131f927277d15526f6ac4/products.json
    1.  Apply new title for each product: `[item].title`
    1.  Styles Desktop:
        - Font: 24px, "Oswald", uppercase
        - Letter spacing: 0.05em
        - color: #2c303d
        - Use Design for the rest
    1.  Styles Tablet:
        - Margin bottom: 30px
        - Use Design for the rest
    1.  Styles Mobile:
        - Margin bottom: 24px
        - Letter spacing: 0.03em
        - Line height: 1.55
        - Use Design for the rest

1.  Product Price

    ![](https://bitbucket.org/ast_amerezhanyi/ast_test_task/raw/7e87788e6acd3aff08d7f145bfb61555c15e70aa/product-price.png)

    1.  Fetch data https://bitbucket.org/ast_amerezhanyi/ast_test_task/raw/c9e0d3ec2d9c4dc6d8e131f927277d15526f6ac4/products.json
    1.  Apply new price (new and old) for each product: `[item].price`, `[item].old_price`
    1.  In case "old price" is not provided use "price" only
    1.  Styles Desktop:
        - Font: 24px, "Open Sans"
        - Old Price color: #2c303d
        - Price color: #ce2c52
        - Use Design for the rest
    1.  Styles Tablet:
        - Font: 36px, "Open Sans"
        - Use Design for the rest
    1.  Styles Mobile:
        - Font: 36px, "Open Sans"
        - Use Design for the rest

1.  Product description

    ![](https://bitbucket.org/ast_amerezhanyi/ast_test_task/raw/7e87788e6acd3aff08d7f145bfb61555c15e70aa/product-description.png)

    1.  Fetch data https://bitbucket.org/ast_amerezhanyi/ast_test_task/raw/c9e0d3ec2d9c4dc6d8e131f927277d15526f6ac4/products.json
    1.  Apply product description for each product: `[item].details`
    1.  Styles Desktop:
        - Font: 12px, 300, "Open Sans"
        - Letter spacing: 0.03em
        - Line height: 1.4
        - Use Design for the rest
    1.  Styles Mobile:
        - Font: 14px, "Open Sans"
        - Letter spacing: 0.04em
        - Line height: 1.45
        - Use Design for the rest

1.  Product variations

    ![](https://bitbucket.org/ast_amerezhanyi/ast_test_task/raw/7e87788e6acd3aff08d7f145bfb61555c15e70aa/product-variations.png)

    1.  Fetch data https://bitbucket.org/ast_amerezhanyi/ast_test_task/raw/c9e0d3ec2d9c4dc6d8e131f927277d15526f6ac4/products.json
    1.  Apply background color accordingly: `[item].color[variation].color`
    1.  On change variation change "title" accordingly: `[item].color[variation].title`
    1.  On change variation change "image" accordingly: `[item].color[variation].image`
    1.  On change variation change "SKU" (Item #) accordingly: `[item].color[variation].sku`

1.  Comments section

    ![](https://bitbucket.org/ast_amerezhanyi/ast_test_task/raw/7e87788e6acd3aff08d7f145bfb61555c15e70aa/comments.png)

    1.  Fetch data https://bitbucket.org/ast_amerezhanyi/ast_test_task/raw/4724958b5a63f0d8634b7ce57b69514575513cb2/comments.json
    1.  Show "Loading..." in the section while data are loading
    1.  Display only 3 top comments
    1.  If there is an error during fetching display "No comments"
    1.  Styles Desktop:
        - Font: 12px, 300, "Open Sans"
        - Letter spacing: 0.03em
        - Line height: 1.4
        - Use Design for the rest
    1.  Styles Mobile:
        - Font: 14px, "Open Sans"
        - Letter spacing: 0.04em
        - Line height: 1.45
        - Use Design for the rest

1.  Change product

    ![](https://bitbucket.org/ast_amerezhanyi/ast_test_task/raw/7e87788e6acd3aff08d7f145bfb61555c15e70aa/change-product.png)

    1.  Implement product сhange (image, title, SKU, price, description, size, color variation) on click on the image from "You may also like" section.
    1.  Use an associated "data" attribute: `<a href="#" data-sku="701642853690">` -> `{ "701642853690": { ... }, ... }`
    1.  Fetch data https://bitbucket.org/ast_amerezhanyi/ast_test_task/raw/c9e0d3ec2d9c4dc6d8e131f927277d15526f6ac4/products.json

## Non-functional Requirements

1.  In case of SASS/SCSS usage add your build scripts (grunt/gulp/webpack) to the project
1.  Your final solution must be testable via local server or local build
1.  Add all required/used packages to the project `package.json`
1.  The task was estimated for 4 hours and due date in 2 days
1.  Use BEM western notation class naming (even you're not like it). Previous developer haven't used it.
1.  Specification is incomplete, use Design. Whether Specification contradicts Design use Specification.
1.  Address all eslint issues.

## Other Requirements

1.  Consider fetching data in a parallel
1.  Do not trust user's data, prevent hijacking and script injections
1.  Consider Unit Testing implementation for your code
1.  Previous developer used jQuery, you can use it or provide Vanilla JS code (ES5 or ES6+ syntax)
1.  Put your attention to semantics (tags' usage)
1.  Consider UX best practices (spinners while loading, consistent size, etc.)
1.  Pay attention to possible JS exceptions and wrap unsafe code.
