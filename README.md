# GOAT-Discord-Bot
This project is a discord bot that uses the Algolia search API to search products and uses that information in GOAT's API to return data on a particular sneaker or piece of clothing.

# Motivation
The goal was to create something that people in the sneaker community would be able to use in their discord groups for free. Being able to visualize all the data on a sneaker at once without having to click and scroll is convenient and saves people time.

# Features
Takes in keywords from the user and displays a list of 10 possible products
- User can choose the desired product by reacting to the bot's message
  - If only 1 result is found, the user does not have to select an option
- Selection message automatically deletes
- User error handling

It returns an embed with:
- Product name w/ hyperlink
- Thumbnail Picture
- SKU
- Release Date (yyyy-mm-dd)
- Size | Lowest Ask | Highest Bid

# Bot Commands
- .goat <keywords here>

# Screenshots
![Errors](https://github.com/kxvxnc/images/blob/master/goaterror.PNG)
![Multiple Selection](https://github.com/kxvxnc/images/blob/master/goatmulti.PNG)
![Single Selection](https://github.com/kxvxnc/images/blob/master/goatsingle.PNG)
![Timeout](https://github.com/kxvxnc/images/blob/master/goattimeout.PNG)

# Installation
- Install python 3+ and add python to your PATH
- Install pip `python get-pip.py`
- Clone this repository `git clone https://github.com/kxvxnc/GOAT-Discord-Bot.git`
- Change directories to the current folder `cd /to/your/directory/GOAT-Discord-Bot`
- Install dependencies `pip install -r requirements.txt`
- Create an application at the [Discord Developer Portal](https://discord.com/developers/applications)
- Edit line 8 in main.py with your own bot token and save
- Run main.py `python main.py`