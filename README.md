# React Structure

## create-react-app (CRA) or from scratch:
**CRA:**
- Pros:
    - easy to start
- Cons:
    - not very flexiable, e.g. SCSS

**From Scratch:**
- Pros:
  - easy to work with in the future
  - very flexiable and scalable
- Cons:
  - take a little bit time to configure (but there are many tutorials for getting start)  

## File Structures
[Official Recommendations](https://reactjs.org/docs/faq-structure.html)

Usually, there are following folders:
- components (only for components, no logics)
  - App.js
  - component-name-1
    - index.js
    - subcomponents for this component
    - ...
  - component-name-2
    - index.js
    - subcomponents for this component
    - ...
  - component-name-3
    - index.js
    - subcomponents for this component
    - ...
- api (only for handling api requests, no logics)
- utils (business logics for components and api)
- layouts (shared layouts by different pages)
- pages (each pages)
  - home
    - index.js
    - any componenets, layout specificly for this page
  - about
    - index.js
    - any componenets, layout specificly for this page
- images (*.png, *.jpg, etc.)
- stylesheets could be in sperated folders or go with the components as long as it's easy to access.

Useful lib: babel-plugin-module-resolver

## Other considerations
- State management: Redux vs Hooks?
- Styles: CSS, SCSS, Styled-components?
- Testing: Jest?
- CI/CD continues integration: travis, jenkins?
- Coding styles: eslint?
- is SEO important? since React renders applications on the fly.