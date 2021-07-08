# Battle For Chicago

Battle For Chicago is a two-player board game based on Risk that uses a map of Chicago's neighborhoods as its game board.

The app provides another way for socially distanced families and friends to spend time together remotely.

[Full Demo](https://www.youtube.com/watch?v=2QhTyIyUOZg) | [Live app](https://fathomless-cove-56346.herokuapp.com/)

![Battle For Chicago demo](https://j.gifs.com/oVBZXz.gif)

I used ActionCable and Redis in Rails and ActionCable Provider for React to establish WebSocket connections between each client and the API. I wrote about deploying an app with ActionCable to Heroku [here](https://medium.com/swlh/deploying-a-rails-react-app-with-actioncable-to-heroku-cb5d42f41a2a).

I built the front end using React with Redux, Redux Thunk, and React Router. The map is an SVG image. I wrote about creating the map [here](https://medium.com/weekly-webtips/how-to-make-clickable-dynamic-graphics-in-react-using-svg-22071f96623d). I used React Bootstrap to style the UI.

I built the API using Rails with PostgreSQL and ActiveRecord.

## Installing Battle For Chicago

To install Battle For Chicago, follow these steps:

1. Clone the full contents of this repo and its submodules

```
git clone --recurse-submodules git@github.com:mpottebaum/battle-chi.git
```

2. Install gems in the back end directory:

```
cd battle-chi-backend
bundle
```

3. Install dependencies in the front end directory:

```
cd battle-chi-frontend
npm install
```

## Using Battle For Chicago

To use Battle For Chicago, follow these steps:

1. From the battle-chi-backend directory, start the API server. Make sure the API server is running on `localhost:3000`.

```
rails s
```

2. From the battle-chi-frontend directory, start the front end server.

```
npm run dev
```

The front end server should run on `localhost:3001`, but any port will work. If you open the front end in an incognito/private window or a separate browser, you can establish separate WebSocket connections and play as both players.

## Contact

If you want to contact me you can reach me at mpottebaum@gmail.com.