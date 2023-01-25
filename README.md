# FORTUNA

Powerful asset management bot with AI to automate your trading, saving you time, and trade around the clock. 

<p align="center">
  <img src="/Users/mosqui/Projects/Python/fortuna/doc/Fortuna-engraving-Hans-Sebald-Beham-1541.webp"/>
</p>

**Fortuna** is the mother of Sors and the goddess of prosperity, wealth, deity, and luck. She is associated with Greek mythology. The vague goddess was worshipped in Italy.

Like goddess Abundatia, she is also portrayed as a divine lady bearing cornucopia. It is believed that Fortuna controls the uncertainty of life, time, fate, and destinies.

Fortuna was the daughter of Jupiter. She is the foremost goddess of Greek mythology. She wields a gubernaculum, Rota Fortunae, and the wheel of fortune in her hand in some ideals.

She is mentioned in more than a thousand manuscripts, engravings, and books.  Even Shakespeare said her in one of the famous “Sonnet 29”.

## Release

### Fortuna 0 (Genesis)

Fortuna is a Python bot that will use machine learning (ML) and artificial intelligence to trade assets (stocks and cryptocurrency) on various platforms using various strategies. The first version, Fortuna 1.0, will be codenamed KLARA. 

predictor.py aims to predict the next 3 days of stock close price

| Release | Description |
| --------------- | --------------------------------- |
| Release Version | 0.1 |
| Release Date | Saturday, April 2nd, 2022 |
| Codebase | 1. Python 3.9 |
| Libraries | pip>=22.0.4 |
| | virtualenv>=20.2.2 |
| | pandas>=1.4.2 |
| | matplotlib>=3.5.1 |
| | datetime>=4.4 |
| | finrl>=0.3.4 |

pip install git+https://github.com/AI4Finance-LLC/FinRL-Library.git
Install "brew install swig" for python39 and up.
https://www.cryptohopper.com/solutions/pro-traders


### Strategy

#### Long-Short

The long-short equity strategy is implemented by this trading algorithm. In other words, the algorithm will rate a set of stocks based on a particular criterion, and it will then buy the top-ranked stocks and sell the lower-ranked ones. Specifically, the algorithm employs the standard 130/30 equity split for longs and shorts (130 percent of equity used for longs, 30 percent of equity used for shorts). The top and worst 25% of stocks will then be selected by the algorithm, and they will be long or shorted in accordance. All of the stocks in the long bucket are ordered with the same quantity since the algorithm will buy equal quantities throughout a bucket of stocks (same with the short bucket). The program will rerank the stocks periodically and modify the position as appropriate.

Certain stocks are not shortable. In this instance, the algorithm shorts the already-shorted stocks by using the remaining equity from the stocks that were unable to be shorted. The algorithm ranks the stocks according to their % change in price over the last 10 minutes, with the stocks that increased the most in value being longed and the ones that decreased the most being shorted.
 