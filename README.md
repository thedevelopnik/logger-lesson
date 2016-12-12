# Logging to improve development
A brief instruction on using loggers to improve development. Uses a MEAN app as a starting point to teach basic logging concepts using [Winston](https://www.npmjs.com/package/winston).

## Why log?
Over and over you're probably heard "don't `console.log()`!" That is good advice, because adding console.logs is a great way to clutter up your code with actions that you won't be able to access in most cases. On the front end, it can work ok, but as soon as you deploy a server, you can't see those logs anymore. Even on the front end the logs are temporary, lasting only as long as someone can look at the console.

But logs are a critical part of debugging, *especially* when something is deployed and you no longer have easy access to console.logs. So if you're going to be logging anyways, why not add a good logging system into your development process from the start? DRY!

## Ok, you sold me, how do I start?
### Project installation
First, clone [this basic crud app](https://github.com/dsudia/mean-crud-app). Then

```
cd mean-crud-app
```

Next, you'll need to have Mongo up and running on your machine. The easiest way to do that on Mac is:

```
brew install mongodb
```

followed by

```
brew services start mongo
```

### Poking around
Open up the project in your favorite code editor. Do a find all (CMD+Shift+F in my fav, VS Code) for "console.log"

There are a number of places where console.log is being used; some just put out some basic information about an event like "Connected to database!" Others are outputting an error to the console to help in debugging. These are great use cases for logging.

What other use cases for logging have you run into for logging in your applications?
