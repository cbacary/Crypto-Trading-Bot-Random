# How to use it

Get an API Key from https://coinmarketcap.com/api/

run:

``python main.py -k <Your key obtained from coinmarketcap>``

Some optional args:

``-w <filename.json>`` -->  writes your portfolio to a specfied file, defualt is portfolio.json.

``-r <filename.json>`` -->  reads a portfolio from a specified file.

type 

``python main.py -h`` for additional commands.

# How it works

Using your API Key -- must be specified via CLI using the -k arg -- queries coinmarket cap 
for the top 100 coins by market cap. Randomly selects one of the coins and buys a random amount between a specified limit.
Once you have one holding it will roll the die to randomly select a holding to sell. 

# Additional Features

With the ``-s True`` argument you can selectively buy cryptos and keep track of them by using the ``-w <filename.json>`` and ``-r <filename.json>``

Example:

Start a portfolio: 

``python main.py -k <API Key> -s True -m <Amount of money to start with> -w selective_custom_profile.json``

then to get an update on your portfolio

``python main.py -k <API Key> -s True -r selective_custom_profile.json``


# Why make something so dumb?

I saw an article about a hampster that, based off of certain movements it made, would sell or buy a stock, a relatively random method of buying/selling stock/crpyto. 
This, apparently, turned out to be quite effective, if I may note, their was a similar thing done with apes. So I created a simple portfolio
and crypto buying emulator to see how it would perform. This method probably only works in bullish market conditions
and overall holding stocks/cryptos long term is a most likely a safer and more suitable method for real life. 

# Issues?

Have any issues? Create an issue or better yet a pull request!
