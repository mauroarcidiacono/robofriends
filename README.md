# Robofriends

This is my first React.js project. I built it by following Andrei Neagoie teachings in the Zero To Mastery Academy. React stablishes a component focused style of development that creates a network, reducing dependencies. The library has a one way data-flow, where the direction of the data is always downstream and only the child react to changes of the parent. React describes the current state of the website with a copy of the DOM which is stored in a JavaScript object.  

Following the [documentation](https://reactjs.org/docs/create-a-new-react-app.html), I started the React application by typing:

    npx create-react-app my-app
    cd my-app
    npm start
    
The project has four components: Card, CardList, Scroll and SearchBox. App is the container that is imported in index and rendered. 

The robots are sourced from https://robohash.org/ and the names and emails are fetched from https://jsonplaceholder.typicode.com/users when componentDidMount() is run. 

The class app defines a robots array and a searchfield variable. The SearchBox component receives a searchChange argument that sets the state of searchfield to the string that is written in the search box of the app. Then, as an event is triggered because something was typed in the input box, render runs again but this time a filter acts by applying the includes() method. This is passed as filteredRobots to the CardList component and now only the cards that were not filtered can be seen. 

The Scroll component wraps the CardList component and applies a style to the children, which are the cards.

Try the app and find your robofriend by typing its name! 
