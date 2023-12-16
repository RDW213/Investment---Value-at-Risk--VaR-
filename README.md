# Investment---Value-at-Risk-VaR-

Value at Risk (VaR) Calculation for Stock Returns
This repository provides three distinct methods to calculate the Value at Risk (VaR) for stock returns: Historical VaR, Parametric (Gaussian) VaR, and Semi-Parametric VaR. VaR is a risk management metric that estimates the potential loss of an investment at a specific confidence level over a given time frame.

Methodologies:
1. Historical VaR:
Historical VaR is computed based on the historical distribution of past returns. The idea is to order historical returns from worst to best, and then identify the return value below which the specified percentage of worst returns lies. For instance, if the confidence level is set at 5%, the VaR will be the return value exceeded by only 5% of historical returns.

2. Parametric (Gaussian) VaR:
The Parametric VaR assumes that the returns follow a normal distribution. This method involves calculating the z-score, which represents the number of standard deviations a data point is from the mean. With the z-score, we can determine the return value below which the specified percentage of returns falls. The basic formula is VaR = Mean + Z * Standard Deviation, where Z is the z-score.

3. Semi-Parametric VaR (with Cornish-Fisher Modification):
The Semi-Parametric VaR builds upon the Parametric VaR but incorporates the Cornish-Fisher modification. This modification adjusts the z-score based on observed skewness and kurtosis in the return distribution. Skewness measures the asymmetry of the distribution, while kurtosis measures the thickness of the tails. By considering these factors, the Cornish-Fisher modification refines the Parametric VaR, providing a more accurate estimate.

Conclusion:
Understanding and calculating VaR using different methodologies are crucial aspects of risk management in finance. Each method has its assumptions and limitations, and the choice of which method to use depends on factors such as the data distribution and the desired level of precision.

This repository serves as a practical guide, offering users the flexibility to choose the most suitable VaR calculation method for their specific needs. It also highlights the importance of considering both historical data and statistical assumptions when assessing the potential downside risk associated with a stock investment. Feel free to adapt and extend these methodologies based on your preferences and the nature of the financial data at hand.
