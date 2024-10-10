CSS Selector 

. Tag Selector
   Selects elements by their HTML tag name.
   Example:
   cy.get('button'); // Selects all <button> elements

2. ID Selector
   Selects elements by their `id` attribute using the `#` symbol.
   Example:
   cy.get('#submit-button'); // Selects element with id="submit-button"

3. Class Selector
   Selects elements by their `class` attribute using the `.` symbol.
   Example:
   cy.get('.nav-item'); // Selects elements with class="nav-item"

4. Attribute Selector
   Selects elements based on a specific attribute and its value.
   Example:
   cy.get('input[type="text"]'); // Selects all <input> elements where type="text"

5. Child Combinator Selector (>)
   Selects direct child elements of a specified element.
   Example:
   cy.get('ul > li'); // Selects all <li> elements that are direct children of a <ul>

6. Descendant Selector (Whitespace)
   Selects all descendants of a specified element.
   Example:
   cy.get('form input'); // Selects all <input> elements inside a <form>

7. Pseudo-Class Selectors
   Used to select elements based on their state or position.
   Examples:
   cy.get('li:first-child'); // Selects the first <li> element
   cy.get('li:last-child');  // Selects the last <li> element
   cy.get('li:nth-child(3)');// Selects the third <li> element
   cy.get('input:not([type="submit"])'); // Selects all <input> elements except submit buttons
   cy.get('input[type="checkbox"]:checked'); // Selects all checked checkboxes

8. Attribute Contains Selector (*=)
   Selects elements whose attribute contains a specified value.
   Example:
   cy.get('a[href*="login"]'); // Selects all <a> elements whose href contains "login"

9. Attribute Starts With Selector (^=)
   Selects elements whose attribute starts with a specific value.
   Example:
   cy.get('input[name^="user"]'); // Selects all <input> elements whose name starts with "user"

10. Attribute Ends With Selector ($=)
    Selects elements whose attribute ends with a specific value.
    Example:
    cy.get('img[src$=".png"]'); // Selects all <img> elements whose src ends with ".png"

11. Group Selector (,)
    Selects multiple elements by grouping selectors.
    Example:
    cy.get('h1, h2, h3'); // Selects all <h1>, <h2>, and <h3> elements

12. Adjacent Sibling Selector (+)
    Selects an element that is immediately adjacent to another element.
    Example:
    cy.get('label + input'); // Selects <input> elements immediately preceded by a <label>

13. General Sibling Selector (~)
    Selects all sibling elements that follow a specified element.
    Example:
    cy.get('h2 ~ p'); // Selects all <p> elements that are siblings after an <h2>

14. Contains Text Selector
    Selects elements that contain a specific text (using Cypress's .contains()).
    Example:
    cy.contains('Submit'); // Selects elements containing the text "Submit"

15. Universal Selector (*)
    Selects all elements.
    Example:
    cy.get('*'); // Selects all elements on the page


![image](https://github.com/user-attachments/assets/e7020c84-1a59-4730-bc13-b929c0b1f730)

Xpath

Install xpath plugin
•	npm install -D cypress-xpath
Then, include the plugin in your Cypress support file:
•	require('cypress-xpath');


![image](https://github.com/user-attachments/assets/7127b99b-7162-4731-8c33-f57eb9d45431)

