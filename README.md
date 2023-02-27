# Bond Option Valuation

We present a pricing model for bond option. Assuming that the bond price at the maturity of the option is lognormal, the model adopts the Black’s analytical closed-form solution. both the underlying spot price of bond and the strike price are clean prices (quoted prices), while dirty prices are used in the price dynamic and the closed-form solution.

In the model for bond options, bond forwards, and bond futures, coupon payment dates and accrual interest dates can be different.  

Let   be a price process of a given bond, and T be a payoff maturity date.  The bond option with the underlying B is a European type derivative security whose matured payoff at the settlement date is given by
	 	(1)
where   is the call-put index, X is the strike.  Here both the bond price and the strike price are dirty prices.  If clean prices (quoted prices) are given, such as in the GED’s token files for bond options, then accrued interests must be added to the clean prices for pricing.

Assuming that the bond price at the maturity of the option is lognormal, the prices of bond options at time zero are given by using the Black’s formula, which are
	 	(2)
	 	(3)
where c and p are the call price and the put price,   is the discount factor (see https://finpricing.com/lib/FxForwardCurve.html), and   and   are given by
	 	(4)
	 .                     	(5)
The volatility  is defined so that   is the standard deviation of the logarithm of the bond price at the maturity of the option.  The forward price of the bond   can be calculated using the formula
	 	(6)
where I is the present value of the coupons that will be paid during the life of the option.

Equation (6) actually calculates both cash forward price and cash futures price.  Let A denote the accrued interest since last coupon date on bond delivered, and let C denote the conversion factor for delivering bond.  We can calculate quoted forward price   and quoted futures price   as follows:
	 	(7)
	 .	(8)

