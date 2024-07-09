# Cmc_Scrape_Top10
Top 10 gainers on Coinmarketcap (24hr)!

Uses selenium and result is static, for now!

Checkout the graphical version [here.]([https://link-url-here.org](https://github.com/AyFait/Cmc_Scrape_Top10_HeatMap_TreeMap)).

# Prerequisite:
I assume you know how to install and setup webdriver, either firefox or chrome. you first need to download webdriver for your os/browser and then place it in a directory
> see: https://www.selenium.dev/documentation/webdriver/

# Requirements:
webdriver 
selenium 
numpy 
pandas
time
datetime

# Issues that got fixed:
-problem: data was generated as a single list
>soln: reshaped into desired number of row n col

-prob: crypto "Symbol" was omitted in the header so it affected reshaping the array
>soln: discarded the rest of the headers all together (skipping first 5 elements of the single list) then used my own

-prob: "price, 24h%, and vol24h" was merged together thereby affecting the reshaping of the array
>soln: after reshaping the the single data list into a r×c arra.  discarded the last indexes (containing the mearged elements) first, created a new array for the discarded ones separately (splitted), concatenated both array back together horizontally (axis=1)


##calm it's literally just plug-n-play!🤧👻
##Just run CmcTop10Scrape.py
##Traders Enjoy!


# Updates:
v1.1 (Jul 1, 2024) - Added title and timestamp

![Screenshot from 2024-07-01 14-16-48](https://github.com/AyFait/Cmc_Scrape_Top10/assets/50885913/d0afbf7e-2ebc-4a5c-b06c-2dc72889076b)
