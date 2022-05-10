# Follow The Signs

This website is a place where people can stay informed with deaf community news, attend events, and particpate in discussions or chats amongst each other.

## Home

The home page allows for non-users to see what our website is about, and allows users to access a summarized amount of information from the other News, Events, and Discussion pages.

<p align="center">
  <img src="https://media.giphy.com/media/RSmDbAPtHXg9BOvs5B/giphy.gif" alt="HomeGIF"/>
</p>

## News

The news page displays information about things occuring in the deaf community. Each news card allows you to directly access more information about an article by taking you to it's specific site.

<p align="center">
  <img src="https://media.giphy.com/media/txIngpIXB4m8IlAp58/giphy.gif" alt="NewsGIF"/>
</p>

## Events

The events page displays experiences and gatherings which anyone can attend to build friendships within the community.

<p align="center">
  <img src="https://media.giphy.com/media/HUIvvGdpjkkCTZxoDY/giphy.gif" alt="EventsGIF"/>
</p>

## Discussions

The discussions page allows users to create or participate in discussion forums with other users and may delete their own comments if they choose to.

<p align="center">
  <img src="https://media.giphy.com/media/4juyeTI7EplDNbK0Zt/giphy.gif" alt="DiscussionsGIF"/>
</p>

## Connections

The connections page encourages users to take part in a global chat where they can talk to other users in real time.

<p align="center">
  <img src="https://media.giphy.com/media/JvnJOm9PcbbTQmClCl/giphy.gif" alt="DiscussionsGIF"/>
</p>
}
```

### Back-End Manual Installation:

It is recomended to install the backend first, make sure you have Python 3.8, Pipenv and a database engine (Posgress recomended)

1. Install the python packages: `$ pipenv install`
2. Create a .env file based on the .env.example: `$ cp .env.example .env`
3. Install your database engine and create your database, depending on your database you have to create a DATABASE_URL variable with one of the possible values, make sure yo replace the valudes with your database information:

| Engine	| DATABASE_URL 						|
| ------------- | ----------------------------------------------------- |
| SQLite	| sqlite:////test.db	 				|
| MySQL		| mysql://username:password@localhost:port/example	|
| Postgress	| postgres://username:password@localhost:5432/example 	|

4. Migrate the migrations: `$ pipenv run migrate` (skip if you have not made changes to the models on the `./src/api/models.py`)
5. Run the migrations: `$ pipenv run upgrade`
6. Run the application: `$ pipenv run start`


### Front-End Manual Installation:

- Make sure you are using node version 14+ and that you have already successfully installed and runned the backend.

1. Install the packages: `$ npm install`
2. Start coding! start the webpack dev server `$ npm run start`

## Publish your website!

This boilerplate it's 100% integrated with Herkou, just by pushing your changes to the heroku repository it will deploy: `$ git push heroku main`


		// "prettier-webpack-plugin": "^1.2.0",
"dotenv-webpack": "^1.7.0",
		"friendly-errors-webpack-plugin": "^1.7.0",
