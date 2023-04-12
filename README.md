# LAB 07 - React Router

## React Router

### Task 1 - initial setup

1. Install React Router
2. Create a browser router with 2 routes, one for the Home page at `/` and one for the Lab page at `/lab` (use the components in `src/components`)
3. in `App.js`, create navigation links that allow switching between the two pages

### Task 2 - add a loader to the Lab page

1. Write a loader in the Lab.js file, that loads todo data using the mock library in `src/data/index.js`
2. Use the loader in the route definition for the Lab page
3. Render the todo list data in the Lab component, using `<ul>` and `<li>` elements

### Task 3 - add a form to create a new todo

1. Write an action in the Lab.js file, that adds a new todo to the list (using the mock library)
2. Use the action in the route definition for the Lab page
3. Render a form in the Lab component, that triggers the action when submitted

### Task 4 - child routes and useNavigation

1. Add a new components called `Bouncer.js` and `Trigger.js` to the `src/components` folder
2. Add children routes to the Lab page, that renders the `Trigger` and an index page, and `Bouncer` under the `/bouncer/:name` path
3. Use Outlet in the Lab component to render the children
4. In the Trigger component get a random name from the mock library (`randomName()`) and render a link that navigates to the Bouncer page `bouncer/${name}`
5. In the Bouncer component, render the name from the route params
6. In the Bouncer component, use the `useNavigation` and `useEffect` hooks to navigate back to the Lab page after 2 seconds
