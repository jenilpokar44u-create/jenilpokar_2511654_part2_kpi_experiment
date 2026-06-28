# Onboarding Campaign Hypothesis Testing Notes

## 1. Experiment Setup & Metrics
* **Metric Under Test:** Paid Conversion Rate (Binary metric: 1 if converted, 0 if not).
* **Why this metric:** It directly impacts our top-line revenue growth and serves as our business North Star.
* **Significance Level ($\alpha$):** 0.05 (Standard 95% confidence threshold).
* **Test Type:** Two-tailed Z-test for two independent proportions (since we are comparing the conversion rates of two large, distinct user groups).

## 2. Hypotheses Formulation
* **Null Hypothesis ($H_0$):** There is no difference in the paid conversion rate between the Control group and the Treatment group ($P_{control} = P_{treatment}$). Any observed change is purely due to random chance.
* **Alternative Hypothesis ($H_1$):** There is a statistically significant difference in the paid conversion rate between the Control group and the Treatment group ($P_{control} \neq P_{treatment}$).

## 3. Test Inputs & Summary
* **Control Group Size:** 700 users
* **Control Conversions:** 36 users (Conversion Rate: 5.1%)
* **Treatment Group Size:** 694 users
* **Treatment Conversions:** 58 users (Conversion Rate: 8.4%)
* **Observed Lift:** +3.3% absolute increase in conversion.

## 4. Statistical Output & Decision Rule
* **Calculated Z-Statistic:** 2.34
* **P-Value:** 0.019
* **Decision Rule:** Reject $H_0$ if the P-value is less than $\alpha$ (0.05).
* **Statistical Conclusion:** Since the P-value (0.019) is strictly less than 0.05, I reject the Null Hypothesis. The lift in the paid conversion rate for the Treatment group is statistically significant and not a result of random variation.

## 5. Business Interpretation
The new onboarding and activation campaign successfully drives an increase in user conversion. We can confidently report to leadership that the campaign changes positively influence a user's decision to become a paid subscriber.