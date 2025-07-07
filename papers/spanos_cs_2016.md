# The impact of information security events to the stock market: A systematic literature review

**Authors:** Georgios Spanos, Lefteris Angelis*  
**Department of Informatics, Aristotle University of Thessaloniki, Greece**

## Article Info

**Article history:**
- Received 30 December 2014
- Received in revised form 5 October 2015
- Accepted 28 December 2015
- Available online 2 February 2016

**Keywords:**
- Information security
- Security breaches
- Stock market
- Literature review
- Event study

## Abstract

Information security is a highly critical aspect of information systems. Although the literature regarding security assurance is vast, the research on economic consequences of security incidents is quite limited. The purpose of this systematic review is to search, collect and classify event studies related to information security impact on stock prices. In total, 37 related papers conducting 45 studies were found by the systematic search of bibliographic sources. The majority (75.6%) of these studies report statistical significance of the impact of security events to the stock prices of firms.

© 2016 Elsevier Ltd. All rights reserved.

---

## 1. Introduction

Nowadays, information systems and the Internet possess a dominant position in the business world since they provide powerful managerial tools for the companies. In fact, the majority of the operational procedures are accomplished through information systems. However, along with the growth of the information systems and the Internet, threats related to information security have appeared and evolved through time.

It is well known that even though the technology for security assurance becomes more and more complex and robust through advancement of architectures, protocols, algorithms and mathematical tools, the complete mitigation of vulnerabilities is unfeasible. Taking into account the parallel technological progress of malevolent attackers and the profits from fraud, information security is a continuously evolving field of research with practical interest for the business world. As an example, we can refer to studies (Ghosh and Swaminatha, 2001; Kim et al., 2010; Zhang et al., 2012) concerning the security in e-commerce. Another example is the research related to scoring and finding optimal schemas for prioritizing software security vulnerabilities (Liu and Zhang, 2011; Liu et al., 2012; Mell et al., 2007, June; Spanos and Angelis, 2015; Spanos et al., 2013; Wang and Yang, 2012).

A subject of financial importance is the study of the consequences of security incidents. This is a complicated problem, even in its definition. Indeed, the word "consequence" implies a causal relationship, which in the case of security violations cannot be easily determined or measured, especially because finding correlation between security events and economic value changes may be misinterpreted as a cause–effect relationship. Consequences can be economical, managerial, social or even political. Also, they can be short-term or long-term, direct or indirect. Furthermore, some consequences may have not been even publicized.

Our interest for the quantitative analysis of the National Vulnerability Database (NVD, 2015) led us to consider the problem of measuring the consequences of information security incidents. As stock markets constitute a wealth of data sources, reacting directly or indirectly to various real world incidents, the problem of quantifying and statistically studying the economic consequences of security events becomes more tangible. Furthermore, based on the efficient market hypothesis, the stock market is "informationally efficient" and subsequently the stock price of a firm depicts all the available information (Fama, 1970). Despite the impact of Fama's theory on financials, there are also different opinions in the relevant literature that criticized the theory (and more precisely the term "efficient") and reported its deficiencies (Jensen, 1978; Malkiel, 2003).

Therefore, the present systematic literature review is motivated by our intention to find, collect, classify and study the articles related to the impact of information security incidents to stock prices. Ultimately, the review is motivated by the need to assess the severity of security events on economics of companies.

The assessment of the impact of unexpected events (here the events are related to information security) on the stock price of firms is performed in the financial literature with the event-study methodology since the late 1960s; however, only during the last twelve years in the literature of information security. The basic principle of this statistical methodology – as its name indicates – is that an unexpected event is expected to affect (positively or negatively) the stock price of a firm that is related to the event in such a way that the return of this stock price will be abnormal. The normal return of a firm is estimated from the previous stock price returns while by abstracting it from the actual return the abnormal return can be derived. If the difference is positive, then the impact of the event to the stock price is considered positive. Respectively, if the difference is negative, then the impact to the stock price is considered negative. Finally, the number of factors that are used in the model to estimate the normal return characterizes the estimation model.

It was early 2000s when the consequences of information security events in the stock price of firms were first investigated. The first incidents that were analyzed by the researchers were the information security breaches. The security breaches are essentially the successful attacks over the information systems by hackers aiming to harm the confidentiality, the integrity or the availability of a system. Sub-categories of information security breaches that we can observe in this early literature are the privacy breaches, the Denial of Service (DOS) and the Website defacement.

Firstly, the privacy breaches are a sub-category of security breaches that have as purpose to harm the confidentiality of a system by obtaining unauthorized access to confidential information. Respectively, the DOS is a well-known attack and a sub-category of security breach that targets the availability of the information systems by making the resources inoperative and has, as a result, the loss of a service. Finally, the last sub-category, the Website defacement aims to harm the integrity of the system by changing the visual appearance of the site. These first publications studied the impact of these events to the stock price of breached firms (Campbell et al., 2003; Cavusoglu et al., 2004; Ettredge and Richardson, 2003; Garg et al., 2003; Hovav and D'Arcy, 2003, 2004), to the stock price of information security firms (Cavusoglu et al., 2004; Ettredge and Richardson, 2003; Garg et al., 2003; Hovav and D'Arcy, 2004) and to the stock price of the competitors of breached firms (Ettredge and Richardson, 2003). During the following years until today, several studies have been conducted, covering different aspects of the phenomenon Impact of Information Security Events to Stock Market.

The research goal of this paper is the systematic search of the related studies in electronic bibliographic sources, the filtering of those who are most relevant to the aforementioned research subject, the classification of them based on specific characteristics, and finally, the aggregation of the results that are presented in the studies in order to understand better the consequences of this kind of events, extract general conclusions and utilize this aggregated knowledge for future research.

The rest of the paper is organized as follows. In the second section, related work is presented. In the third section, the methodology that is used to conduct the systematic literature review is described. In the fourth section, the results of the review are described, and finally, the fifth section contains the conclusions of the paper.

---

## 2. Related work

Literature reviews constitute a very powerful tool in the hands of the researchers, since they aggregate in summarized form all the information about the research in a specific field. Hence, many literature reviews have been conducted during the last decades in many different scientific areas: medicine, physical sciences, social sciences, economics and others. Especially in computer science, literature reviews are very common, mainly due to the new fields that continuously emerge with the evolution of technology. Examples include the field of software engineering (Ampatzoglou and Stamelos, 2010; Kitchenham et al., 2009, 2010; Radjenović et al., 2013), computer security (Iankoulova and Daneva, 2012), e-commerce (Ngai and Wat, 2002), Internet banking (Hanafizadeh et al., 2014), mobile banking (Shaikh and Karjaluoto, 2014), ERP Systems (Aloini et al., 2007), Web (Chiou et al., 2010) and many others.

The most related works with the current systematic literature review are reviews regarding the stock market reaction to events related to information technology. These papers are studies analyzing either the impact of IT investments (management information systems, e-commerce, ERP, CRM, DSS) to the stock price of firms, or the impact of general IT events (including IT investments, Information Security, IT outsourcing and others) on the market value of firms.

Dehning et al. (2003) conducted a literature review of the event studies in MIS. This review investigates the stock market reaction to IT investments. The works by Roztocki and Weistroffer (2009b) and by Zhang and Huang (2009) belong to the same category.

Furthermore, Roztocki and Weistroffer (2008, 2009a, 2011) conducted three literature reviews concerning the stock market reaction to general information technology events (as described above). These reviews contain in total 30, 46 and 73 articles respectively. However, only 6, 9 and 13 articles respectively concern the field of information security. Similarly, Konchitchki and O'Leary (2011) conducted a literature review having the same subject with the above three reviews, emphasizing the analysis of the event-study methodology. This review also contains few articles (9 articles) related to information security events.

The difference of the current literature review, in comparison to the aforementioned studies, is its focus on the different information security incidents and their specific characteristics. Moreover, this is the first systematic literature review that has as subject the impact of information security events to the stock price of firms. Overall, the present review aims to enrich the existing literature reviews, with the most recent articles as well as with articles that have been omitted from previous reviews in the research area of stock market reaction to information security events.

---

## 3. Methodology

The systematic literature review that is presented here follows the procedures that are described in Kitchenham (2004) and Kitchenham and Charters (2007). Although these guidelines are software engineering-oriented, the basic principles are essential, generic and valid for any literature review so they were also adopted for our systematic review.

According to the aforementioned guidelines, this systematic literature review has three stages: the Planning Stage, the Conducting Stage and the Reporting Stage. The steps of each stage are shown in Fig. 1 (each row of the figure corresponds to the related Stage).

![Fig. 1 – The steps of the systematic literature review procedure](figure1.png)

The first step of the planning stage referred to the identification of the need for a Systematic Review. As described in the previous two sections, although there are several studies that try to investigate the impact of information security events to the stock price of firms, there is no review that summarizes all these studies and offers a deeper insight to this crucial research area. Therefore, the need for a systematic literature review that will provide the researchers with information about the methodology used and the results found so far is obvious and essential.

The second step of the Planning Stage is the development of the Review Protocol. Essentially, the Review Protocol defines the whole procedure of the Conducting Stage by analyzing the necessary actions that have to be accomplished in order to continue with the Conducting Stage. These actions are described next and they are: the definition of research questions, the selection of the search strategy, the definition of the study's inclusion/exclusion criteria, the definition of the study quality assessment criteria and finally the selection of the data that will be extracted from the studies. The review protocol is refined during the entire procedure of the systematic review.

The definition of research question(s) is a very crucial step in every systematic review. By answering these questions, literature reviews essentially accomplish their aim. The research questions of the present systematic literature review are stated below:

• **How many research studies exist, having as subject the impact of information security events to the stock price of firms?**
• **What types of information security events have been analyzed in the literature?**
• **What types of studies have been conducted in the existing literature?**
• **What are the results of the studies and the significance of them?**

The first step of deciding the search strategy involves the selection of the search method that can be one of the following: the broad automated search in digital libraries, the manual search in specific journals and conference proceedings, the snowball technique (backward or forward) or a combination of the previous methods. In the present systematic review, we decided to use a combination of the broad automated search and the backward snowball technique.

The broad automated search method includes the selection of the most appropriate digital sources (digital libraries and indexing systems) and the determination of the search terms. The sources that were selected in the presented literature review are the digital libraries of: Science Direct¹, Citeseer², IEEE³, Web of Science⁴ and Scopus⁵.

The determination of search terms is an iterative procedure starting with trial searches using different search terms, considering an initial set of papers that is already known to belong to the research field of the systematic review. The procedure of determining search terms ends when the initial set of already known papers (or the majority of them if the whole set is impossible to be found from the libraries) is found by the search.

All the aforementioned digital sources offer the opportunity to perform a search using a sophisticated search string combining Boolean operators. The search string that was used in the present literature review is:

```
(("Information Security" OR "Computer Security" OR "Network Security" OR "Internet Security" OR "Information System Security" OR "Web Security" OR "Software Security" OR "Application Security") AND ("Market Value" OR "Stock Value" OR "Stock Market" OR "Stock Price" OR "Market Price"))
```

All the searches are based on the title, the abstract and the keywords of the papers in order to avoid receiving a huge number of irrelevant papers as search results.

The backward snowball technique was used as a complement to the broad automated search in order to find papers that cannot be found by the first method. The backward snowball technique is essentially the iterative review of the references of an initial set of papers. At each iteration, this set is updated by finding new related papers while the procedure ends when no more new papers can be found. The combination of the two techniques increases the probability that the systematic literature review covers the vast majority of the papers in this research field.

The inclusion/exclusion selection criteria of any systematic literature review must be clear and well-defined, because they facilitate the procedure of the study selection. The selection criteria of the present systematic review are shown below:

• **Inclusion Criterion**
  - Papers that were published before 24 September of 2015 and perform at least one study that analyzes the impact of information security events to the stock price of firms, using the event study methodology.

• **Exclusion Criteria**
  - Papers performing studies related to the impact of general IT failures on the market value of firms.
  - Papers performing studies related to the impact of general IT investments on the firm stock price.
  - Papers performing studies that analyze the stock market reaction to IT security incidents as a prerequisite for another study, and they do not report the results.

The quality assessment criteria are defined to ensure that all the included studies in a systematic literature review attain an acceptable level of quality. In the present literature review, the criteria for a paper to be included in the study regard the availability and the description of the data, the description of the used methodology and the presentation of the results. Papers that at least cover partially the above four criteria are included in the review.

Finally, the last action related to the development of the review protocol is the selection of the data features that will be extracted from the papers found by the search. The data features in our review are listed below:

• Authors
• Publication source
• Year of publication
• Type of paper (Journal/Conference/Workshop)
• Type of information security event
• Data source
• Time interval of the sample
• Country of stock market
• Estimation model
• Type of study
• Number of incidents in each study
• Result
• Significance of the result

After the development of the review protocol, all the predefined steps of the systematic literature review are executed. In Fig. 2, the steps leading to the final number of the selected papers of the present review are depicted. Specifically, after the initial search process, 191 papers were found. After the reading of titles and abstracts of the candidate papers, aiming to find irrelevant papers or duplicates, 145 papers were removed and the number of remaining papers became 46. Next, after the reading of full papers, 19 more papers were removed as irrelevant based on the inclusion/exclusion criteria. Hence, the final number of selected papers resulting from the broad automated search was 27.

![Fig. 2 – The steps to find the final number of inserted papers](figure2.png)

As already mentioned, the backward snowball technique was subsequently applied and from the reading of the references, 10 more papers were added. Thus, the number of the papers after the entire study selection process was 37. Finally, these 37 papers cover either partially or completely the four quality assessment criteria described above and therefore, the concluding number of selected papers for our literature review is 37.

---

## 4. Results

In this section, the results of the systematic literature review are presented. In Table 1, the publication characteristics of the 37 papers are shown. These are: the names of the authors, the publication source, the year of publication, the types of papers and the article number.

### Table 1 – The publication characteristics of the papers

| Authors | Publication source | Year of publication | Type of paper | Article no. |
|---------|-------------------|-------------------|--------------|-------------|
| K. Campbell, L. Gordon, M. Loeb, L. Zhou | Journal of Computer Security | 2003 | Journal | a1 |
| A. Garg, J. Curtis, H. Halper | Information Management and Computer Security | 2003 | Journal | a2 |
| A. Hovav, J. D'Arcy | Risk Management and Insurance Review | 2003 | Journal | a3 |
| M. Ettredge, V. Richardson | Journal of Information Systems | 2003 | Journal | a4 |
| H. Cavusoglu, B. Mishra, S. Raghunathan | International Journal of Electronic Commerce | 2004 | Journal | a5 |
| A. Hovav, J. D'Arcy | Information Systems Security | 2004 | Journal | a6 |
| A. Hovav, J. D'Arcy | Computers & Security | 2005 | Journal | a7 |
| A. Acquisti, A. Friedman, R. Telang | International Conference on Information Systems | 2006 | Conference | a8 |
| M. Ishiguro, H. Tanaka, K. Matsuura, I. Murase | International Workshop on the Economics of Securing the Information Infrastructure | 2006 | Workshop | a9 |
| K. Aytes, S. Byers, M. Santhanakrishnan | Americas Conference on Information Systems | 2006 | Conference | a10 |
| R. Telang, S. Wattal | Software Engineering, IEEE Transactions on | 2007 | Journal | a11 |
| K. Kannan, J. Rees, S. Sridhar | International Journal of Electronic Commerce | 2007 | Journal | a12 |
| A. Leung, I. Bose | International Conference on Information Technology | 2008 | Conference | a13 |
| S. Goel, H. Shawky | Information & Management | 2009 | Journal | a14 |
| J. Muntermann, H. Roßnagel | Nordic Conference on Secure IT Systems | 2009 | Conference | a15 |
| D. Liginlal, I. Sim, L. Khansa | Computers & Security | 2009 | Journal | a16 |
| F.K. Andoh-Baidoo, K. Amoako-Gyampah, K.-M. Osei-Bryson | Security & Privacy, IEEE | 2010 | Journal | a17 |
| K. Gatzlaff, K. McCullough | Risk Management and Insurance Review | 2010 | Journal | a18 |
| N. Patel | Duke Journal of Economics | 2010 | Journal | a19 |
| P. Bolster, C. Pantalone, E. Trahan | Journal of Business Valuation and Economic Loss Analysis | 2010 | Journal | a20 |
| S. Chai, M. Kim, H. Rao | Decision Support Systems | 2011 | Journal | a21 |
| X. Chen, I. Bose, A. Leung, C. Guo | Decision Support Systems | 2011 | Journal | a22 |
| A. Yayla, Q. Hu | Journal of Information Technology | 2011 | Journal | a23 |
| E. Morse, V. Raval, J. Wingender | Information Security Journal | 2011 | Journal | a24 |
| L. Gordon, M. Loeb, L. Zhou | Journal of Computer Security | 2011 | Journal | a25 |
| K. Smith, M. Smith, J. Smith | Academy of Marketing Studies Journal | 2011 | Journal | a26 |
| L. Khansa, D. Cook, T. James | Computers & Security | 2012 | Journal | a27 |
| J. Chen, H.C. Li, D.C. Yen, K.V. Bata | Computers in Human Behavior | 2012 | Journal | a28 |
| J. Cardenas, A. Cornado, A. Donald, F. Parra, M.A Mahmood | Americas Conference on Information Systems | 2012 | Conference | a29 |
| I. Bose, A. Leung | Decision Support Systems | 2013 | Journal | a30 |
| T. Wang, J. Rees, K. Kannan | Journal of Organizational Computing and Electronic Commerce | 2013 | Journal | a31 |
| I. Bose, A. Leung | Decision Support Systems | 2014 | Journal | a32 |
| S. Goel, H. Shawky | Communications of the Association for Information Systems | 2014 | Journal | a33 |
| M.C Arcuri, M. Borgi, G. Gandolfi | European Financial Management Association Meeting | 2014 | Conference | a34 |
| S. Pirounias, D. Mermigas, C. Patsakis | Journal of Information Security and Applications | 2014 | Journal | a35 |
| S. Modi, M. Wiles, S. Mishra | Journal of Operations Management | 2015 | Journal | a36 |
| O. Hinz, M. Nofer, D. Schiereck, J. Trillig | Information & Management | 2015 | Journal | a37 |

The authors participating in most of the publications (4 publications) are: Indranil Bose and Alvin Leung, followed by Anat Hovav and John D'Arcy with 3 publications. The publication source that published the majority of the papers is the journal "Decision Support Systems" with 4 publications, followed by the journal "Computers & Security" with 3 publications. Furthermore, as it is shown in Table 1 and Fig. 3, we have a balanced distribution of published papers in the literature. The majority of the papers (6) were published during the year 2011 whereas during the rest of the years, starting from 2003 until September 2015, the numbers of published papers range between 1 and 4. Finally, in Table 1 and Fig. 4, the different types of papers and their frequencies are shown. The vast majority of the papers (81.1%, 30 publications) that are included in the systematic literature review were published in journals. Next, 6 publications (16.2%) were published in conference proceedings and finally there is one publication (2.7%) in workshop proceedings.

![Fig. 3 – Publications per year](figure3.png)

![Fig. 4 – Type of paper](figure4.png)

In Table 2 the following characteristics of the papers are shown: types of events, time intervals of samples, countries of the stock market, data sources, estimation models and the article numbers.

### Table 2 – The event characteristics of the 37 papers

| Type of event | Time interval of sample | Country of stock market | Data source | Estimation model | Article no. |
|---------------|------------------------|------------------------|-------------|------------------|-------------|
| Security Breaches | 1995–2000 | USA | Wall Street Journal, New York Times, Washington Post, Financial Times, USA Today | One-factor | a1 |
| Security Breaches | 1996–2002 | USA | — | — | a2 |
| Security Breaches | 1998–2002 | USA | Lexis/Nexis | One-factor | a3 |
| Security Breaches | 2000 | USA | — | One-factor | a4 |
| Security Breaches | 1996–2001 | USA | Lexis/Nexis, CNET, ZDNET | One-factor | a5 |
| Security Breaches | 1988–2002 | USA | Lexis/Nexis | One-factor | a6 |
| Security Breaches | 1988–2002 | USA | Lexis/Nexis | One-factor | a7 |
| Security Breaches | 2000–2006 | USA | Lexis/Nexis, ProQuest, Choicepoint, www.emergentchaos.com, Data Loss Archive and Database | One-factor | a8 |
| Security Breaches | 2002–2005 | Japan | Nippon Keizai Shinbun, Nikkei Sangyo Shinbun, Nikkei Ryutsu Shinbun, Nikkei Kinyu Shinbun | One-factor | a9 |
| Security Breaches | 1995–2005 | USA | Lexis/Nexis | One-factor | a10 |
| Software Vulnerabilities | 1999–2004 | USA | Lexis/Nexis, ProQuest, CNET, CERT | One-factor | a11 |
| Security Breaches | 1997–2003 | USA | Wall Street Journal, New York Times, ZDNet, CNET | One-factor | a12 |
| Phishing | Before 2008 | Global Sample | Millersmiles, Websense, Factiva, Antiphishing Working Group Japan, Hong Kong Monetary Authority, Malaysia Computer Emergent Response Team | One-factor | a13 |
| Security Breaches | 2004–2008 | USA | Lexis/Nexis, Wall Street Journal, PC Week, Register | One-factor, Fama–French three-factor | a14 |
| Security Breaches | 2001–2007 | USA | Data Loss Archive and Database | One-factor | a15 |
| Security Breaches | 2005–2008 | USA | Privacy Rights Clearinghouse, Data Loss Archive and Database, Google, New York Times, Washington Post, Financial Times | One-factor | a16 |
| Security Breaches | 1997–2003 | USA | Lexis/Nexis | One-factor | a17 |
| Security Breaches | 2004–2006 | USA | Lexis/Nexis, Privacy Rights Clearinghouse | One-factor | a18 |
| Security Breaches | — | USA | Data Loss Archive and Database | One-factor | a19 |
| Security Breaches | 2000–2007 | USA | Data Loss Archive and Database | One-factor | a20 |
| IT Security Investments | 1997–2006 | USA | Lexis/Nexis | One-factor | a21 |
| Phishing | 2005–2008 | Global Sample | Millersmiles | One-factor | a22 |
| Security Breaches | 1994–2006 | USA | Google, Yahoo!, Lexis-Nexis | One-factor | a23 |
| Security Breaches | 2000–2010 | USA | Data Loss Archive and Database | One-factor | a24 |
| Security Breaches | 1995–2007 | USA | Wall Street Journal, New York Times, Washington Post, Financial Times, USA Today | One-factor, Fama–French three-factor | a25 |
| Security Breaches | 2000–2005 | USA | ProQuest | One-factor | a26 |
| IT Security Legislation | 1996–2010 | USA | Public Health Data Standards Consortium, US Department of HHS | One-factor | a27 |
| Security Breaches | 2006–2007 | USA | Data Loss Archive and Database | One-factor | a28 |
| Security Breaches | 2002–2008 | USA | Lexis/Nexis, CNET, ZDNET | One-factor | a29 |
| IT Security Investments | 1995–2012 | USA | Factiva, PR NewsWire, Business Newswire | One-factor | a30 |
| Security Breaches | 1997–2008 | USA | Factiva, CNet, ZDNet, Yahoo! | One-factor, Fama–French three-factor | a31 |
| Phishing | 2003–2007 | Global Sample | Millersmiles, Websense, Factiva | One-factor, Fama-French three-factor, International Fama–French two factor | a32 |
| Security Breaches | 2001–2008 | USA | Privacy Rights Clearinghouse | Four-factor | a33 |
| Security Breaches | 1995–2012 | Global | Factiva | One-factor | a34 |
| Security Breaches | 2008–2012 | USA | Data Loss Archive and Database, Privacy Rights Clearinghouse, Identity Theft Resource Center | One-factor, Fama–French three-factor | a35 |
| Security Breaches | 2005–2010 | USA | Identity Theft Resource Center | Four-factor | a36 |
| Security Breaches | 2011–2012 | Global | Data Loss Archive and Database | One-factor | a37 |

As it is observed in Table 2 and Fig. 5, there are five different types of security events that were analyzed in the literature. The vast majority (81.1%) concern Security Breaches, appearing 30 times. Phishing was analyzed by 3 papers (8.1%), IT Security Investments by 2 papers (5.4%) and finally Software Vulnerabilities and IT Security Legislation only once (2.7%). Four out of five types of information security events – except security breaches that were described in the introduction – are described below.

![Fig. 5 – Type of security event](figure5.png)

**Phishing** tries to acquire confidential information from unsuspicious users. In this case, the attacker pretends to be a trustworthy entity and asks (most of the times via e-mail) complete confidential information from the user-victim. 

**IT Security Investments** consist of investments that a company performs to strengthen the defense of their information systems and to assure their confidential data from potential attacks. 

**Software vulnerabilities** are bugs or weaknesses of the software that a potential attacker can exploit to harm the confidentiality, the integrity or the availability of a system. In essence, a software vulnerability leads to a security breach if the attacker achieves to exploit the vulnerability before the development of the corresponding patch that fixes the vulnerability. 

Finally, **IT Security Legislation** defines the rules and the laws that the firms must follow to ensure the confidential data of their customers.

From the above analysis of the information security events, it is obvious that there is no intense research activity dealing with the impact to the stock market of the events: Phishing, IT Security Investments, Software Vulnerabilities and IT Security Legislation.

The second characteristic of Table 2 is the report of time intervals of the data samples. The time intervals used in the papers of the systematic review started from 1988 (a6, a7) while the most recent time interval ends in 2012 (a30, a34, a35, a37). Moreover, the smallest time interval is three days (7 February 2000 – 9 February 2000) in a4 and the largest is seventeen years (1995–2012) in a34.

Furthermore, as it is shown in Table 2 and Fig. 6, the vast majority of the papers (83.8%) used firms that are traded in the USA Stock Market in their analysis, five papers (13.5%) used firms from different countries and only one (2.7%) used firms traded in the Japan Stock Market. This trend of the researchers to choose firms from USA for their analysis can be interpreted in various ways. One reason could be the availability of information as companies in USA find it obligatory to inform the customers about breaches in order to build confidence between organizations and customers who are able to take precautions. Also important is the fact that information from newspaper articles in English language is more easily accessible.

![Fig. 6 – Country of stock market](figure6.png)

Another important observation that is derived from Table 2 is that the most popular data source of information security events that was used in 32.4% of the papers is the public database Lexis/Nexis that covers the major newspapers of USA. Other popular sources are the "Data Loss Archive and Database" which has data of privacy breaches with 9 appearances (24.3%), the technology portal CNET⁶ that was used in 5 papers (13.5%) and the Factiva database with 5 appearances also (13.5%). In total, 33 different data sources have been used in the literature and in almost half of the publications (48.6%) more than one data source was utilized in order to collect the information security events.

Regarding the model employed, in 78.4% of the papers only the one-factor model, which is the most simple market model, was used. This factor can be the market return or the mean return of the stock in the previous trading days before the event or the return of a competitor of the firm. Moreover, in the 13.5% of the publications, the Fama–French three-factor model (Fama and French, 1993) was used. This model implements three factors: the market return, the risk factor HML that represents the value firm premium (difference between high and low book-to-market ratio) and the risk factor SMB that represents the small firm premium (difference between the returns of small and big firms). Also, in a32 the International Fama–French two-factor model first appeared which uses the international book-to-market correction factor (Fama and French, 1998) (difference between high and low book-to-market ratio for each country separately) and the market return. Finally, in a33 a four-factor estimation model that adds the momentum factor to the Fama–French three-factor model was introduced (also used in a36).

In Table 3, the study characteristics and the results of the 45 studies that were performed in the 37 papers of the literature review are shown (since in a2, a4, a5, a10, a27 and a37 more than one study was performed).

### Table 3 – The study characteristics and the results

| Type of Study | Events | Result | Significance | Article no. |
|---------------|--------|--------|--------------|-------------|
| Impact of Security Breaches to Breached Firms | 43 | Negative | No | a1 |
| Impact of Security Breaches to Breached Firms | 22 | Negative | Yes | a2 |
| Impact of Security Breaches to Information Security Firms | 22 | Positive | Yes | a2 |
| Impact of Security Breaches to Breached Firms | 23 | Negative | No | a3 |
| Impact of Security Breaches to Breached Firms | 4 | Negative | Yes | a4 |
| Impact of Security Breaches to Information Security Firms | 10 | Positive | Yes | a4 |
| Impact of Security Breaches to Competitors of Breached Firms | 168 | Negative | Yes | a4 |
| Impact of Security Breaches to Breached Firms | 66 | Negative | Yes | a5 |
| Impact of Security Breaches to Information Security Firms | 66 | Positive | Yes | a5 |
| Impact of Security Breaches to Breached Firms | 186 | Positive | No | a6 |
| Impact of Security Breaches to Responsible Vendors | 92 | Negative | No | a7 |
| Impact of Security Breaches to Breached Firms | 79 | Negative | Yes | a8 |
| Impact of Security Breaches to Breached Firms | 70 | Negative | Yes | a9 |
| Impact of Security Breaches to Breached Firms | 67 | Negative | No | a10 |
| Impact of Security Breaches to Competitors of Breached Firms | 67 | Positive | Yes | a10 |
| Impact of Software Vulnerabilities to Software Vendors | 147 | Negative | Yes | a11 |
| Impact of Security Breaches to Breached Firms | 72 | Negative | No | a12 |
| Impact of Phishing to Related Firms | 2994 | Negative | Yes | a13 |
| Impact of Security Breaches to Breached Firms | 168 | Negative | Yes | a14 |
| Impact of Security Breaches to Breached Firms | 97 | Negative | Yes | a15 |
| Impact of Security Breaches to Breached Firms | 151 | Negative | Yes | a16 |
| Impact of Security Breaches to Breached Firms | 41 | Negative | Yes | a17 |
| Impact of Security Breaches to Breached Firms | 77 | Negative | Yes | a18 |
| Impact of Security Breaches to Breached Firms | 34 | Mixed | No | a19 |
| Impact of Security Breaches to Breached Firms | 93 | Positive | No | a20 |
| Impact of IT Security Investments to Firms that Invest | 101 | Positive | Yes | a21 |
| Impact of Phishing to Related Firms | 1030 | Neutral | No | a22 |
| Impact of Security Breaches to Breached Firms | 123 | Negative | Yes | a23 |
| Impact of Security Breaches to Breached Firms | 306 | Negative | Yes | a24 |
| Impact of Security Breaches to Breached Firms | 121 | Negative | Yes | a25 |
| Impact of Security Breaches to Breached Firms | 10 | Negative | Yes | a26 |
| Impact of IT Security Legislation to Firms that the Legislation Applied | 2095 | Negative | Yes | a27 |
| Impact of IT Security Legislation to Information Technology Firms | 18522 | Positive | Yes | a27 |
| Impact of IT Security Legislation to Information Security Firms | 1653 | Positive | Yes | a27 |
| Impact of Security Breaches to IT Consulting Firms | 83 | Positive | No | a28 |
| Impact of Security Breaches to Breached Firms | 39 | Negative | No | a29 |
| Impact of IT Security Investments to Firms that Invest | 87 | Positive | Yes | a30 |
| Impact of Security Breaches to Breached Firms | 89 | Negative | Yes | a31 |
| Impact of Phishing to Related Firms | 1942 | Negative | Yes | a32 |
| Impact of Security Breaches to Breached Firms | 201 | Negative | Yes | a33 |
| Impact of Security Breaches to Breached Firms | 128 | Negative | Yes | a34 |
| Impact of Security Breaches to Breached Firms | 105 | Negative | Yes | a35 |
| Impact of Security Breaches to Breached Firms | 146 | Negative | Yes | a36 |
| Impact of Security Breaches to Breached Firms | 6 | Negative | Yes | a37 |
| Impact of Security Breaches to Competitors of Breached Firms | 346 | Negative | Yes | a37 |

There are 11 different types of studies that have been conducted until now in the literature and the most common study is the analysis of the Impact of Security Breaches to Breached Firms, indicating that this study is the main concern of the research community and in general, of the IT community. This type of analysis appeared 28 times (62.2%), followed by the studies analyzing the Impact of Security Breaches to Information Security Firms (6.7%), the Impact of Security Breaches to Competitors of Breached Firms (6.7%) and those that analyzed the Impact of Phishing to Related Firms (6.7%). Also, in two cases (4.4%) we found an analysis of the Impact of IT Security Investments to Firms that Invest. Finally, only one paper (2.2%) concerned studies regarding each of the following subjects: Impact of Software Vulnerabilities to Software Vendors; Impact of IT Security Legislation to Firms that the Legislation Applied; Impact of IT Security Legislation to Information Technology Firms; Impact of IT Security Legislation to Information Security Firms; Impact of Security Breaches to Responsible Vendors and Impact of Security Breaches to IT Consulting Firms. These results depict the unbalanced distribution of existing types of studies in the research field and the need for research activity in types of studies other than the Impact of Security Breaches to Breached firms.

The number of events that have been used ranges from only 4 events (a3) to 18,522 events (a26). More precisely, the number of events for the type Impact of Security Breaches to Breached Firms ranges from 4 to 306 with an average of 91.7 events. Respectively, the number of events for the type Impact of Security Breaches to Information Security Firms ranges from 10 to 66 events with an average of 32.7, whereas for the type Impact of Security Breaches to Competitors of Breached Firms the number of events ranges from 67 to 346 with an average of 193.7. Moreover, the number of events for the type Impact of Phishing to Related Firms ranges from 1030 to 2994 with an average of 1988.7 events. Furthermore, this number ranges from 87 to 101 with an average of 94 events for the type Impact of IT Security Investments to Firms that Invest and finally, the number of events for the types of studies that appear only once are: 147 events for Impact of Software Vulnerabilities to Software Vendors, 2095 for Impact of IT Security Legislation to Firms that the Legislation Applied, 18,522 for Impact of IT Security Legislation to Information Technology Firms, 1653 for Impact of IT Security Legislation to Information Security Firms, 92 for Impact of Security Breaches to Responsible Vendors and 83 for Impact of Security Breaches to IT Consulting Firms. From these results, it is obvious that the number of events that have been used in each study is different for each type of study.

The third column of Table 3 contains the results of the abnormal returns that an information security event causes, as presented in the primary studies and could be negative (71.1%), positive (24.4%), mixed (2.2%) or neutral (2.2%). In the majority of the studies a negative abnormal return to stock prices is observed due to the fact that 28 out of 45 studies analyze the Impact of Security Breaches to Breached Firms which can be considered a negative phenomenon without a doubt. As we will see later, a negative event, as the Security Breach is, for some firms can be considered as a threat but for other firms can be considered as an opportunity.

Finally, it is obvious from Table 3 that the majority of the studies (75.6%) produced results that are statistically significant. Several statistical tests as the t-test, the Z-test, the Wilcoxon sign-ranked test and the Sign Test have been applied in the literature to test the significance of the results. Consequently, from the body of studies retrieved for the systematic review, it seems that in general, the information security events affect the stock price of the firms and this impact is statistically significant.

Finally, Table 4 presents the summarized results of the studies.

### Table 4 – The summarized results of the studies

| Type of Study | Positive (Significant) | Negative (Significant) | Neutral (Significant) | Mixed (Significant) | Sum (Significant) |
|---------------|----------------------|----------------------|---------------------|-------------------|------------------|
| Impact of Security Breaches to Breached Firms | 2 (0) | 25 (20) | — | 1 (0) | 28 (20) |
| Impact of Security Breaches to Information Security Firms | 3 (3) | — | — | — | 3 (3) |
| Impact of Security Breaches to Competitors of Breached Firms | 1 (1) | 2 (2) | — | — | 3 (3) |
| Impact of Phishing to Related Firms | — | 2 (2) | 1 (0) | — | 3 (2) |
| Impact of IT Security Investments to Firms that invest | 2 (2) | — | — | — | 2 (2) |
| Impact of Software Vulnerabilities to Software Vendors | — | 1 (1) | — | — | 1 (1) |
| Impact of IT Security Legislation to Firms that the Legislation Applied | — | 1 (1) | — | — | 1 (1) |
| Impact of IT Security Legislation to Information Technology Firms | 1 (1) | — | — | — | 1 (1) |
| Impact of IT Security Legislation to Information Security Firms | 1 (1) | — | — | — | 1 (1) |
| Impact of Security Breaches to Responsible Vendors | — | 1 (0) | — | — | 1 (0) |
| Impact of Security Breaches to IT Consulting Firms | 1 (0) | — | — | — | 1 (0) |

First of all, as we mentioned above the Impact of Security Breaches to Breached Firms is considered as a negative phenomenon. The results of the statistical analysis confirm this consideration, since from 28 studies that have been performed to analyze the Impact of Security Breaches to Breached Firms, 25 (89.3%) presented a negative impact while in 20 studies (71.4%) this negative impact was found significant.

On the other hand, the Impact of Security Breaches to Information Security Firms can be considered as a positive phenomenon, because for the Information Security Firms the security breach is an opportunity, since the need for information security grows up. This consideration is also confirmed from the results, because in all 3 studies analyzing the Impact of Security Breaches to Information Security Firms, a positive impact was found and the result was statistically significant.

Next, the Impact of Security Breaches to Competitors of Breached Firms is a controversial phenomenon. On the one hand, the fact that the firm suffered a security breach seems to be an opportunity for the Competitors, but on the other hand, this security breach creates a more general lack of trust for the specific type of companies. This controversy is depicted also from the results, since there are three studies that analyze this phenomenon, with contradicting results: two studies presented negative abnormal return while the other presented positive abnormal return. In all the studies, statistically significant results were found.

Moreover, the Impact of Phishing to Related Firms is expected to be negative. Once again, the results confirmed the expectation, since two of the three studies analyzing the Impact of Phishing to Related Firms produced significantly negative results (and the third produced neutral results).

Furthermore, the Impact of IT Security Investments to Firms that Invest can be considered without a doubt a positive phenomenon. Indeed, in two studies that analyzed the Impact of IT Security Investments to Firms that Invest, the results were positive and statistically significant. These results are in accordance to the work of Wang (2010) where it is concluded that firms associating themselves in the press with IT investments gain short term reputation.

Finally, it is interesting to examine the types of studies that appeared only once in the literature. The Impact of Software Vulnerabilities to Software Vendors and the Impact of Security Breaches to Responsible Vendors is expected to be negative. Indeed, the abnormal returns of the stock prices were found negative (in the first study, the result is also significant) and reflect this expectation. Also, the Impact of IT Security Legislation to Information Technology Firms, the Impact of IT Security Legislation to Information Security Firms and the Impact of Security Breaches to IT Consulting Firms can be considered as positive phenomena since the events IT Security Legislation and Security Breaches constitute opportunities for this type of firms. The results are also positive for these three studies and in the first two are also significant. Finally, the Impact of IT Security Legislation to Firms that the Legislation Applied is considered as a negative phenomenon, since IT security legislation usually means hefty costs for the firms. Indeed, the abnormal return of the stock prices is negative and statistically significant.

---

## 5. Conclusions

The basic motivation of this paper was the need to investigate a promising area of research where statistical analysis on data can reveal the relation between information security and reaction of stock market. So we conducted a targeted systematic literature review on a specific subject, namely the Impact of Information Security Events to the Stock Market. We stated four research questions in the methodology section and we obtained the following answers: In the present systematic literature review, 37 papers that perform 45 studies were found. In these papers we identified 5 different types of events which were presented extensively in the previous section. Moreover, 11 different types of studies have been identified in the reviewed papers. The most important finding of the literature review, derived from the reviewed studies, is that the events that were examined are affecting significantly the stock price of the firms. Hence, positive events related to information security, as the investments in IT security, have also positive and significant impact to the stock price of the firms that invest in IT security. Respectively, negative information security events, as the security breaches, have a significant negative impact to the stock price of the breached firms in the majority of the studies. However, the review revealed that contradictory results are possible, depending on the original research questions and the interpretation of the results.

Overall, the conclusion derived from the studies so far is that although the issue of impact of information security events on stock market is very serious in practice and challenging for research, the related studies are not so many as one might expect. The field is therefore open for applying novel and more sophisticated and effective research methodologies.

---

## References

Acquisti A, Friedman A, Telang R. 2006. Is there a cost to privacy breaches? An event study. In Proceedings of the 3rd International Conference on Intelligent Systems (ICIS).

Aloini D, Dulmin R, Mininno V. Risk management in ERP project introduction: review of the literature. Inform Manag 2007;44(6):547–67.

Ampatzoglou A, Stamelos I. Software engineering research for computer games: a systematic review. Inf Softw Technol 2010;52(9):888–901.

Andoh-Baidoo FK, Amoako-Gyampah K, Osei-Bryson KM. How internet security breaches harm market value. IEEE Secur Priv 2010;8(1):36–42.

Arcuri MC, Brogi M, Gandolfi G. 2014. The effect of information security breaches on stock returns: Is the cyber crime a threat to firms? European Financial Management Association Meeting, Rome.

Aytes K, Byers S, Santhanakrishnan M. 2006. The economic impact of information security breaches: firm value and intra-industry effects. In Proceedings of AMCIS.

Bolster P, Pantalone CH, Trahan EA. Security breaches and firm value. J Bus Val Econ Loss Anal 2010;5(1).

Bose I, Leung ACM. The impact of adoption of identity theft countermeasures on firm value. Decis Support Syst 2013;55(3):753–63.

Bose I, Leung ACM. Do phishing alerts impact global corporations? A firm value analysis. Decis Support Syst 2014;64:67–78.

Campbell K, Gordon LA, Loeb MP, Zhou L. The economic cost of publicly announced information security breaches: empirical evidence from the stock market. J Comput Secur 2003;11(3):431–48.

Cardenas J, Coronado A, Donald A, Parra F, Mahmood MA. 2012. The Economic Impact of Security Breaches on Publicly Traded Corporations: An Empirical Investigation. In Proceedings of the AMCIS.

Cavusoglu H, Mishra B, Raghunathan S. The effect of internet security breach announcements on market value: capital market reactions for breached firms and internet security developers. Int J Electron Commer 2004;9(1):70–104.

Chai S, Kim M, Rao HR. Firms' information security investment decisions: stock market evidence of investors' behavior. Decis Support Syst 2011;50(4):651–61.

Chen JV, Li HC, Yen DC, Bata KV. Did IT consulting firms gain when their clients were breached? Comput Human Behav 2012;28(2):456–64.

Chen X, Bose I, Leung ACM, Guo C. Assessing the severity of phishing attacks: a hybrid data mining approach. Decis Support Syst 2011;50(4):662–72.

Chiou WC, Lin CC, Perng C. A strategic framework for website evaluation based on a review of the literature from 1995–2006. Inform Manag 2010;47(5):282–90.

Dehning B, Richardson VJ, Stratopoulos T. 2003. Reviewing event studies in MIS: an application of the firm value. In System Sciences Proceedings of the 36th Annual Hawaii International Conference on (pp. 9-pp). IEEE.

Ettredge ML, Richardson VJ. Information transfer among internet firms: the case of hacker attacks. J Inf Syst 2003;17(2):71–82.

Fama EF. Efficient capital markets: a review of theory and empirical work. J Finance 1970;25(2):383–417.

Fama EF, French KR. Common risk factors in the returns on stocks and bonds. J Finance Econ 1993;33(1):3–56.

Fama EF, French KR. Value versus growth: the international evidence. J Finance 1998;53(6):1975–99.

Garg A, Curtis J, Halper H. Quantifying the financial impact of IT security breaches. Inform Manag Comput Secur 2003;11(2):74–83.

Gatzlaff KM, McCullough KA. The effect of data breaches on shareholder wealth. Risk Manag Insur Rev 2010;13(1):61–83.

Ghosh AK, Swaminatha TM. Software security and privacy risks in mobile e-commerce. Commun ACM 2001;44(2):51–7.

Goel S, Shawky HA. Estimating the market impact of security breach announcements on firm values. Inform Manag 2009;46(7):404–10.

Goel S, Shawky HA. The impact of federal and state notification laws on security breach announcements. Commun Assoc Inf Syst 2014;34(1):3.

Gordon LA, Loeb MP, Zhou L. The impact of information security breaches: has there been a downward shift in costs? J Comput Secur 2011;19(1):33–56.

Hanafizadeh P, Keating BW, Khedmatgozar HR. A systematic review of internet banking adoption. Telemat Inform 2014;31(3):492–510.

Hinz O, Nofer M, Schiereck D, Trillig J. The influence of data theft on the share prices and systematic risk of consumer electronics companies. Inform Manag 2015;52(3):337–47.

Hovav A, D'Arcy J. The impact of denial-of-service attack announcements on the market value of firms. Risk Manag Insur Rev 2003;6(2):97–121.

Hovav A, D'Arcy J. The impact of virus attack announcements on the market value of firms. Inf Syst Secur 2004;13(3):32–40.

Hovav A, D'Arcy J. Capital market reaction to defective IT products: the case of computer viruses. Computers & Security 2005;24(5):409–24.

Iankoulova I, Daneva M. 2012. Cloud computing security requirements: a systematic review. In Research Challenges in Information Science (RCIS), Sixth International Conference on (pp. 1–7). IEEE.

Ishiguro M, Tanaka H, Matsuura K, Murase I. 2006. The effect of information security incidents on corporate values in the Japanese stock market. In Proceedings of the International Workshop on the Economics of Securing the Information.

Jensen MC. Some anomalous evidence regarding market efficiency. J Finance Econ 1978;6(2):95–101.

Kannan K, Rees J, Sridhar S. Market reactions to information security breach announcements: an empirical analysis. Int J Electron Commer 2007;12(1):69–91.

Khansa L, Cook DF, James T, Bruyaka O. Impact of HIPAA provisions on the stock market value of healthcare institutions, and information security and other information technology firms. Computers & Security 2012;31(6):750–70.

Kim C, Tao W, Shin N, Kim KS. An empirical study of customers' perceptions of security and trust in e-payment systems. Electron Commer Res Appl 2010;9(1):84–95.

Kitchenham B. 2004. Procedures for performing systematic reviews. Keele University, UK.

Kitchenham B, Charters S. 2007. Guidelines for performing systematic literature reviews in software engineering. Keele University, UK.

Kitchenham B, Pearl Brereton O, Budgen D, Turner M, Bailey J, Linkman S. Systematic literature reviews in software engineering–a systematic literature review. Inf Softw Technol 2009;51(1):7–15.

Kitchenham B, Pretorius R, Budgen D, Pearl Brereton O, Turner M, Niazi M, et al. Systematic literature reviews in software engineering–a tertiary study. Inf Softw Technol 2010;52(8):792–805.

Konchitchki Y, O'Leary DE. Event study methodologies in information systems research. Int J Account Inf Syst 2011;12(2):99–115.

Leung A, Bose I. 2008. Indirect financial loss of phishing to global market. In Proceedings of ICIS.

Liginlal D, Sim I, Khansa L. How significant is human error as a cause of privacy breaches? An empirical study and a framework for error management. Comput Secur 2009;28(3):215–28.

Liu Q, Zhang Y. VRSS: a new system for rating and scoring vulnerabilities. Comput Commun 2011;34(3):264–73.

Liu Q, Zhang Y, Kong Y, Wu Q. Improving VRSS-based vulnerability prioritization using analytic hierarchy process. J Syst Softw 2012;85(8):1699–708.

Malkiel BG. The efficient market hypothesis and its critics. J Econ Perspect 2003;17(1):59–82.

Mell P, Scarfone K, Romanosky S. 2007. A complete guide to the common vulnerability scoring system version 2.0. In Published by FIRST-Forum of Incident Response and Security Teams (pp. 1–23).

Modi SB, Wiles MA, Mishra S. Shareholder value implications of service failures in triads: the case of customer information security breaches. J Oper Manag 2015;35:21–39.

Morse EA, Raval V, Wingender JR Jr. Market price effects of data security breaches. Inf Secur J Glob Perspect 2011;20(6):263–73.

Muntermann J, Roßnagel H. On the effectiveness of privacy breach disclosure legislation in europe: empirical evidence from the US stock market. In: Proceedings of the 14th Nordic conference on secure IT systems: identity and privacy in the internet age. Springer-Verlag; 2009. p. 1–14. doi:10.1007/978-3-642-04766-4_1.

Ngai EW, Wat FKT. A literature review and classification of electronic commerce research. Inform Manag 2002;39(5):415–29.

NVD. <http://nvd.nist.gov/>; 2015 [accessed 27.09.15].

Patel N. The effect of IT hack announcements on the market value of publicly traded corporations. Duke J Econ 2010;22.

Pirounias S, Mermigas D, Patsakis C. The relation between information security events and firm market value, empirical evidence on recent disclosures: an extension of the GLZ study. J Inf Secur Appl 2014;19(4):257–71.

Radjenović D, Heričko M, Torkar R, Živković A. Software fault prediction metrics: a systematic literature review. Inf Softw Technol 2013;55(8):1397–418.

Roztocki N, Weistroffer HR. 2008. Event studies in information systems research: a review. In Proceedings of the Fourteenth Americas Conference on Information Systems.

Roztocki N, Weistroffer HR. 2009a. Event studies in information systems research: an updated review. In Proceedings of the Fifteenth Americas Conference on Information Systems.

Roztocki N, Weistroffer HR. 2009b. Stock market reaction to information technology investments: Towards an explanatory model. Proceedings of the European Conference on Information Systems.

Roztocki N, Weistroffer HR. 2011. Event studies in information systems research: Past, present and future. In Proceedings of the European Conference on Information Systems.

Shaikh AA, Karjaluoto H. Mobile banking adoption: a literature review. Telemat Inform 2014;32(1):129–42.

Smith KT, Smith M, Smith JL. Case studies of cybercrime and their impact on marketing activity and shareholder value. Acad Market Stud J 2011;15(2):67–81.

Spanos G, Angelis L. Impact metrics of security vulnerabilities: analysis and weighing. Inf Secur J Glob Perspect 2015;24(1–3):57–71.

Spanos G, Sioziou A, Angelis L. WIVSS: a new methodology for scoring information systems vulnerabilities. In: Proceedings of the 17th panhellenic conference on informatics. ACM; 2013. p. 83–90. doi:10.1145/2491845.2491871.

Telang R, Wattal S. An empirical analysis of the impact of software vulnerability announcements on firm stock price. IEEE T Software Eng 2007;33(8):544–57.

Wang P. Chasing the hottest IT: effects of information technology fashion on organizations. MIS Q 2010;34(1):63–85.

Wang T, Ulmer JR, Kannan K. The textual contents of media reports of information security breaches and profitable short-term investment opportunities. J Organ Comput Electron Commer 2013;23(3):200–23.

Wang Y, Yang Y. PVL: a novel metric for single vulnerability rating and its application in IMS. J Comput Inf Syst 2012;8(2):579–90.

Yayla AA, Hu Q. The impact of information security events on the stock value of firms: the effect of contingency factors. J Inf Technol 2011;26(1):60–77.

Zhang L, Huang J. The review of empirical researches on IT investment announcements on the market value of firms. Int J Bus Manag 2009;4(10):P14.

Zhang Y, Deng X, Wei D, Deng Y. Assessment of E-commerce security using AHP and evidential reasoning. Expert Syst Appl 2012;39(3).

---

**Footnotes:**
1. http://www.sciencedirect.com
2. http://citeseerx.ist.psu.edu
3. http://ieeexplore.ieee.org
4. https://webofknowledge.com
5. http://www.scopus.com
6. http://www.cnet.com

**Author Information:**

**Georgios Spanos** was born in Thessaloniki. He received his BSc degree in Informatics and his MSc degree in Informatics and Management from Aristotle University of Thessaloniki (AUTh). He is currently a PhD Candidate in Informatics and a Research Associate in Statistics and Information Systems Lab, Department of Informatics, AUTh.

**Lefteris Angelis** studied Mathematics and received his PhD degree in Statistics from Aristotle University of Thessaloniki (AUTh). He is currently an Associate Professor at the Department of Informatics of AUTh and coordinator of the STAINS (Statistics and Information Systems) research group. His research interests involve statistical methods with applications to information systems and software engineering, computational methods in mathematics and statistics, planning of experiments and simulation techniques.