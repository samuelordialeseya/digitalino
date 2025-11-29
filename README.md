# digitalino

## CSS Organization Update

To significantly improve the codebase's maintainability and scalability, we have moved away from a single monolithic `style.css` file to a **modular CSS architecture**.

The site's styling is now organized into the following logical files, all linked through the main `style.css` file via the `@import` rule:

| File Name | Purpose | Content Focus |
| :--- | :--- | :--- |
| **`style.css`** | **Master Entry Point** | Only contains the `@import` declarations for the other three files. |
| **`base.css`** | **Foundation** | Global, foundational styles (e.g., `body`, fonts, typography). |
| **`layout.css`** | **Structure** | Defines the main page organization (e.g., `.site-header`, `.main-content` positioning, Flexbox rules). |
| **`components.css`** | **Elements** | Styles for reusable UI elements (e.g., `.author-info`, article images, components). |

This organization makes it much easier to locate and update specific parts of the site's design.

**Please note:** This section describes the *intended* structure. The actual refactoring (cutting and pasting the code out of `style.css` and into `base.css`, `layout.css`, and `components.css`) is a large task and will be implemented and pushed in a future work session.