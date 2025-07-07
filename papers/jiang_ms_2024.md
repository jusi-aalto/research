# The Cyber Risk Premium

**Authors:** Hao Jiang*, Naveen Khanna†, Qian Yang‡, Jiayu Zhou§

*First Draft: June 28, 2020*  
*This Version: July 25, 2023*

## Abstract

Cyber risk is an important, emerging source of risk in the economy. To estimate its impact on the asset market, we use machine learning techniques to develop a firm-level measure of cyber risk. The measure aggregates information from a rich set of firm characteristics and shows superior ability to forecast future cyberattacks on individual firms. We find that firms with higher cyber risk earn higher average stock returns. When these firms underperform, cybersecurity experts tend to have higher concerns about cyber risk, and cybersecurity exchange-traded funds outperform. Further tests strengthen the identification of the cyber risk premium.

**JEL classification:** G11, G12, G14, G17.

**Keywords:** Cyber risk, Cybersecurity, Risk premium, Machine learning.

---

## Acknowledgments

We thank Will Cong (department editor), an anonymous associate editor, and two anonymous referees for helpful comments and suggestions. We also thank Andrea Eisfeldt, Nuri Ersahin, Wayne Ferson, Itay Goldstein, Larry Harris, Gerard Hoberg, Ryan Israelsen, Mete Kilic, Dmitriy Muravyev, Markus Pelger (discussant), Vincenzo Quadrini, David Robinson, Selale Tuzel, Michael Weber, Ivo Welch, and participants in seminars held at the Michigan State University and the University of Southern California, and the Winter Research Conference on Machine Learning and Business for valuable discussions. We thank Michael Weber for providing the cybersecurity risk data, Kai Li for data on corporate culture, and Philip Mattera for data on corporate misconduct.

**Author Affiliations:**
- *Corresponding author. Eli Broad College of Business, Michigan State University. E-mail: jiangh@broad.msu.edu.
- †Eli Broad College of Business, Michigan State University. E-mail: khanna@broad.msu.edu.
- ‡DeGroote School of Business, McMaster University. E-mail: yangq109@mcmaster.ca.
- §Computer Science and Engineering, Michigan State University. E-mail: zhou@cse.msu.edu.

*Electronic copy available at: https://ssrn.com/abstract=3637142*

---

## 1. Introduction

The digital transformation of the economy and increased interconnectivity have created unprecedented opportunities and under-explored risks. On the one hand, the ever-growing pool of data along with advances in artificial intelligence helps to promote efficiency and productivity in the economy; on the other hand, it exposes households, businesses, and governments to a new and potentially systemic source of risk: the cyber risk.¹ In the past decade, various forms of cyberattacks have attracted widespread attention. For instance, the Equifax data breach in 2017 exposed approximately 147 million names and dates of birth, 145.5 million Social Security numbers, and 209,000 payment card numbers along with expiration dates, which led to a settlement of nearly $700 million with federal and state investigators. The recent SolarWinds cyberattack, which came to light in December 2020, illustrates both the vulnerability of the most secure networks and the potential for immense collateral damage to corporate and governmental entities connected to these networks.

Considering the importance of cyber risk, it is natural to study how it might influence stock market prices and returns. The primary challenge for such a study is that cyber risk is new, evolving and hard to reliably estimate. To address this challenge, we use machine learning algorithms to develop a real-time estimate of the likelihood for each individual firm to experience a cyberattack in the subsequent period. Previous research has shown that firms with certain characteristics tend to have a higher likelihood of cyberattacks (Kamiya et al., 2021). Moreover, firms tend to communicate their self-perceived exposures to cyber risk through their disclosures, e.g., through 10-K filings. This information is also likely to be important in predicting the level of the firm's cyber risk. Machine learning techniques are particularly suited to this task due to their ability to extract useful information from a large set of features and to deliver superior out-of-sample forecasts.

In our empirical analyses, we introduce a novel data set of cyberattacks and apply a variety of machine learning techniques including the logistic ridge regression, the K-Nearest Neighbor, and Naive Bayes combined with an "EasyEnsemble" sampling technique (EEC-KNN and EEC-NB).² We find that our cyber risk measure based on these algorithms has a superior ability to forecast the occurrence of future cyberattacks. For instance, compared with the simple logistic forecasting model, the predictive performance of the logistic ridge regression improves from 0.4% to 6.3% based on the harmonic mean of precision and recall rates (F-score) and from around 1.4% to 59.9% based on the geometric mean of sensitivity and specificity (G-mean). Because the different machine learning techniques yield similar results, we present our main results using the logistic ridge regression, which is commonly used in asset pricing literature.

Armed with the cyber risk measure, we study how cyber risk is related to stock returns. Our primary tests use the Fama and MacBeth (1973) cross-sectional regressions to examine the incremental predictive power of the cyber risk measure for stock returns against well-known firm characteristics in the period from July 2008 to June 2019. In the first set of regressions, we include the natural log of market capitalization, book-to-market ratio, gross profitability, investment ratio, and past 11-month return skipping the most recent month as control variables. In the second set, we add past one-month return, idiosyncratic volatility (Ang et al., 2006), and the Amihud illiquidity ratio (Amihud, 2002). In a contemporary study, Florackis et al. (2023) propose a cyber cosine measure based on the linguistic similarity between hacked and non-hacked firms in the risk factor section of their annual reports, which is also included in some of our regression specifications. In all these regressions, the relation between cyber risk and stock returns is economically meaningful and statistically significant. In terms of magnitudes, a one standard deviation increase in cyber risk is associated with higher average stock returns of between 0.15% and 0.20% per month. These results show that cyber risk is an independent and important driver of cross-sectional variation in stock returns during our sample period.

We also perform a standard portfolio analysis. At the end of each June from 2008 to 2018, we sort stocks into five quintiles based on the estimated level of cyber risk using information available in real-time and form value-weighted portfolios that are rebalanced at the end of the following June. Consistent with the Fama-MacBeth regressions, we find that stocks in the top quintile with the highest level of cyber risk have higher returns than those in the bottom quintile. The spread in returns is 0.84% per month after we adjust for their market exposure and 0.58% per month after adjusting for Fama-French five factors and momentum. The alpha remains large and statistically significant when we form tercile and quartile portfolios as well as under alternative asset pricing models.

In addition to the cross-sectional variation in average returns, we examine the time variation in the relative returns between stocks with high and low cyber risk. We conduct two tests. First, we study the relation between the variation in the return difference between high and low cyber risk stocks and the New York University's Index of Cyber Security (ICS), which is based on monthly surveys of industry executives about their perceived level of cyber risk. Because ICS is a monthly aggregate measure of cyber security, we form a factor-mimicking portfolio and compute its performance. We estimate each stock's return sensitivity to changes in ICS in the past year. A lower ICS beta is associated with higher firm-level cyber risk. Then we form a spread portfolio that buys stocks with high ICS beta and sells those with low ICS beta. The return on the spread portfolio based on our cyber risk measure and that based on the ICS beta have a strong negative comovement, with a time-series correlation coefficient of −32%.

Second, we study the relation between the performance of the spread portfolio based on our cyber risk measure and that of two cybersecurity ETFs that invest in firms providing cybersecurity services. We again find strong negative comovements between the two, with time-series correlation coefficients below −40%. That is, when stocks with higher cyber risk underperform, cybersecurity firms tend to have higher returns. These results suggest that the time variation in the return spread between high and low cyber-risk firms is likely driven by the market's perception of cyber risk in the economy.

The strong relation between our cyber risk measure and future stock returns is consistent with the view that cyber risk is priced in the stock market. We conduct a number of tests to strengthen the identification of the cyber risk premium. First, we exploit the variation along the dimension of industry competition. Kamiya et al. (2021) shows that the negative stock market reaction to cyberattacks on target firms spills over to their peers around the announcement of cyberattacks. We find that this spill-over effect is larger when the hacked firm is a stronger competitor of its peer firms in the product market. This is because weaker peer firms are less likely to be able to increase market share at the expense of a stronger competitor—the repricing effect of their shares due to market recognition of their cyber risk exposure is less confounded by the effects of product market competition. Second, firms that provide products and services similar to those of hacked firms are likely to hold similarly valuable data, which makes them vulnerable to cyberattacks. We use the product similarity measure proposed by Hoberg and Philips (2016) as a proxy for data similarity. We find that peer firms with higher data similarity to hacked firms tend to experience a more negative stock market reaction around the announcement of cyberattacks, and that data similarity is a positive contributor to our cyber risk measure. These tests provide further evidence for cyber risk being an important determinant of stock returns.

We evaluate the robustness of our results by performing additional tests. First, we split our sample into two subperiods. We find that in both periods, the cyber risk measure is positively related to future stock returns, with the effect slightly stronger in the more recent subperiod. Second, we construct a cyber risk measure based on industry-adjusted risk disclosure variables and compute industry-adjusted returns for each stock in our sample. In both cases, we find that the positive relation between cyber risk and future stock returns remains strong. Third, to address the concern that our cyber risk measure may be driven by other dimensions of risks such as corporate fraud, we use our measure to predict the incidence of corporate misconduct and financial misconduct. Our tests empirically reject this hypothesis. Fourth, we consider different machine learning algorithms and use different dictionaries in linguistic analyses to estimate the cyber risk measure. The results are robust. Finally, we consider a placebo test to pinpoint the importance of cyber risk. In particular, we randomly select firms to construct a fake sample of cyber-attacked firms. The number of random draws to create the fake sample equals the actual number of cyberattacks for each industry in each year. We then use the same machine learning algorithms to estimate each firm's pseudo-cyber risk and estimate its relation to stock returns. Our results show that this relation is essentially flat. This result highlights the importance of cyber risk in driving stock returns.

Our study contributes to the fast-growing literature that studies the implications of cyber risk for firms, the financial markets, and the economy. Many studies in this literature focus on the impact of realized cyberattacks. For instance, Kamiya et al. (2021) find that the announcement of successful cyberattacks is, on average, associated with a 1.09% wealth loss for shareholders within a three-day window around the incidents. They argue that successful cyberattacks lead to value loss for hacked firms for both actual and reputational reasons.³ Notable exceptions include Jamilov et al. (2020), and Florackis et al. (2023), who use textual information to identify firms with high cybersecurity risk. Jamilov et al. (2020) use firms' earnings conference call transcripts to develop a measure for firm-level cyber risk exposure and sentiment and report a number of interesting findings, such as an increase in corporate discussions of cyber risk in earnings calls, increasingly negative sentiment regarding cyber risk, and the spread of cyber risk discussions across regions.⁴ However, they do not distinguish between cyber risk exposure and cyber risk awareness. For instance, corporate managers' extensive cyber risk discussions in conference calls can be driven by their keen awareness of cyber risk; a lack of such discussions can be driven by their inadequate attention to or even ignorance of cybersecurity risk. Our results are robust to excluding textual variables from the cyber risk measure. Closer to us, Florackis et al. (2023) study the relation between cyber risk and stock returns. They use firms' descriptions of cyber-related risk in 10-K reports to identify firms with high cyber risk. Their conclusion that cybersecurity risk is priced in the cross-section of stock returns provides independent support for our results. The main difference between their study and ours is methodological. Florackis et al. (2023) compare the word distribution of "Item 1A. Risk Factors" in the 10-K reports of training firms with that of the hacked sample, identifying the most similar firms as high cybersecurity risk firms. Their method is simple and powerful, relying only on the textual data in firms' annual reports. Our machine learning algorithms provide a mapping from any feature set to the occurrence of cyberattacks. The special strength of our approach is its flexibility: the feature set can be expanded to encompass any form of data, including traditional and alternative data.

Our paper also joins the burgeoning literature that applies machine learning techniques to asset pricing. This literature has focused on using machine learning algorithms to efficiently select and combine firm characteristics to predict stock returns (see, e.g., Freyberger et al. (2020); Gu et al. (2020)) and to construct a robust stochastic discount factor (see, e.g., Kelly et al. (2019), Kozak et al. (2020), and Chen et al. (2023)). Recent work combines state-of-the-art machine learning/artificial intelligence technologies and economic restrictions to directly facilitate portfolio optimization and stock return prediction while improving economic interpretability. For example, Cong et al. (2021) combines deep reinforcement learning and economic restrictions to construct optimal portfolios that can achieve outstanding out-of-sample performance; Cong et al. (2023a) develops a class of interpretable tree-based models to shed light on the characteristics that separately drive the cross-sectional variation of stock returns and regime changes in the macroeconomic environment. Instead of directly targeting asset returns, our paper uses machine learning techniques to estimate an important, emergent risk as economies become more digital. Our approach exploits the correlations between firm characteristics and the likelihood of cyberattacks and shows that the resulting estimate of cyber risk has predictive power for stock returns beyond the usual firm characteristics.

The rest of the paper is organized as follows. Section 2 describes the data. Section 3 shows the methodology to construct the cyber risk measure. Section 4 presents the key results on the relationship between cyber risk and stock returns. Section 5 provides further identification of the cyber risk premium. Section 6 reports robustness tests. Section 7 concludes.

---

## 2. Data

### 2.1. Cyberattacks

In this paper, we use a novel data set obtained from the Identity Theft Resource Center (ITRC).⁵ It has a number of advantages over the data set from the Privacy Rights Clearinghouse which has been used previously in the literature.⁶ It provides more up-to-date data, reports many more cyberattacks on public firms, and importantly, contains the source of the reports, which allows for cross-validation. ITRC provides annual data breach reports from the year 2005, detailing all the reported and confirmed cyberattack incidents for US-based organizations. These reports are stored on their website in the form of PDF files. We obtained the available annual reports from 2005 to 2019 and extracted all items connected to cyber incidents. We first matched them to Compustat firms using a fuzzy matching algorithm, and then manually checked each one of the matched pairs for confirmation. After this process, we are left with 1,010 cyberattack incidents.⁷ Since we use the cyberattack as a binary variable, we count multiple attacks of a firm in a given year as one instance. This leaves us with 552 unique firm-year pairs, with 368 unique firms that experienced at least one cyberattack incident. Because we use accounting variables as predictors, we follow the convention in Fama and French (1996) and define each year as the 12 months from July to the following June. The sample then spans from 2006 to 2018.⁸ Figure 1 plots the number of unique incidents and the unique firm-year pairs for firms that experienced cyberattacks during the sample period. It shows an increasing time trend in cyberattacks.

From Figure 2, we find that the financial sector is the hardest-hit industry, with a total of 247 incidents, dwarfing all other sectors. This is not surprising because financial firms possess large amounts of client identification and financial data. With the exception of the "Mining and Minerals" industry, no sector appears immune to cyberattacks as firms increasingly rely on online platforms to conduct their business and on cloud services to store their data.

Before leaving this subsection, we shall note that in an important paper, Cong et al. (2023b) point out that a large fraction of cybercrimes and cyberattacks are unreported and kept hidden by hacked firms. The under-reporting and under-recording would lead researchers to miss instances of cyberattacks, the inclusion of which may increase the statistical power of empirical tests to identify the risk premium. One useful observation from our analyses is that when we restrict our sample of cyberattacks to significant incidents with strong stock market reactions, the algorithm shows stronger power in identifying the risk premium associated with cyber risk. If the incentive to underreport cyberattacks is stronger for more significant incidents, it would lead us to underestimate the importance of cyber risk in the stock market. Future research will benefit from a more comprehensive data coverage of cyberattacks.

### 2.2. Other Data

The rest of the data sources are as follows. Stock price and return data are from the CRSP. Accounting data are from Compustat. Asset pricing factors are from Kenneth French's website.⁹ The 10-K filings are from the University of Notre Dame Repository website.¹⁰

### 2.3. Summary Statistics

Table 1 summarizes the characteristics of firms that experience cyberattacks (hacked firms) and those that do not (non-hacked firms) in our sample. All the variables are measured prior to the year when the incidents happen. The accounting variables are lagged by six months to ensure data availability. We follow Kamiya et al. (2021) in the definitions of the firm characteristics. In addition, we use two linguistic variables: the "Risk Factor Length," which is based on the length of "Item 1A: Risk Factors" in the firm's 10-K disclosure, and the "NIST Counts," which is the number of times a firm mentions a cybersecurity-related term in Item 1A, based on the NIST dictionary. We discuss this dictionary in more detail in Section 3.

Table 1 shows that hacked firms tend to be larger, which suggests that hackers target firms with larger customer bases and bigger data sets, as such targets are likely to offer them potentially higher gains. They also tend to have more intangible assets, have higher cash flow, spend less on research and development, have a higher return on assets, and experience higher past year excess returns. These characteristic differences are in line with the results in Kamiya et al. (2021). In addition, hacked firms tend to spend more time discussing cybersecurity-related risks in their 10-K disclosure. In the next section, we describe how we use these characteristics to construct the firm-level measure of cyber risk.

---

## 3. Measuring Firm-Level Cyber Risk

A well-known insurer, Northbridge Insurance, provides a broad definition of cyber risk: "Cyber risk commonly refers to any risk of financial loss, disruption or damage to the reputation of an organization resulting from the failure of its information technology systems."¹¹ To operationalize this notion, we follow the literature (e.g., Kamiya et al. (2021) and Michel et al. (2020)) and treat reported cyberattacks as realized cyber risk. Based on these cyberattacks, we use machine learning algorithms to develop a real-time estimate of the likelihood for each individual firm to experience a cyberattack in the subsequent period.

### 3.1. Constructing Predictors

Kamiya et al. (2021) document that a set of firm-specific variables are correlated with the probability that a firm experiences a cyberattack. We use these variables as the starting point in building our model. The variables include asset intangibility, the ratio of capital expenditures to total assets (CAPX/AT), the ratio of cash flows to total assets (CF/AT), firm size, net worth, R&D, ROA, Tobin's q, sales growth, financial constraint, prior year excess return over the CRSP value-weighted market return, and the natural log of firm age.

In addition, we explore soft information about a firm's cyber vulnerability. One source is a firm's self-assessment of its cyber risk disclosed in the "Item 1A: Risk Factors" section in firms' annual 10-K filings. The SEC requires that firms disclose the most significant risk factors.¹² Per this requirement, firms started to include this section prominently and regularly from 2006. Firms are in a unique position to assess their own risk level given their private information and familiarity with the firm's operations. In addition, this risk disclosure is forward-looking, providing useful information about the perceived exposures. The nature and intensity of the discussion on cyber-related risk in their 10-K filings should be a useful indicator of their firms' vulnerability to cyberattacks.

To measure the intensity of perceived cyber risk, we count the number of times a firm mentions cyber risk-related terms in the risk factors section in its 10K filing as well as the length of the entire section. In this way, we can capture the information about a firm's self-assessment of both its overall risk exposure and exposure specific to cyber risk.

To identify cyber risk terms, we exploit a specialized dictionary compiled by the National Institute of Standards and Technology (NIST), named the "Glossary of Key Information Security Terms."¹³ An important feature worth noting is that the NIST dictionary was compiled in 2006, suggesting that cyber risk was already a concern with governmental bodies. Secondly, it avoids a potential look-ahead bias since our sample starts in the year 2006.¹⁴

Next, we turn to firms' annual 10-K filings. Since the SEC mandate for disclosing risk factors came into effect in 2006, we start our sample in 2006. We obtain the filings from 2006 to 2018 through the University of Notre Dame Repository and extract their risk factor sections.¹⁵ We use the central index key (CIK) to match the filing firms to Compustat firms. Then we count the number of tokens per risk factor text block, only keeping the blocks with at least 100 tokens.¹⁶

The final step in constructing the cyber risk disclosure variable is to measure the intensity with which cybersecurity-related terms are mentioned. We apply the following procedure: first, we measure the maximum number of tokens in each term in each dictionary. We find that the NIST dictionary contains terms that can be as long as seven tokens. Second, to control for the fact that there might be common boilerplate language that most firms use, we eliminate the common terms used by firms in each year as in Hoberg and Philips (2016). Third, we transform each risk factor text block into a collection of Ngrams, where N ∈ [1, 2, 3, 4, 5, 6, 7]. Each Ngram is a collection of every possible combination of adjacent N tokens in each document.¹⁷ Finally, we count how many times each cybersecurity term occurs in each Ngram-transformed text block.

We use the length of the risk factor section and the NIST term frequency as two separate variables for two reasons. First, the length of the risk factor section measures the number of tokens, or uni-grams, while the NIST term frequency is the number of times each term is mentioned. Here the term ranges from uni-grams to seven grams, and thus it is inappropriate to scale the frequency by the length of the section. Second, we keep both variables in the feature set to maximize the power of the machine-learning techniques.

### 3.2. Constructing the Predictive Model

#### 3.2.1. In-sample Fit

Before building the predictive models, we examine the in-sample explanatory power of the regressors we select in-sample. In particular, we perform in-sample logit regressions, which include the accounting and text-based variables, which are cross-sectionally standardized to have means of zero and standard deviations of one. Following Petersen (2009), we cluster standard errors by both firm and year.

The results in Table A.1 of the Appendix show that many firm characteristics have strong associations with the probability of future cyberattacks. In terms of magnitudes, firm size is particularly important, with larger firms more likely to be attacked. We also find that the text-based cyber risk count variables have positive predictive power for future cyberattacks. Interestingly, as shown in Column (1), the total number of tokens in the Risk Factors section of a firm's 10-K filing has a negative association with the probability of future cyberattacks. This result suggests that firms with more thorough discussions of their risk factors may also have better risk management practices.

#### 3.2.2. Building Machine Learning Predicting Models

To build an effective cyberattack forecasting model, there are two main considerations. First, an in-sample fit could induce look-ahead bias and overfitting. Second, cyberattacks are rare events, which result in a highly imbalanced sample, thereby introducing biases into the Maximum Likelihood Estimator (King and Zeng (2001)).

To address the possible look-ahead bias, we follow a recursive and expanding prediction procedure. Namely, we start from the year 2006, run a predictive model, save the coefficients, and then use them to fit the data in 2007. We do this recursively, so the final step is to use the data from 2006 to 2017 to train the model to fit the year 2018. In this way, we avoid the look-ahead bias and generate true out-of-sample (OOS) predictions.

Next, to address overfitting and maximize OOS performance, we introduce machine learning classification models to improve the predictive power. In particular, we select logistic ridge regression as our main model.¹⁸ The logistic ridge regression combines the logistic regression with ridge regularization, which uses an L-2 penalty.¹⁹ The objective function for logistic ridge regression is:

$$\min_{\beta_0,\beta\in\mathbb{R}^{p+1}} -\left(\frac{1}{N}\left[\sum_{i=1}^{N} y_i \cdot (\beta_0 + x_i^T\beta) - \log(1 + e^{\beta_0+x_i^T \beta})\right]\right) + \frac{1}{2}\lambda\|\beta\|_2^2 \quad (1)$$

where β is the slope coefficients, p is the number of parameters, λ controls the regularization strength, $y_i$ is the response or dependent variables, and $x_i$ is the predictors or independent variables.

To fully exploit the conditioning information and the logistic ridge regression's regularization capability, we perform the polynomial transformation of our regressors.²⁰ A polynomial transformation of degree d converts the variables to all possible interactions and powers up to degree d. In our implementation, we choose a polynomial transformation of degree 4.

In each training window, we tune hyperparameters for optimal performance via three-fold cross-validation, using the training data in each recursive sample period. Cross-validation is done through the following procedure: for the training data in each window, we randomly split the training data into three folds, i.e., three subsets of equal size; we use two of the three folds to fit the model, and one remaining fold as the "validation set" to find the best estimator; we iterate this procedure three times and find the best estimator, in terms of out-of-sample performance metric (based on the validation set of each iteration); then we use this estimator for prediction on the test data. Since regularization is sensitive to the unit of variables, we standardize the variables before the training process (Hastie et al., 2017).

Since our sample is highly imbalanced, we use the stratified K-fold strategy of Zeng and Martinez (2000) to ensure that the class distribution is maintained across all folds. In addition to tuning the penalty factor λ, we also tune the class weight parameter in the loss function, using a heuristic proposed by King and Zeng (2001).²¹

#### 3.2.3. Filtering the Sample

In our study, we wish to capture significant cyberattacks with meaningful impacts on the hacked firms. In a contemporaneous study, Florackis et al. (2023) select events that are prominently featured in media reports as a filter that identifies important attacks. We take a similar but more direct approach: we use a filter based on the 7-day cumulative abnormal returns (CAR) around the events. Specifically, we first calculate the [-3,3] window CAR for each event using a four-factor model, the Fama-French three factors and the momentum factor, as the benchmark. Then we choose the events with an absolute value of CAR greater than 1%; we consider these events as important to investors based on the stronger market reaction.²² After using this filter, our sample consists of 394 cyberattacks from 2007 to 2018.

#### 3.2.4. Evaluating the Forecasting Performance

To evaluate the performance of the logistic ridge regression against the simple logistic regression, we follow the machine learning literature and choose three commonly used metrics of forecasting performance: the F1-score, G-mean, and Balanced Accuracy.²³

The building blocks for these metrics include recall (also called sensitivity), precision, and specificity.

$$\text{Recall} = \text{Sensitivity} = \frac{\text{True Positives}}{\text{True Positives + False Negatives}}$$

$$\text{Precision} = \frac{\text{True Positives}}{\text{True Positives + False Positives}}$$

$$\text{Specificity} = \frac{\text{True Negatives}}{\text{True Negatives + False Positives}}$$

The F1 score is the harmonic average of recall and precision. G-mean is the geometric average of recall and specificity. Balanced Accuracy is the arithmetic average of sensitivity (recall) and specificity.

Table 2 compares the average forecasting performance of the logistic ridge regression with that of the commonly used simple logistic regression over our sample period. Figure 3 presents the time series of the performance metrics.

The results show that the logistic ridge regression strongly outperforms the baseline logistic regression across all three performance metrics. For instance, the average F1 score of the logistic ridge regression is approximately 15 times as large as that of the logistic regression, and the average G-mean of the logistic ridge regression is approximately 40 times as large as that of the logistic regression. The Balanced Accuracy of the logistic ridge regression exceeds that of the logistic regression by approximately 30%. The strong outperformance of the logistic ridge regression is persistent through time.

To understand the drivers of the superior performance of the logistic ridge regression, we plot the aggregate (or equivalently, mean) confusion matrices for the logistic ridge and logistic regressions in Figure 4. The rows of a confusion matrix are the true classes, while the columns are predicted classes. Each of the four quadrants indicates the total number of observations across the sample period classified per the prediction model.

In a confusion matrix, a superior forecasting technique tends to register higher relative numbers in the diagonal elements, which implies that the classifier more correctly classifies observations. The results show the source of the weakness of the simple logistic regression: it overwhelmingly predicts firms as negative cases and under-predicts the positive cases. Among the firms that experience a cyberattack the following year, the algorithm falsely predicts more than 99% of them as negative cases. In comparison, the logistic ridge regression falsely predicts approximately 50% of them as negative cases. In other words, the logistic ridge regression benefits from a jump in recall in exchange for a small decrease in precision, and thus achieves a better balance in performance.

In the rest of the paper, we use the cyber risk measure based on the logistic ridge regression as the primary measure. We present the results based on alternative machine learning techniques in Section 6 as robustness tests.

#### 3.2.5. Characterizing the Firms with High Cyber Risk

Figure 5 shows the correlation coefficients between our cyber risk measure and firm characteristics. The left column presents the time-series averages of the cross-sectional Spearman correlations, and the heat map is based on the absolute value of the average correlation coefficient.

The results of average correlation coefficients indicate that firms with higher cyber risk tend to be larger, less financially constrained, and more profitable. The heat map also shows that these three characteristics tend to have high and stable correlations with cyber risk across time. In addition, the text-based variables have high correlations with cyber risk.

Before leaving this section, we examine the relation between our cyber risk measure and the measure of Cyber Cosine developed by Florackis et al. (2023). Although both measures intend to capture firm-level cyber risk, the methodologies are distinct. It is therefore of interest to quantitatively examine the relation. We find that the two measures have positive but moderate correlations, with a Pearson correlation coefficient of 14% and Spearman correlation coefficient of 30%. Because the Cyber Cosine measure is purely text-based, it also makes sense to compare the correlation between their measure and the textual variables we use in our cyber risk forecasting model. We find that the correlation between Cyber Cosine and the "NIST Counts" is 0.40 and that between Cyber Cosine and "Risk Factor Length" 0.27, suggesting that our textual variables have a stronger comovement with Cyber Cosine. Overall, these results show that our cyber risk measure and the Cyber Cosine measure share a moderate amount of common information. In other words, both measures should be of value for studies on cyber risk.

---

## 4. Cyber Risk and Stock Returns

In this section, we study the relationship between cyber risk and stock returns. We start with cross-sectional analyses using both the Fama and MacBeth (1973) regressions and portfolio analyses. Then we examine the time variation in the return spread between firms with high and low cyber risk, focusing on its comovement with other measures of aggregate cyber risk concern.

### 4.1. Cross-sectional Regressions

To examine whether firms with higher cyber risk compensate investors with higher average returns, we use Fama-MacBeth cross-sectional regressions to examine the incremental predictive power of the cyber risk measure for stock returns, controlling for well-known stock characteristics proposed in the previous literature. Specifically, at the end of each month from July of year t to June of year t + 1, we regress individual stock returns on our cyber risk measure estimated in year t and a set of firm characteristics. The cyber risk estimate is based on firms' accounting information for the fiscal year ending anytime in the calendar year t − 1, the cyberattack forecasting model parameters estimated using the accounting information available up to June in year t − 2, and the cyberattack incidents available up to the end of June of year t − 1. The year t ranges from 2008 to 2018. All regressors are cross-sectionally standardized to have a mean of zero and a standard deviation of one. Then we test whether the time-series averages of the regression coefficients are statistically significant. The standard errors are based on the Newey and West (1987) adjustment with 6 lags. For a stock to be included in the analysis, it is required to have a CRSP share code 10 or 11 and to have a closing price above $5 at the end of June in year t.

Table 3 shows the results. In Column (1), we include our cyber risk measure, together with control variables including natural log of market cap, natural log of book-to-market ratio, gross profitability, asset growth, and momentum (measured as prior twelve to one-month return). Column (2) replaces our cyber risk measure with Cyber Cosine of Florackis et al. (2023). Column (3) jointly includes our cyber risk measure and the Cyber Cosine measure. Column (4) further includes the past one-month return to control for short-term return reversal, idiosyncratic volatility (Ang et al., 2006), and illiquidity (Amihud, 2002).

The results in Table 3 show a strong relation between our cyber risk measure and future stock returns. For instance, Column (1) indicates that a one-standard-deviation increase in cyber risk is associated with an approximately 20 basis-point increase in returns per month, or 2.4% per year. The effect is statistically significant at the 1% level. Consistent with Florackis et al. (2023), we find in Column (2) that the Cyber Cosine measure has strong predictive power for future stock returns. When we include both variables in the same regression in Column (3), both our cyber risk measure and the Cyber Cosine measure have strong relations with future stock returns. In terms of magnitudes, the coefficient for our cyber risk measure is 0.186 and that for the Cyber Cosine measure 0.093. This result indicates that our cyber risk measure captures independent information about firms' cyber risk exposure as compared to the Cyber Cosine measure of Florackis et al. (2023). Columns (4) further establishes the robustness of the results when we include more control variables.

### 4.2. Portfolio Sorts

We also use the portfolio approach to examine the relationship between cyber risk and stock returns. At the end of each June from 2008 to 2018, we sort stocks into three tercile portfolios, four quartile portfolios, and five quintile portfolios according to the cyber risk measure. These portfolios are held until the end of June in year t + 1 and then rebalanced based on the updated cyber risk estimate when new information becomes available.

We create zero-cost hedge portfolios that buy high cyber-risk stocks and short low cyber-risk stocks. We compute the monthly equal- and value-weighted alphas on the hedge portfolios using a number of asset pricing models: the CAPM, Fama-French three-factor model (FF3), FF3 augmented by a momentum factor (FF4), Fama-French five-factor model (FF5), and FF5 augmented with a momentum factor (FF6).

Table 4 shows that the hedge portfolios generate large alphas across the different portfolio constructions and against the various benchmark models. The monthly alpha ranges from 40 to 80 basis points per month and is always statistically significant. These results show that investors in high cyber-risk stocks earn high average returns, which cannot be explained by these asset pricing models.

### 4.3. Comovement with the Index of Cybersecurity

In addition to the cross-sectional variation in average returns, we examine the time variation in the relative returns between stocks with high and low cyber risk. In this subsection, we relate the return spread to the index based on an independent survey conducted by New York University on the perception of cyber risk among industry experts: the Index of Cybersecurity (ICS).²⁴ Each month, the survey queries experts such as chief risk officers, chief information security officers, selected academicians engaged in fieldwork, and selected security product vendors' chief scientists about their perceived level of cyber risk, from which an aggregate measure of cyber risk is built.

To examine the relationship between our annual firm-level cyber risk measure and the monthly aggregate ICS, we project both variables onto the return space. For each stock in our sample, we estimate its return sensitivity to the monthly percentage change in the ICS. That is, we perform bivariate regressions of monthly excess returns of individual stocks on the monthly changes in the ICS and the excess returns on the market portfolio. Stocks with a high (low) ICS beta tend to have lower (higher) cyber risk exposures based on the ICS. Therefore, a long-short portfolio that buys stocks with a high ICS beta and sells those with a low ICS beta should deliver higher performance when aggregate cyber risk concern is high. If our firm-level cyber risk measure and the ICS capture some common component of cyber risk in the economy, we would expect the portfolio that buys high cyber-risk stocks and sells low cyber-risk stocks to have a negative correlation with the ICS factor-mimicking portfolio.

We apply a 12-month rolling window to estimate the ICS beta for individual stocks, requiring at least six observations for the statistical estimation. We form five quintile portfolios at the end of each month from December 2015. Then we repeat this process for each subsequent month. Therefore, we have monthly ICS beta portfolios from December 2015 to June 2019, with concurrent observations for our cyber risk-based quintile portfolios.

Panel A of Figure 6 shows the performance of the portfolio that buys stocks with high cyber risk and sells those with low cyber risk (the solid black line) against the return on the portfolio that buys high ICS beta stocks and sells low ICS beta stocks (the dotted red line). Consistent with our conjecture, the two series show a strong negative comovement. The time-series correlation coefficient is -41.2% and statistically significant.

### 4.4. Comovement with the Cybersecurity ETFs

In this subsection, we use the return on cybersecurity index ETFs as another proxy for aggregate concern about cyber risk. The conjecture is that when investors have stronger concerns about cyber risk, cybersecurity ETFs tend to outperform. Our analyses include two such ETFs: the First Trust Nasdaq Cybersecurity ETF (CIBR)²⁵ and ETFMG Prime Cyber Security ETF (HACK).²⁶ Both ETFs track a set of firms that provide cybersecurity services. Table 5 shows their top ten holdings.

Panel B of Figure 6 plots the monthly returns on the spread portfolio that buys high cyber risk stocks and sells low cyber risk stocks (the solid dark line) against the performance of the cybersecurity ETFs (the dotted blue and dashed green lines). It shows a strong negative comovement. The time-series correlations are below -40% for both ETFs. If we perform a time series regression of our cyber risk portfolio return against the two ETF returns individually, the coefficients are -0.405 and -0.312, respectively, for CIBR and HACK, and are statistically significant at the 1% level. This result provides further validation for our cyber risk measure.

As a still further validation, we hypothesize that when major cyberattacks happen, high cyber-risk firms would underperform low cyber-risk firms. To examine this conjecture, we first identify major cyberattacks via a Bloomberg report.²⁷ Because the list consists of private and public firms, we further screen the list to include only public firms to match our sample. We then manually check the dates to ensure they reflect when the attacks became public. The final list includes the following firms: Yahoo! (September 2016), Equifax (September 2017), Under Armor (March 2018), Facebook (September 2018), and Quest Diagnostics (June 2019). We mark these events in both panels of Figure 6. The figure shows clearly that our cyber risk high-minus-low portfolio underperformed when major cyberattacks happened, while the ICS beta portfolio and cybersecurity ETFs overperformed, consistent with our conjecture. These results provide further evidence for the validity of our cyber risk measure.

---

## 5. Is Cyber Risk Priced? Further Identification

The preceding results show a strong relation between our cyber risk measure and future stock returns, which is consistent with the view that cyber risk is priced in the stock market. In this section, we provide further tests that strengthen the identification of the cyber risk premium.

### 5.1. Industry Competition

We start by exploiting the variation along the dimension of industry competition. Kamiya et al. (2021) show that when a firm is hacked, its peer firms in the same industry tend to experience stock price drops around the announcement. This result is consistent with the view that increased awareness of cyber risk exposure for peer firms leads the stock market to reprice their stocks. Building on this observation, we hypothesize that the average market reaction to peer firms is confounded by the nature of product market competition in the industry. For instance, if the hacked firm is a weaker player in the product market, the incidence of a cyber attack is likely to provide its stronger competitor an opportunity to increase market share. Thus, the stock market reaction to the cyber risk exposure of the peer firm can be muted by the stock market's perception of its improved product market opportunities. However, this confounding effect is likely to be weaker when the hacked firm is a stronger player in the industry: It is harder for a weaker competitor to exploit the potential opportunity to the same extent.

To empirically test this hypothesis, for each hacked firm, we identify its peers in the same industry based on the Fama-French 48-industry classification (Fama and French, 1997). We construct a variable "Strong Victim" to capture the relative competitive position of the hacked firm (victim) to a peer firm: It equals one if the hacked firm has a higher market share (firm sales over industry sales) than that of the peer firm, and zero otherwise. The idea is that if the hacked firm is a stronger (weaker) competitor of the peer firm, the peer firm is less (more) likely to increase its market share in response to a cyberattack on the target firm. As a result, the negative market reaction to the peer firm around the time period when the data breach of the hacked firm becomes public would be stronger. This is because it is a cleaner test of the market price reaction of a peer's stock as investors re-calibrate their estimate of its cyber risk in response to the firm getting hacked. That is, in a regression of the [-3,+3] window cumulative abnormal return (CAR) of the peer firm on the [-3,+3] window CAR of the hacked firm around the date when the data breach is announced, the coefficient for the interaction of the "Strong Victim" dummy variable and the hacked firm's CAR is expected to be positive.

Table 6 presents the results based on the cyberattack events when the hacked firm experiences a CAR of lower than -1% during the [-3,+3] window. In Column (1), we confirm the analysis in Kamiya et al. (2021) that when focal firms experience a cyberattack, peer firms in the same industry also suffer, demonstrated by the statistically significant and positive coefficient for "Victim CAR". Column (2) shows that the "Strong Victim" variable itself has no effect on the stock market reaction of peer firms. However, when we interact "Strong Victim" with "Victim CAR", the coefficient for the interaction is statistically significant and positive. The spillover of the negative stock market reaction from the hacked firm to its peer firms is stronger when the confounding effect from the product market is weaker. This reinforces our claim that cyber risk is an important driver of stock prices.

### 5.2. Product Similarity as a Proxy for Data Similarity

We note that firms with valuable data holdings tend to be particularly vulnerable to cyberattacks. Based on this observation, we seek to identify firms with data holdings similar to the hacked firm. Hoberg and Philips (2016) propose an interesting measure that captures the similarity of products and services between two firms. If two firms provide similar products and services to their customers, it is likely that the data generated and stored by the two firms would be similar. Based on the Hoberg and Philips (2016) product similarity score, we identify firms providing similar products and services to those of the hacked firm. Since these firms should have a higher probability of experiencing a cyberattack due to their data similarity to the hacked firm, a public release of information about a hack would lead the stock market to update their beliefs about the cyber risk exposure of these firms, resulting in a larger stock price drop for them.

To test this hypothesis, we use the event study framework similar to the preceding tests, focusing on the interaction between "Data Similarity" and "Victim CAR". In Table 7, we find that firms providing products and services similar to those of the hacked firm experience a more negative market reaction when the data breach of the hacked firm becomes public, which supports our hypothesis. In terms of magnitudes, because the data similarity measure has a mean of 0.022 and a standard deviation of 0.045, a one-standard-deviation increase in data similarity is associated with an increase in the response of peer firm's stock price to the CAR of the hacked firm by 0.037 (0.045 × 0.82).

Building on the success of the Hoberg and Philips (2016) product similarity measure to capture data similarity, we construct a firm-level Composite Data Similarity measure that averages a firm's data similarity with all the firms experiencing a cyberattack in the previous year:

$$\text{CompositeDataSim}_{i,t} = \frac{1}{m}\sum_{j=1}^{m} \text{DataSim}_{i,j,t} \quad (2)$$

where i represents individual firms in the Compustat universe, j indexes firms that have been attacked in year t, and DataSim is the product similarity score measure in Hoberg and Philips (2016). Thus CompositeDataSim is the average data similarity of each firm to the group of attacked firms in the previous year.

Since a firm holding valuable data similar to previously attacked firms is a more likely target, we expect its composite data similarity score to be a positive contributor to a firm's cyber risk. To examine this conjecture, we regress both our cyber risk measure and the Cyber Cosine measure proposed by Florackis et al. (2023) on the composite data similarity. To make the coefficients comparable, we standardize each of the continuous variables to be have a mean of zero and a standard deviation of unity. The results in Table 8 are consistent with our hypothesis. The coefficients for the "Composite Data Sim" are positive and statistically significant across the different specifications. A one-standard-deviation increase in "Composite Data Sim" is associated with a 0.012 standard deviation increase in our "Cyber Risk" measure, and a 0.038 standard deviation increase in the "Cyber Cosine" measure, when we control for the effects of firm size and book-to-market ratio. These results support the idea that valuable data holdings tend to attract the attention of hackers, which increases the cyber risk of a firm.

---

## 6. Robustness Tests

### 6.1. Sub-sample Analysis and Industry Effects

To evaluate the robustness of our results, we split our sample into two subperiods and perform the Fama-MacBeth regressions of stock returns on cyber risk and other characteristics for each subperiod. The first two columns of Table 9 show the results. We find that in both periods, the cyber risk measure is positively related to future stock returns, with the effect slightly stronger in the more recent subperiod.

It is also possible that the firms with high cyber risk based on our measure may over-represent firms from industries that benefit more from digitization, which may, in turn, drive their relatively high performance. To address this concern, we conduct the following analyses. First, to address the concern of potential industry clustering with respect to these variables, we include asset intangibility and R&D expenditures in the Fama-MacBeth regressions as additional controls. The results are presented in Columns (3) to (5) of Table 9, which show a robust relation between cyber risk and future stock returns. Second, for each stock in our sample, we subtract the industry portfolio return from the stock's monthly returns based on the Fama-French 48 industry classifications (Fama and French, 1997) to arrive at the industry-adjusted excess returns. We then perform the Fama-MacBeth cross-sectional regressions with the industry-adjusted return as the dependent variable and our cyber risk measure and other firm characteristics as independent variables. We report the coefficients in Column (6) of Table 9. The results show that cyber risk is positively and significantly correlated with future stock returns even after controlling for industry returns.

It is also possible that firms in the same industry may have similar disclosure language with respect to cyber risk, which may introduce noise to the textual variables. To further examine the robustness of our findings, we conduct the following analysis. We first demean the two textual variables "NIST Counts" and "Risk Factor Length" based on firms' Fama-French 48 industry classifications. Then we repeat the forecasting tests of cyberattacks and the portfolio-based return tests. The results are reported in Table 10.

Panel A shows that the performance of the logistic ridge regression-based cyber risk measure is close to our main measure. Panel B shows a strong relationship between the cyber risk measure based on the industry-adjusted textual variables and future stock returns. These results provide further support for the robustness of our main results.

### 6.2. Cyber Risk and Misconduct

The "Risk Factor" section of firms' 10-K filings covers all material risks that firms deem necessary to report to investors. It is possible that our textual variables "NIST Counts" and "Risk Factor Length" capture other dimensions of corporate risks, such as the risk of corporate misconduct. To address this concern, we examine whether our cyber risk measure predicts future incidents of corporate misconduct.

We obtain data on corporate misconduct from the Violation Tracker, which details the date when the courts determined the penalty for each incident of corporate misconduct. We merge this data set with Compustat data based on firm names. We create a dummy variable Misconduct that equals one if a firm commits misconduct in a fiscal year and zero otherwise. Since misconduct comprises several categories, we further define a dummy variable FinMisconduct that equals one if a firm commits financial misconduct and zero otherwise. Because the dependent variables have binary outcomes, we use logistic regressions, with control variables including size, book-to-market ratio, and corporate culture variables from Li et al. (2021).

The results in Table 11 show that, throughout all specifications, the coefficients for our cyber risk measure are economically small and statistically insignificant, which provides evidence that our cyber risk measure is not driven by the risk of corporate misconduct. It strengthens the notion of cyber risk being an independent source of risk.

### 6.3. Alternative Machine Learning Models

In this subsection, we present the results using alternative machine learning models to estimate ex-ante cyber risk. In particular, we follow Liu et al. (2008), using a combination of undersampling and bootstrapping in an Ensemble method termed "EasyEnsemble" (EEC). The procedure of this method is as follows. In each training window, we randomly sample a subset of non-hacked observations and pair them with the hacked set, which ensures an equal number of non-hacked and hacked firms, thereby constructing a "balanced" sample. We fit an estimator on this sample and save the parameters. We repeat this process 50 times by independently sampling 50 subsets from the non-hacked set. Based on these bootstrapped samples and results, we obtain an ensemble and arrive at a final estimate. Liu et al. (2008) argues that this procedure has superior forecasting performance.

In our setting, we present two additional sets of results using the K-nearest neighbors algorithm and the Naive Bayes algorithm as the base estimators for EEC. We find that the cyber risk measures using the alternative machine learning models also have superior out-of-sample forecasting performance. In Figure 7, We plot the time series of the forecasting performance metrics for the measures based on the logistic regression, logistic ridge regression, EEC-KNN, and EEC-NB techniques. It shows that all three machine learning techniques outperform the simple logistic regression.

Moving to the asset pricing tests, we find that the cyber risk measure based on alternative machine learning techniques also shows a strong relation to future stock returns. For instance, Table 12 presents portfolio performance based on the alternative cyber risk measure. The alpha on the long-short portfolio remains large and statistically significant.

### 6.4. Placebo Test

To address the concern that the relation between our cyber risk measure and future stock returns is driven merely by the correlations between the returns and characteristics of the firms that were exposed to cyberattacks, we design the following placebo test. For each hacked firm in each year, we randomly select a firm from the same Fama-French 48 industry and label it as the "pseudo" attacked firm. We repeat this for all the attacked firms in our sample and thus create a sample of 394 pseudo-attacked firms. With this pseudo sample of hacked firms, we use the same statistical procedure as in our main analyses to estimate a cyber risk measure for each firm. We then test whether the resulting pseudo cyber risk measure (a mechanical combination of stock characteristics) shows a reliable relation to future stock returns. The results from our portfolio tests, as shown in Table 13, indicate that there is no reliable relation between this pseudo cyber risk measure and future stock returns.

### 6.5. Alternative Dictionary

In a contemporaneous study, Jamilov et al. (2020) uses a set of 30 cyber risk-related words and phrases to capture the level of cyber-related concerns expressed by corporate executives during their quarterly earnings conference calls. We evaluate the robustness of our results using this alternative dictionary.

Specifically, we count the number of times a firm uses these cyber-related words and phrases in the Item 1A "Risk Factors" section of the 10-K filings. We replace our original text variable constructed based on the NIST glossary with the new variable. Then we apply the same statistical techniques to estimate our cyber risk measures. The results in the Appendix show a robust relation between these cyber risk measures and future stock returns.

---

## 7. Conclusion

In this paper, we use machine learning algorithms to develop an ex-ante cyber risk measure for individual firms, which has a superior ability to forecast the occurrence of future cyberattacks. We find that firms with higher cyber risk, according to this measure, earn higher average stock returns, which cannot be explained by standard asset pricing models. In times when these firms underperform, cybersecurity experts tend to have higher concerns about cyber risk, and cybersecurity exchange-traded funds outperform. Further evidence based on product market competition and data similarity between firms provides further support to the notion that cyber risk is an important determinant of expected returns in increasingly digitized economies.

Our study suggests interesting avenues for future research. First, we have followed a bottom-up approach to estimate the cyber risk premium, starting with firm-level estimates of cyber risk. Another approach, which is top-down, can examine the systemic impact of a large attack on major players in the economy. For instance, Eisenbach et al. (2020) models how cyber attacks on large banks can influence the financial system and even the economy through network effects. It would be of interest to explore the connections between these two broad approaches.

Second, a limitation of our study is that we focus on the likelihood of cyberattacks as a proxy for cyber risk but do not study the scale of the loss resulting from cyberattacks. Although the probability of cyberattacks is likely to be correlated with the severity of cyberattacks, these two dimensions of cyber risk can contain different information. Our research makes a useful first step toward understanding the implications of cyber risk for asset prices. Future research can benefit from investigating these two dimensions in a unified framework.

---

## Figures

### Figure 1: Disclosed Cyberattack Incidents for US Public Firms
The figure depicts the number of cyberattack incidents that are disclosed for US public firms from 2006 to 2018. The year convention follows Fama and French (1996), which starts from July to next June. The source of data is the Identity Theft Resource Center (ITRC). The black line indicates the number of unique cyberattack incidents matched to Compustat firms; the blue dashed line shows the number of unique public firms that experienced cyberattack incidents each year.

### Figure 2: Industry Distribution of Cyberattacks
The figure depicts the industry distribution of attacked firms based on Fama-French 17 industry classification per Fama and French (1988). The bars show the number of incidents in the sample period in each industry. The hardest hit is the financial industry, with a total of 247 incidents. The least hit is the "Mining and Minerals" industry, which has zero incidents in our sample. The sample runs from 2006 to 2018.

### Figure 3: Out-of-Sample Performance Metrics
The figure depicts the time series of three out-of-sample performance metrics for both logit and logistic ridge regression across the test years. The three metrics are F1 score, G-mean, and Balanced Accuracy. F1-score is the harmonic mean between precision and recall. The geometric mean is the geometric mean between sensitivity and specificity. Balanced accuracy is the arithmetic mean between sensitivity and specificity. The black solid line indicates logit, while the blue dashed line represents logistic ridge. The metrics are all measured against test samples, and thus the figure runs from 2008 to 2018.

### Figure 4: Confusion Matrices
The figure shows the aggregate/mean confusion matrices for logit and logistic ridge regression. That is, we aggregate the numbers in the four quadrants across the 11 test windows for each model. The rows are true classes, while the columns are predicted classes. Each quadrant presents the number of observations that the classification model allocates. The diagonal numbers represent the total number of observations that are correctly allocated to their respective classes. For example, for logit in the left panel, it correctly predicts 1 cyberattack case, while misallocating 376 cases as non-victims. On the other hand, logistic ridge regression in the right panel correctly predicts 184 cyberattack cases, while misallocating 193 cases in the non-victim class.

### Figure 5: Absolute Rank Correlations between Predictors and Cyber Risk
The figure depicts the absolute value of rank correlations between each of the 14 predictor variables and the estimated cyber risk using logistic ridge regression for each test year, as well as the time-series mean of rank correlations for each variable. Specifically, for each test year, we compute the rank correlation between each variable and cyber risk measure, and then take the time-series mean for each variable and put them in the left column of the figure. Then we compute the absolute values of all the rank correlations of all variables across the test years. In so doing, we have 11 sets of coefficients, since the test years run from 2008 to 2018. We plot them in a heat map, as shown in the figure. The color depth represents how large the coefficient is relative to other variables. For example, firm size is consistently important across years, while CAPX/AT has been consistently less important.

### Figure 6: Comovement with ICS and Cybersecurity ETFs & Major Cyberattacks
The figure shows the comovement of the return series of our high-minus-low cyber risk portfolio and that of the ICS beta portfolio, and that of two cybersecurity ETFs. In Panel A, we plot the return series of our high-minus-low cyber risk portfolio and ICS beta portfolio. The ICS beta portfolio is constructed at a monthly frequency by sorting stocks into quintile portfolios based on stocks' return betas with respect to the monthly change of the ICS index, controlling for market excess returns during the past 12 months. The two series have a correlation of -41.2%. In Panel B, we plot the monthly returns of the First Trust Nasdaq Cybersecurity ETF (CIBR) and ETFMG Prime Cyber Security ETF (HACK) from August 2015 to June 2019. The time-series correlation between the returns on the long-short cyber risk portfolio and the ETFs are -47.6% and -41.5% for CIBR and HACK, respectively. In both panels, we also mark the months that major cyberattacks happened, where the major attacks are according to a Bloomberg report. We screen the major attacks to only include public firm attacks during our sample period, which include Yahoo!, Equifax, Under Armor, Facebook, and Quest Diagnostics. Returns and events are plotted at month ends.

### Figure 7: Performance Metrics
The figure depicts the time series of three performance metrics for logit, logistic ridge regression, EasyEnsemble based on KNN (EEC-KNN), and EasyEnsemble based on Naive Bayes (EEC-NB). The three metrics are F1 score, G-mean, and Balanced Accuracy. F1-score is the harmonic mean between precision and recall. Geometric mean is the geometric mean between sensitivity and specificity. Balanced accuracy is the arithmetic mean between sensitivity and specificity. The black solid line indicates logit, the gray dotted line logistic ridge, the red dotted line EEC-KNN, and the light blue dashed line EEC-NB. The metrics are all measured against test samples, and thus the sample runs from 2008 to 2018.

---

## Tables

### Table 1: Summary Statistics
The table presents the summary statistics for key characteristics of both hacked firms and non-hacked firms. There are in total 37,481 firm-year pairs, with 552 cyberattack cases, during the period 2006–2018. We show the mean, standard deviation, 25th percentile, and 75th percentile for each group, and present them side by side for comparison. Hacked firms are denoted as Hacked = 1, while zero indicates non-hacked firms. The variables are defined in the Appendix. Risk Factor Length is the number of tokens in a firm's 10-K Item 1A. NIST Term Counts is the number of times a firm mentions cybersecurity terms per NIST dictionary in its Item 1A in 10-K.

| Variable | Hacked | Mean | STD | P25 | P75 |
|----------|--------|------|-----|-----|-----|
| Intangibility | 0 | 0.79 | 0.23 | 0.70 | 0.97 |
| | 1 | 0.82 | 0.21 | 0.74 | 0.97 |
| CAPX/AT | 0 | 0.04 | 0.06 | 0.01 | 0.05 |
| | 1 | 0.03 | 0.04 | 0.01 | 0.05 |
| CF/AT | 0 | 0.02 | 0.22 | 0.01 | 0.11 |
| | 1 | 0.07 | 0.09 | 0.02 | 0.12 |
| Firm Size | 0 | 6.68 | 2.03 | 5.26 | 8.02 |
| | 1 | 9.22 | 2.30 | 7.56 | 10.99 |
| Net Worth | 0 | 0.45 | 0.25 | 0.25 | 0.66 |
| | 1 | 0.37 | 0.21 | 0.18 | 0.51 |
| R&D | 0 | 0.05 | 0.12 | 0.00 | 0.04 |
| | 1 | 0.02 | 0.06 | 0.00 | 0.01 |
| ROA | 0 | -0.02 | 0.23 | -0.01 | 0.07 |
| | 1 | 0.04 | 0.09 | 0.01 | 0.07 |
| Tobin's Q | 0 | 1.86 | 1.55 | 1.05 | 2.06 |
| | 1 | 1.86 | 1.19 | 1.09 | 2.10 |
| Sales Growth | 0 | 1.56 | 22.94 | 0.97 | 1.18 |
| | 1 | 1.10 | 0.23 | 1.00 | 1.13 |
| Financial Constraint | 0 | -0.27 | 0.81 | -0.33 | -0.18 |
| | 1 | -0.38 | 0.12 | -0.47 | -0.29 |
| Annual Exret | 0 | 0.01 | 0.52 | -0.25 | 0.18 |
| | 1 | 0.03 | 0.31 | -0.16 | 0.19 |
| Log(age) | 0 | 2.11 | 0.62 | 1.79 | 2.56 |
| | 1 | 2.26 | 0.60 | 1.95 | 2.71 |
| Risk Factor Length | 0 | 7,191 | 5,288 | 3,668 | 9,299 |
| | 1 | 8,710 | 6,422 | 4,304 | 12,019 |
| NIST Counts | 0 | 95 | 71 | 48 | 122 |
| | 1 | 135 | 96 | 66 | 178 |

### Table 2: Performance Metrics
This table reports the time-series mean out-of-sample performance metrics across the recursive windows for logit and logistic ridge. F1-score is the harmonic mean between precision and recall. The geometric mean is the geometric mean between sensitivity and specificity. Balanced accuracy is the arithmetic mean between sensitivity and specificity. Each recursive window contains n + 1 years of data, with n ∈ [1, 10] as the training data and +1 the subsequent year as the test data. There are in total 11 windows, starting at the year 2007 as the training data and 2008 as the test data. The final window consists of the years 2007 - 2017 as the training data and 2018 as the test data. The first two rows are the means of each corresponding metric for 11 windows. The third row represents the mean difference between the logistic ridge and logit, and the fourth row computes the standard error of the difference in means.

| Metrics | F1-score: Harmonic Mean | G-mean: Geometric Mean | Balanced Accuracy |
|---------|-------------------------|------------------------|-------------------|
| Logit | 0.004 | 0.014 | 0.501 |
| Logistic Ridge | 0.063 | 0.599 | 0.650 |
| Logistic Ridge - Logit | 0.059*** | 0.584*** | 0.149*** |
| | (0.010) | (0.043) | (0.022) |

*Note: ∗p<0.1; ∗∗p<0.05; ∗∗∗p<0.01*

### Table 3: Fama-MacBeth Cross-sectional Regressions
This table reports Fama-MacBeth cross-sectional regressions of returns on firm characteristics and anomaly variables. For each month, we run cross-sectional regression of stock returns on firm characteristics, and then we average the coefficients across time series. The sample runs from July 2008 to June 2019. Column (1) includes the natural log of market cap, the natural log of book-to-market ratio, gross profitability, asset growth, and momentum. Column (2) replaces our cyber risk measure with Cyber Cosine (Florackis et al., 2023). Column (3) adds back our cyber risk measure. Column (4) further includes the past one-month return to control for the short-term return reversal, idiosyncratic volatility (Ang et al., 2006), and illiquidity (Amihud, 2002). Standard errors are Newey-West standard errors with 6 lags and are reported in parentheses. Returns are measured as percentages, and all independent variables are cross-sectionally winsorized at [1%,99%] level and standardized to have zero mean and standard deviation of unity.

| Variable | (1) | (2) | (3) | (4) |
|----------|-----|-----|-----|-----|
| Cyber Risk | 0.197*** | | 0.186*** | 0.148** |
| | (0.067) | | (0.064) | (0.063) |
| Cyber Cosine | | 0.132*** | 0.093** | 0.100** |
| | | (0.049) | (0.043) | (0.043) |
| Log(MktCap) | -0.127 | -0.006 | -0.133 | -0.159 |
| | (0.158) | (0.139) | (0.152) | (0.128) |
| B/M | 0.163 | 0.204 | 0.160 | 0.087 |
| | (0.148) | (0.143) | (0.149) | (0.150) |
| GP | 0.098 | 0.155 | 0.103 | 0.081 |
| | (0.108) | (0.112) | (0.107) | (0.100) |
| ATG | -0.247*** | -0.225*** | -0.249*** | -0.244*** |
| | (0.055) | (0.058) | (0.055) | (0.056) |
| MOM | -0.089 | -0.081 | -0.091 | -0.119 |
| | (0.181) | (0.183) | (0.182) | (0.188) |
| ST Rev | | | | -0.345*** |
| | | | | (0.107) |
| IdioRisk | | | | -0.226 |
| | | | | (0.146) |
| Illiquidity | | | | 0.134 |
| | | | | (0.111) |
| Observations | 289,696 | 310,243 | 275,301 | 275,301 |
| R-squared | 0.031 | 0.030 | 0.032 | 0.046 |

*Note: ∗p<0.1; ∗∗p<0.05; ∗∗∗p<0.01*

### Table 4: Portfolio Analyses
This table provides various portfolio analyses for the universe of stocks sorted on predicted ex-ante cyberattack probabilities. The prediction model used here is the logistic ridge regression. At the end of each June from 2008 to 2018, we sort stocks into three tercile portfolios, four quartile portfolios, and five quintile portfolios according to the estimated cyber risk measure. These portfolios are held until the end of June in year t+1 and then rebalanced based on the updated cyber risk estimate when new information is available. We create zero-cost hedge portfolios that buy high cyber-risk stocks and short low cyber-risk stocks. We compute the monthly equal- and value-weighted alpha on the hedge portfolios using a number of asset pricing models: the CAPM, Fama-French three-factor model (FF3), FF3 augmented by a momentum factor (FF4), Fama-French five-factor model (FF5), and FF5 augmented with a momentum factor (FF6). The left half panel reports value-weighted results, while the right half panel reports equal-weighted results. Standard errors are Newey-West standard errors with 6 lags and are included in parentheses.

| Model | Value-Weighted | | | Equal-Weighted | | |
|-------|----------------|---|---|----------------|---|---|
| | Tercile | Quartile | Quintile | Tercile | Quartile | Quintile |
| CAPM | 0.574*** | 0.765*** | 0.843*** | 0.508*** | 0.645*** | 0.713*** |
| | (0.176) | (0.207) | (0.227) | (0.154) | (0.171) | (0.180) |
| FF3 | 0.458*** | 0.658*** | 0.739*** | 0.437*** | 0.581*** | 0.657*** |
| | (0.122) | (0.190) | (0.219) | (0.131) | (0.154) | (0.157) |
| FF4 | 0.461*** | 0.660*** | 0.742*** | 0.433*** | 0.577*** | 0.653*** |
| | (0.127) | (0.193) | (0.226) | (0.121) | (0.141) | (0.150) |
| FF5 | 0.431*** | 0.536*** | 0.577*** | 0.425*** | 0.541*** | 0.616*** |
| | (0.116) | (0.157) | (0.179) | (0.138) | (0.160) | (0.165) |
| FF6 | 0.438*** | 0.540*** | 0.585*** | 0.419*** | 0.533*** | 0.611*** |
| | (0.124) | (0.161) | (0.190) | (0.131) | (0.151) | (0.163) |

*Note: ∗p<0.1; ∗∗p<0.05; ∗∗∗p<0.01*

### Table 5: Cybersecurity ETFs: Top 10 Holdings
This table presents the top ten holdings of two cybersecurity ETFs, respectively: First Trust Nasdaq Cybersecurity ETF (CIBR) and ETFMG Prime Cyber Security ETF (HACK). The holdings are as of February 2021.

| CIBR | Weight | HACK | Weight |
|------|--------|------|--------|
| CrowdStrike Holdings, Inc. (Class A) | 7.49% | Blackberry Ltd. | 3.57% |
| Zscaler, Inc. | 7.08% | Cisco Sys Inc. | 3.13% |
| Cisco Systems, Inc. | 5.60% | Palo Alto Networks Inc. | 2.81% |
| Accenture Plc | 5.25% | Cyberark Software Ltd. | 2.80% |
| Splunk Inc. | 4.41% | Ping Identity Hldg Corp | 2.77% |
| FireEye, Inc. | 3.41% | FireEye Inc. | 2.76% |
| Palo Alto Networks, Inc. | 3.38% | Sumo Logic Inc. | 2.71% |
| Proofpoint, Inc. | 3.28% | Commvault Systems Inc. | 2.69% |
| SailPoint Technologies Holdings, Inc. | 3.27% | Cloudflare Inc. | 2.64% |
| Fortinet, Inc. | 3.22% | Qualys Inc. | 2.64% |

### Table 6: Stock Price Reaction of Peer Firms to Cyberattacks and Industry Competition
This table examines how industry competition influences the stock market reaction of peer firms to cyberattacks on target firms. Peer firms are defined as those in the same Fama-French 48 industry (Fama and French, 1997) as the hacked firms that experienced a cyberattack. We select only those cyberattack incidents when hacked firms experienced lower than -1% CAR around the [-3,+3] window, consistent with the screening criteria used in our main results. The CAR is defined as the cumulative daily abnormal returns based on the Fama-French three-factor model augmented by the momentum factor, with an estimation window of 100 days. We require a minimum number of valid returns of 70 days in the estimation window, and a gap of 50 days between the end of the estimation window and the beginning of the event window. Victim CAR is the [-3,+3] window cumulative abnormal return of the focal firm around cyberattack events. Peer CAR is the [-3,+3] window cumulative abnormal return of the peer firm around cyberattack events. "Strong Victim" is a dummy variable if the peer firm's sales are lower than the hacked firm in the previous year or zero otherwise. Industry and year-fixed effects are included. Standard errors are clustered at the industry and event levels.

| Variable | (1) | (2) | (3) |
|----------|-----|-----|-----|
| Victim CAR | 0.046*** | 0.046*** | 0.051*** |
| | (0.015) | (0.015) | (0.013) |
| Strong Victim | | -0.000 | 0.001 |
| | | (0.002) | (0.002) |
| Victim CAR × Strong Victim | | | 0.025*** |
| | | | (0.008) |
| Size | -0.001 | -0.001 | -0.001 |
| | (0.001) | (0.001) | (0.001) |
| B/M | -0.001 | -0.001 | -0.001 |
| | (0.001) | (0.001) | (0.001) |
| Constant | 0.002 | 0.002 | 0.002 |
| | (0.005) | (0.006) | (0.006) |
| Observations | 57,194 | 57,194 | 57,194 |
| R-squared | 0.008 | 0.008 | 0.008 |
| Industry & Year FE | YES | YES | YES |
| Industry & Event Cluster | YES | YES | YES |

*Note: ∗p<0.1; ∗∗p<0.05; ∗∗∗p<0.01*

### Table 7: Stock Price Reaction of Firms with Data Similarity to Cyberattacks
This table uses product similarity as a proxy for data similarity to study the impact of cyberattacks on firms with similar data holdings. First, we identify firms in the same Fama-French 48 industry (Fama and French, 1997) as the hacked firms that experienced a cyberattack. Then we use the product similarity score from Hoberg and Philips (2016) as our proxy for data similarity between two firms. Other variables are as defined in Table 6. Industry and year-fixed effects are included. Standard errors are clustered at the industry and event levels.

| Variable | (1) | (2) | (3) |
|----------|-----|-----|-----|
| Victim CAR | 0.046*** | 0.049*** | 0.038** |
| | (0.015) | (0.017) | (0.016) |
| Data Similarity | | -0.055*** | -0.011 |
| | | (0.010) | (0.009) |
| Victim CAR × Data Similarity | | | 0.820*** |
| | | | (0.237) |
| Size | -0.001 | -0.001 | -0.001 |
| | (0.001) | (0.001) | (0.001) |
| B/M | -0.001 | -0.000 | -0.001 |
| | (0.001) | (0.001) | (0.001) |
| Constant | 0.002 | 0.003 | 0.003 |
| | (0.005) | (0.005) | (0.005) |
| Observations | 57,191 | 57,191 | 57,191 |
| R-squared | 0.008 | 0.008 | 0.009 |
| Industry & Year FE | YES | YES | YES |
| Industry & Event Cluster | YES | YES | YES |

*Note: ∗p<0.1; ∗∗p<0.05; ∗∗∗p<0.01*

### Table 8: Cyber Risk and Data Similarity
This table presents the results of regressing our cyber risk measure and the Cyber Cosine measure from Florackis et al. (2023) on the composite data similarity measure in the previous year. We construct the "Composite Data Sim" variable as follows:

CompositeDataSim_{i,t} = (1/m) ∑_{j=1}^m DataSim_{i,j,t}

where i represents firms in the Compustat universe, j indexes firms that have been attacked in year t, and DataSim is the product similarity score measure in Hoberg and Philips (2016). In Columns (2) and (4), we control for size and book-to-market ratio. Every continuous variable is standardized to have a mean of zero and a standard deviation of one. We include industry (Fama and French 48-industry classification) fixed effects and year fixed effects. Standard errors are clustered at the industry level.

| Variable | (1) | (2) | (3) | (4) |
|----------|-----|-----|-----|-----|
| | Cyber Risk | | Cyber Cosine | |
| Composite Data Sim | 0.028*** | 0.012*** | 0.061*** | 0.038*** |
| | (0.007) | (0.004) | (0.016) | (0.010) |
| Log(MktCap) | | 0.137*** | | 0.200*** |
| | | (0.003) | | (0.013) |
| B/M | | 0.021*** | | -0.013 |
| | | (0.002) | | (0.011) |
| Constant | 0.000*** | -0.013*** | 0.042*** | 0.024*** |
| | (0.000) | (0.000) | (0.000) | (0.001) |
| Observations | 31,106 | 31,084 | 29,797 | 29,776 |
| R-squared | 0.872 | 0.887 | 0.470 | 0.506 |
| Industry FE | YES | YES | YES | YES |
| Year FE | YES | YES | YES | YES |

*Note: ∗p<0.1; ∗∗p<0.05; ∗∗∗p<0.01*

### Table 9: Sub-sample Analysis and Industry Effects
This table reports sub-sample analysis and industry analysis via Fama-MacBeth cross-sectional regressions. In the first two columns, we split our sample into two sub-periods, from July 2008 to December 2013 and from January 2014 to June 2019. We regress monthly stock returns on the common stock characteristics, including natural log of market cap, natural log of book-to-market ratio, gross profitability, asset growth, and momentum, and report the time-series means of the coefficients for the two sub-periods in Columns (1) and (2) separately. In Columns (3) to (5), we include intangibility and/or R&D in the regressions as additional controls since there could be industry clustering with respect to these variables, depending on how data-reliant the industry is. In the sixth column, we conduct industry analysis to see whether our results are driven by industry returns. In each month in our sample, we subtract Fama-French 48 industry (Fama and French, 1997) portfolio returns from stock returns to arrive at the industry-adjusted excess returns. Then we conduct Fama-MacBeth regressions using the adjusted returns on stock characteristics and report the time-series means in Column (6). Standard errors are Newey-West standard errors with 6 lags and are reported in parentheses. Returns are measured as percentages, and all independent variables are cross-sectionally winsorized at [1%,99%] level and standardized to have zero mean and standard deviation of unity.

| Variable | (1) | (2) | (3) | (4) | (5) | (6) |
|----------|-----|-----|-----|-----|-----|-----|
| | 2008/07-2013/12 | 2014/01-2019/06 | | | | FF48-Ind Adj Returns |
| Cyber Risk | 0.180* | 0.214** | 0.144** | 0.228*** | 0.173** | 0.145*** |
| | (0.095) | (0.094) | (0.072) | (0.074) | (0.080) | (0.054) |
| Log(MktCap) | -0.298 | 0.044 | -0.037 | -0.075 | -0.017 | -0.058 |
| | (0.254) | (0.176) | (0.163) | (0.142) | (0.153) | (0.147) |
| B/M | 0.363* | -0.037 | 0.226* | 0.252 | 0.279* | 0.205 |
| | (0.212) | (0.191) | (0.134) | (0.156) | (0.151) | (0.129) |
| GP | 0.053 | 0.144 | 0.079 | 0.166 | 0.136 | 0.047 |
| | (0.102) | (0.191) | (0.109) | (0.105) | (0.104) | (0.104) |
| ATG | -0.334*** | -0.160** | -0.256*** | -0.232*** | -0.244*** | -0.205*** |
| | (0.070) | (0.076) | (0.053) | (0.052) | (0.051) | (0.043) |
| MOM | -0.223 | 0.046 | -0.076 | -0.057 | -0.057 | -0.117 |
| | (0.326) | (0.147) | (0.179) | (0.177) | (0.175) | (0.167) |
| Intangibility | | | 0.225** | | 0.176* | |
| | | | (0.095) | | (0.093) | |
| R&D | | | | 0.199* | 0.140 | |
| | | | | (0.103) | (0.101) | |
| Constant | 1.669 | 0.563 | 1.145* | 1.094* | 1.123* | 0.113 |
| | (1.157) | (0.577) | (0.651) | (0.652) | (0.645) | (0.288) |
| Observations | 153,509 | 136,187 | 289,696 | 289,696 | 289,696 | 276,025 |
| R-squared | 0.026 | 0.035 | 0.035 | 0.035 | 0.039 | 0.026 |

*Note: ∗p<0.1; ∗∗p<0.05; ∗∗∗p<0.01*

### Table 10: Cyber Risk Based on Industry-Adjusted Textual Variables
This table reports the performance metrics and portfolio results when we generate cyber risk measures using industry-adjusted (subtracting the industry average) textual variables. All the accounting variables remain unchanged, while the two textual variables "NIST Counts" and "Risk Factor Length" are demeaned according to each firm's Fama-French 48-industry classification (Fama and French, 1997). Panel A follows Table 2 and Panel B Table 4.

**Panel A: Prediction Performance Metrics**

| Metrics | F1-score: Harmonic Mean | G-mean: Geometric Mean | Balanced Accuracy |
|---------|-------------------------|------------------------|-------------------|
| Logit | 0.000 | 0.000 | 0.500 |
| Logistic Ridge | 0.089 | 0.478 | 0.625 |

**Panel B: Long-Short Portfolio Alphas**

| Model | Value-Weighted | | | Equal-Weighted | | |
|-------|----------------|---|---|----------------|---|---|
| | Tercile | Quartile | Quintile | Tercile | Quartile | Quintile |
| CAPM | 0.502** | 0.664*** | 0.720*** | 0.583*** | 0.672*** | 0.805*** |
| | (0.203) | (0.231) | (0.245) | (0.176) | (0.202) | (0.216) |
| FF3 | 0.456*** | 0.629*** | 0.693*** | 0.561*** | 0.660*** | 0.803*** |
| | (0.157) | (0.187) | (0.200) | (0.157) | (0.173) | (0.184) |
| FF4 | 0.458*** | 0.634*** | 0.696*** | 0.557*** | 0.657*** | 0.800*** |
| | (0.163) | (0.198) | (0.208) | (0.141) | (0.163) | (0.174) |
| FF5 | 0.271* | 0.425*** | 0.451*** | 0.439*** | 0.526*** | 0.652*** |
| | (0.145) | (0.161) | (0.167) | (0.160) | (0.185) | (0.202) |
| FF6 | 0.275* | 0.435** | 0.459*** | 0.430*** | 0.520*** | 0.646*** |
| | (0.149) | (0.170) | (0.173) | (0.150) | (0.179) | (0.196) |

*Note: ∗p<0.1; ∗∗p<0.05; ∗∗∗p<0.01*

### Table 11: Cyber Risk and Corporate Misconduct
This table examines whether our cyber risk measure is related to future incidents of corporate misconduct, to address the concern that our cyber risk measure is driven by other sources of corporate risk. Data on corporate misconduct come from the Violation Tracker, which are merged with data from Compustat. We create a dummy variable Misconduct that equals one if a firm commits misconduct in a fiscal year and zero otherwise. Since corporate misconduct comprises several categories, we further define a dummy variable FinMisconduct that equals one if a firm commits financial misconduct and zero otherwise. Because the dependable variables have binary outcomes, we use logistic regressions, with control variables including size, book-to-market ratio, and corporate culture variables from Li et al. (2021). Industry and year-fixed effects are included. Standard errors are clustered at the industry level.

| Variable | (1) | (2) | (3) | (4) |
|----------|-----|-----|-----|-----|
| | Misconduct | | FinMisconduct | |
| Cyber Risk | 0.017 | -0.175 | 3.267 | 2.508 |
| | (0.532) | (0.653) | (3.101) | (5.953) |
| Log(MktCap) | 0.566*** | 0.590*** | 0.612*** | 0.721*** |
| | (0.041) | (0.041) | (0.083) | (0.104) |
| B/M | 0.339*** | 0.370*** | 0.621*** | 0.531** |
| | (0.066) | (0.073) | (0.159) | (0.225) |
| Integrity | | 0.184 | | -0.453 |
| | | (0.124) | | (0.552) |
| Teamwork | | -0.261** | | -0.429 |
| | | (0.119) | | (0.513) |
| Innovation | | -0.193*** | | 0.137 |
| | | (0.068) | | (0.287) |
| Respect | | 0.108* | | -0.379** |
| | | (0.063) | | (0.175) |
| Quality | | -0.013 | | -0.141 |
| | | (0.084) | | (0.293) |
| Constant | -14.171*** | -14.698*** | -19.786*** | -21.823*** |
| | (0.903) | (0.918) | (1.577) | (2.232) |
| Observations | 31,055 | 22,856 | 21,193 | 14,431 |
| Pseudo R2 | 0.188 | 0.178 | 0.186 | 0.251 |
| Industry FE | YES | YES | YES | YES |
| Year FE | YES | YES | YES | YES |

*Note: ∗p<0.1; ∗∗p<0.05; ∗∗∗p<0.01*

### Table 12: Portfolio Analyses on Ensemble-based Cyber Risk
This table provides portfolio analyses by using cyber risk estimated by EasyEnsemble methods using K-nearest neighbors and Naive Bayes. We show portfolio high-minus-low alpha results in terciles, quartiles, and quintiles, from both EEC-KNN and EEC-NB. These are benchmarked to various asset pricing models, including CAPM, Fama-French three-factor model (FF3), FF3 augmented by a momentum factor (FF4), Fama-French five-factor model (FF5), and FF5 augmented with a momentum factor (FF6). The left half panel reports results from using EEC-KNN generated cyber risk, while the right half panel reports results from using EEC-NB generated cyber risk. Standard errors are Newey-West standard errors with 6 lags and are included in parentheses.

| Model | EEC-KNN | | | EEC-NB | | |
|-------|----------|---|---|--------|---|---|
| | Tercile | Quartile | Quintile | Tercile | Quartile | Quintile |
| CAPM | 0.467*** | 0.556*** | 0.489*** | 0.509*** | 0.711*** | 0.984*** |
| | (0.164) | (0.198) | (0.204) | (0.262) | (0.267) | (0.273) |
| FF3 | 0.366*** | 0.446*** | 0.381*** | 0.606*** | 0.812*** | 1.058*** |
| | (0.091) | (0.088) | (0.099) | (0.228) | (0.209) | (0.228) |
| FF4 | 0.369*** | 0.449*** | 0.385*** | 0.616*** | 0.824*** | 1.072*** |
| | (0.094) | (0.091) | (0.102) | (0.239) | (0.219) | (0.252) |
| FF5 | 0.270*** | 0.335*** | 0.239** | 0.355** | 0.537*** | 0.744*** |
| | (0.083) | (0.092) | (0.099) | (0.179) | (0.157) | (0.162) |
| FF6 | 0.276*** | 0.342*** | 0.246** | 0.372** | 0.559*** | 0.770*** |
| | (0.085) | (0.094) | (0.101) | (0.182) | (0.160) | (0.176) |

*Note: ∗p<0.1; ∗∗p<0.05; ∗∗∗p<0.01*

### Table 13: Placebo "Pseudo-Cyber-Risk" Portfolio High-Minus-Low Alphas
This table reports the placebo portfolio high-minus-low alphas. First, for each hacked firm in each year, we randomly sample a firm from the same Fama-French 48 industry and label it as the "pseudo" attacked firm; we do this for all the attacked firms in our sample, and thus we have 394 "pseudo" attacked firms. We follow the same prediction procedure as in our main results (logistic ridge regression), but on the sample of these "pseudo" attacked firms, and generate a "pseudo" cyber risk measure for each firm. We finally test whether, by using this "pseudo" measure, we can find significant high-minus-low portfolio alphas. We perform these tests on terciles, quartiles, and quintile sorts based on this pseudo measure, and then regress the resulting monthly return series on various empirical asset pricing factors. Standard errors are adjusted with the Newey-West procedure with 6 lags and are included in parentheses.

| Model | Tercile | Quartile | Quintile |
|-------|---------|----------|----------|
| CAPM | -0.130 | -0.198 | -0.210 |
| | (0.216) | (0.286) | (0.325) |
| FF3 | -0.162 | -0.227 | -0.273 |
| | (0.242) | (0.316) | (0.350) |
| FF4 | -0.161 | -0.225 | -0.272 |
| | (0.243) | (0.317) | (0.351) |
| FF5 | -0.212 | -0.293 | -0.344 |
| | (0.229) | (0.297) | (0.334) |
| FF6 | -0.214 | -0.293 | -0.347 |
| | (0.230) | (0.299) | (0.335) |

*Note: ∗p<0.1; ∗∗p<0.05; ∗∗∗p<0.01*

---

## Appendix A. Selected Variable Definitions

**ATG** = asset growth over the previous year

**Book Value of Equity** = SEQ + TXDITC − Preferred, preferred is PSTKRV, or PSTKL, or PSTK, whichever is first available.

**Balanced Accuracy** = (sensitivity+specificity)/2

**CAPX/AT** = CAPX/AT

**CF/AT** = (IB + DP)/AT

**Cyber Cosine** = cybersecurity risk measure defined in Florackis et al. (2023)

**Cyber Risk** = predicted one-year ahead probability of suffering cyberattack events

**Financial Constraint** = −0.091 × CF/AT − 0.062 × DIVPOS + 0.021 × TLTD − 0.044 × Firm Size + 0.102 × SIC − 3digit − industry − growth − 0.035 × Sale Growth (Whited and Wu (2006))

**Firm Size** = natural log of firm's total assets

**F1 − score** = 2(precision × recall)/(precision + recall)

**G − mean** = √(sensitivity × specificity)

**GP** = gross profitability, equals (REVT − COGS)/AT

**Illiquidity** = monthly mean of absolute daily return over price times volume of that day, see Amihud (2002).

**Intangibility** = 1 − PPENT/AT

**Net Worth** = SEQ/AT

**R&D** = max of XRD/AT or zero divided by total assets

**ROA** = NI/AT

**Tobin's Q** = (AT − CEQ + PRCC_F × CSHO)/AT

---

## Appendix B. In-sample Logit

This section provides detailed results for the in-sample logit produced in Section 3. The results are shown in Table A.1.

As expected and consistent with findings in Kamiya et al. (2021), larger firms (as measured by the natural log of the firm's total assets), firms with more intangible assets, higher cash flows, more growth potential (measured by Tobin's q), and firms that face more financial constraints (measured according to Whited and Wu (2006)), are more likely targets of cyber attacks next year. On the other hand, firms with low returns on assets are more likely targets.

---

## References

Amihud, Y., 2002. Illiquidity and stock returns: cross-section and time-series effects. Journal of Financial Markets 5, 31–56.

Ang, A., Hodrick, R. J., Xing, Y., Zhang, X., 2006. The Cross-Section of Volatility and Expected Returns. The Journal of Finance 61, 259–299.

Binfarè, M., 2019. The Real Effects of Risk Management Vulnerabilities: Evidence from Data Breaches. Available at SSRN 3411553.

Brodersen, K. H., Ong, C. S., Stephan, K. E., Buhmann, J. M., 2010. The balanced accuracy and its posterior distribution. In: 2010 20th international conference on pattern recognition, IEEE, pp. 3121–3124.

Chen, L., Pelger, M., Zhu, J., 2023. Deep learning in asset pricing. Management Science, forthcoming.

Cong, L. W., Feng, G., He, J., He, X., 2023a. Asset pricing with panel tree under global split criteria. Tech. rep., National Bureau of Economic Research.

Cong, L. W., Harvey, C. R., Rabetti, D., Wu, Z.-Y., 2023b. An anatomy of crypto-enabled cybercrimes. Tech. rep., National Bureau of Economic Research.

Cong, L. W., Tang, K., Wang, J., Zhang, Y., 2021. Alphaportfolio: Direct construction through deep reinforcement learning and interpretable AI. Available at SSRN 3554486.

Damashek, M., 1995. Gauging Similarity with n-Grams: Language-Independent categorization of text. Science 267, 843–848.

Duffie, D., Younger, J., 2019. Cyber runs. Hutchins Center Working Paper.

Eisenbach, T. M., Kovner, A., Lee, M. J., 2020. Cyber risk and the us financial system: A pre-mortem analysis. FRB of New York Staff Report.

Fama, E. F., French, K. R., 1988. Permanent and temporary components of stock prices. Journal of Political Economy 96, 246–273.

Fama, E. F., French, K. R., 1996. Multifactor explanations of asset pricing anomalies. The Journal of Finance 51, 55–84.

Fama, E. F., French, K. R., 1997. Industry costs of equity. Journal of Financial Economics 43, 153–193.

Fama, E. F., MacBeth, J. D., 1973. Risk, return, and equilibrium: empirical tests. Journal of Political Economy 81, 607–636.

Florackis, C., Louca, C., Michaely, R., Weber, M., 2023. Cybersecurity risk. The Review of Financial Studies 36, 351–407.

Freyberger, J., Neuhierl, A., Weber, M., 2020. Dissecting characteristics nonparametrically. The Review of Financial Studies 33, 2326–2377.

Gu, S., Kelly, B., Xiu, D., 2020. Empirical asset pricing via machine learning. The Review of Financial Studies 33, 2223–2273.

Hastie, T., Tibshirani, R., Friedman, J., 2017. The Elements of statistical learning. Springer Science+Business Media New York.

He, H., Garcia, E. A., 2009. Learning from imbalanced data. IEEE Transactions on knowledge and data engineering 21, 1263–1284.

Hoberg, G., Philips, G. M., 2016. Text-based network industries and endogenous product differentiation. Journal of Political Economy 124, 1423–1465.

Jamilov, R., Rey, H., Tahoun, A., 2020. The Anatomy of Cyber Risk. London Business School Working Paper.

Kamiya, S., Kang, J.-K., Kim, J., Milidonis, A., Stulz, R. M., 2021. Risk management, firm reputation, and the impact of successful cyberattacks on target firms. Journal of Financial Economics 139, 719–749.

Kashyap, A. K., Wetherilt, A., 2019. Some Principles for Regulating Cyber Risk. AEA Papers and Proceedings 109, 482–487.

Kelly, B. T., Pruitt, S., Su, Y., 2019. Characteristics are covariances: A unified model of risk and return. Journal of Financial Economics 134, 501–524.

King, G., Zeng, L., 2001. Logistic regression in rare events data. Political Analysis 9, 137–163.

Kopp, E., Kaffenberger, L., Jenkinson, N., 2017. Cyber risk, market failures, and financial stability. International Monetary Fund.

Kozak, S., Nagel, S., Santosh, S., 2020. Shrinking the cross-section. Journal of Financial Economics 135, 271–292.

Li, K., Mai, F., Shen, R., Yan, X., 2021. Measuring corporate culture using machine learning. The Review of Financial Studies 34, 3265–3315.

Lin, Z., Sapp, T. R., Ulmer, J. R., Parsa, R., 2020. Insider trading ahead of cyber breach announcements. Journal of Financial Markets 50, 100527.

Liu, X.-Y., Wu, J., Zhou, Z.-H., 2008. Exploratory undersampling for class-imbalance learning. IEEE Transactions on Systems, Man, and Cybernetics, Part B (Cybernetics) 39, 539–550.

Michel, A., Oded, J., Shaked, I., 2020. Do security breaches matter? The shareholder puzzle. European Financial Management 26, 288–315.

Newey, W. K., West, K. D., 1987. A simple, positive semi-definite, heteroskedasticity and autocorrelation consistent covariance matrix. Econometrica 55, 703–708.

Petersen, M. A., 2009. Estimating standard errors in finance panel data sets: Comparing approaches. The Review of Financial Studies 22, 435–480.

Schütze, H., Manning, C. D., Raghavan, P., 2008. Introduction to information retrieval, vol. 39. Cambridge University Press Cambridge.

Warren, P., Kaivanto, K., Prince, D., et al., 2018. Could a cyber attack cause a systemic impact in the financial sector? Bank of England Quarterly Bulletin 58, 21–30.

Whited, T. M., Wu, G., 2006. Financial constraints risk. The Review of Financial Studies 19, 531–559.

Yue, Y., Finley, T., Radlinski, F., Joachims, T., 2007. A support vector method for optimizing average precision. In: Proceedings of the 30th annual international ACM SIGIR conference on Research and development in information retrieval, pp. 271–278.

Zeng, X., Martinez, T. R., 2000. Distribution-balanced stratified cross-validation for accuracy estimation. Journal of Experimental & Theoretical Artificial Intelligence 12, 1–12.

---

**Footnotes:**

¹ See Kashyap and Wetherilt (2019) for discussions on the distinguishing features of cyber risk.

² The EasyEnsemble technique combines undersampling and bootstrapping, which is effective in dealing with class-imbalance problems. This technique is particularly suited to address issues like cyberattacks, which represent rare events in the data. See Section 6.3 for relevant technical details on the EasyEnsemble technique.

³ In another study, Michel et al. (2020) study the timing of cyberattack announcements. They find negative abnormal returns on hacked firms prior to the announcement of the attacks, which is consistent with some information leakage. Echoing this message, Lin et al. (2020) reports evidence of insider trading ahead of public announcements of cyberattacks. Binfarè (2019) studies the effect of data breaches on the cost of debt financing. He finds that lenders tend to charge borrowing firms larger spreads after they experience data breaches.

⁴ Kopp et al. (2017) and Warren et al. (2018) examine the impact of cyberattacks on financial institutions and financial market infrastructure, and argue such attacks potentially can be quite damaging. Duffie and Younger (2019) study the linkage between the cyber security of large banks and financial stability. They argue that large banks tend to have sufficient liquidity to weather relatively extreme cyber runs; however, severe cyberattacks may deter nonbanks from sending funds through these institutions, which could create systemic risk.

⁵ ITRC, https://www.idtheftcenter.org/. On their website: "The ITRC is a non-profit organization established to support victims of identity theft in resolving their cases, and to broaden public education and awareness in the understanding of identity theft, data breaches, cyber security, scams/fraud, and privacy issues." See this SEC report that cites the data from ITRC: https://www.sec.gov/files/speech-jackson-cybersecurity-2018-03-15-data-appendix-updated.pdf.

⁶ Privacy Rights Clearinghouse, 2019, https://www.privacyrights.org/data-breaches.

⁷ This increases our data set from the 311 observations from PRC, which is nearly a 3-fold increase.

⁸ We drop the first 6 months of the calendar year 2006 and the last 6 months of the year 2019, as they do not constitute a whole year per our definition.

⁹ French, Kenneth, 2019, http://mba.tuck.dartmouth.edu/pages/faculty/ken.french/data_library.html.

¹⁰ McDonald, Bill, University of Notre Dame, https://sraf.nd.edu/data/stage-one-10-x-parse-data/.

¹¹ Northbridge Insurance, 2019, https://www.nbins.com/blog/cyber-risk/what-is-cyber-risk-2/.

¹² See SEC, 2005, https://www.sec.gov/rules/final/33-8591.pdf.

¹³ NIST, April 25, 2006, https://www.nist.gov/publications/glossary-key-information-security-terms.

¹⁴ A contemporaneous study by Jamilov et al. (2020) uses a dictionary with a different set of words and phrases. We show in Section 6 that our results are robust to using alternative dictionaries.

¹⁵ We use an algorithm to match the section between the beginning of Section 1A and either Section 1B or Section 2.

¹⁶ A token is an instance of a sequence of characters in some particular document that is grouped together as a useful semantic unit for processing (Schütze et al. (2008)). Here we refer to each term as a token after preprocessing the text, such as dropping stop words.

¹⁷ See, e.g., Damashek (1995) for description of Ngrams.

¹⁸ We show in Section 6 additional results based on Ensemble methods, and find our results to be robust to model choice.

¹⁹ Another popular algorithm in asset pricing is LASSO, which uses an L-1 penalty to achieve model sparsity. Since we are primarily interested in the forecasting performance of the model rather than variable selection, we focus on logistic ridge regression. With LASSO, we are able to report weaker but consistent results.

²⁰ See Hastie et al. (2017) for an introduction of polynomial transformation. This function is implicitly used in kernel methods such as support vector machines.

²¹ King and Zeng (2001) shows that in highly imbalanced learning problems, the coefficients can be biased towards the majority class, effectively rendering the model useless. They propose several measures to mitigate the bias, including the prior correction procedure and weighted logistic regression. We use the second option because the first requires the knowledge of prior distribution. The log-likelihood function of the weighted logit equation is: ln L_w(β|y) = w_1 ∑_{Y_i=1} ln π_i + w_0 ∑_{Y_i=0} ln (1 − π_i), where w is the weight, and π is the conditional probabilities. The intuition for the weighted logistic is that the objective function is weighted by a coefficient w that is inversely related to the sample class distribution. Consequently, the minority class gets weighted more heavily, thus mitigating the bias. We tune w via cross-validation.

²² We choose 1% because Kamiya et al. (2021) document that attacked firms on average experienced -1% CAR around the events. Our results are robust to different specifications. We show in Section 6 that using 0.5% absolute CAR as the filter or using no filter produces similar results.

²³ See Brodersen et al. (2010); Yue et al. (2007); He and Garcia (2009) for discussions of these metrics.

²⁴ ICS, NYU Engineering, https://wp.nyu.edu/awm1/. According to the website, "The Index of Cyber Security is a measure of perceived risk. A higher index value indicates a perception of increasing risk, while a lower index value indicates the opposite."

²⁵ CIBR, https://www.ftportfolios.com/retail/etf/etfsummary.aspx?Ticker=CIBR.

²⁶ HACK, https://etfmg.com/funds/hack/.

²⁷ Bloomberg report: https://www.bloomberg.com/graphics/corporate-hacks-cyber-attacks/?sref=GlJWBQ7Q.