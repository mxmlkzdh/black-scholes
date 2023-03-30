# A C++ header-only library for the Black-Scholes model

## TL;DR:
- The Black-Scholes model, aka the Black-Scholes-Merton (BSM) model, is a differential equation widely used to price options contracts.
- The Black-Scholes model requires five input variables: [the strike price of an option](https://www.investopedia.com/terms/s/strikeprice.asp), [the current stock price](https://www.investopedia.com/terms/u/underlying-asset.asp), the time to expiration, [the risk-free rate](https://www.investopedia.com/terms/i/interestrate.asp), and [the volatility](https://www.investopedia.com/terms/v/volatility.asp).
- Though usually accurate, the Black-Scholes model makes certain assumptions that can lead to predictions that deviate from the real-world results.
- The standard BSM model is only used to price [European options](https://www.investopedia.com/terms/e/europeanoption.asp), as it does not take into account that American options could be [exercised](https://www.investopedia.com/ask/answers/06/excerciseonexpiration.asp) before the expiration date.

## What Is the Black-Scholes Model?
The Black-Scholes model, also known as the Black-Scholes-Merton (BSM) model, is one of the most important concepts in modern financial theory. This mathematical equation estimates the theoretical value of derivatives based on other investment instruments, taking into account the impact of time and other risk factors. Developed in 1973, it is still regarded as one of the best ways for pricing an options contract.

## Black-Scholes Assumptions
The Black-Scholes model makes certain assumptions:

- No dividends are paid out during the life of the option.
- Markets are random (i.e., market movements cannot be predicted).
- There are no transaction costs in buying the option.
- The risk-free rate and volatility of the underlying asset are known and constant.
- The returns of the underlying asset are normally distributed.
- The option is [European](https://www.investopedia.com/terms/e/europeanoption.asp) and can only be [exercised](https://www.investopedia.com/ask/answers/06/excerciseonexpiration.asp) at expiration.


### Sources
- [The Black-Scholes Model on Investopedia](https://www.investopedia.com/terms/b/blackscholes.asp)