# Where is IT in Information Security? The Interrelationship among IT Investment, Security Awareness, and Data Breaches

**Authors:** Li, Wilson Weixun; Leung, Alvin Chung Man; Yue, Wei Thoo

**Published in:** MIS Quarterly  
**Published:** 01/03/2023  
**Volume:** 47, Issue 1, Pages 317-342  
**DOI:** 10.25300/misq/2022/15713

---

## Abstract

Data breaches can severely damage a firm's reputation and its customers' confidence. Firms must therefore continuously invest in security measures to prevent such breaches. However, the effectiveness of security investment has been questioned by both practitioners and academics. We illustrate the bidirectional dynamic relationship between information technology (IT) investment and data breaches moderated by threat and countermeasure security awareness using an eight-year panel of 311 U.S.-listed firms to provide empirical evidence that threat awareness broadens firms' scope for addressing data-breach issues by investing more in IT than in security. Countermeasure awareness equips firms with sufficient knowledge and experience to ensure effective implementation of IT, which provides more comprehensive protection than security investment alone. Our results suggest that firms should evolve beyond the reactive mindset of solely upgrading security and begin nurturing both threat awareness and countermeasure awareness to address the underlying IT system issues that are the cause of data breaches.

**Keywords:** Security investment, IT investment, security awareness, threat awareness, countermeasure awareness, data breach, panel vector autoregression model

---

## Introduction

In recent years, firms have rapidly increased their security budgets. However, the effects of the added funds appear to be marginal and data breaches continue to proliferate. This casts doubt on the effectiveness of investments in security protection in general, which range from activities such as conducting information security training to implementing identity access management technologies. Many security experts caution that firms are not spending their security budgets effectively and some researchers have suggested that poorly integrated security solutions can lead to diminishing security investment returns (Angst et al., 2017; Sen & Borle, 2015).

IT investment is considered to play an increasingly critical role in security for addressing fundamental or root-cause issues that lead to poor security management² (Chen et al., 2011; Hsu, 2009; Pang & Tanriverdi, 2022; Sun et al., 2006). Security professionals have suggested that inefficiencies and flaws in the underlying IT environment are to blame and advise scrutinizing IT investments after breach incidents to enhance the effectiveness of integrating IT and security objectives (DiPietro, 2018; Glavach, 2017; Morgan, 2015). However, others have found that it is insufficient to rely on IT investment to address security issues due to the fact that some firms treat security investment and IT investment as independent decisions (Coltman et al., 2015; Pang & Tanriverdi, 2022; Van Niekerk & Von Solms, 2010). Accordingly, it has been suggested that security awareness is the missing link in integrating comprehensive security solutions (Boss et al., 2009; Spears & Barki, 2010; Straub & Welke, 1998). Hence, we posit that security awareness serves a moderating role between firms' IT and security resource allocations and their security outcomes.

Security awareness—broadly defined as a unified sense of awareness of security threats and proper countermeasures at the senior management level—is vital to maintaining a firm's security. With a better understanding of security threats and potential business impacts, firms' key stakeholders are more willing to cooperate with security policies and proactively protect the security environment by exchanging information and providing support (Johnson & Goetz, 2007; Ruighaver et al., 2007). In addition, comprehensive mindfulness of threats also enhances a firm's security mindset by assessing a wider range of investments (e.g., IT investments) related to data breaches, which promotes changes in both security and IT investment strategies (Loft et al., 2021; Soomro et al., 2016; Straub & Welke, 1998). Moreover, a holistic understanding of countermeasures can help a firm explore practical solutions to avoid conflicts between security and business (Herath et al., 2020; McEvilley, 2002).

Using panel data for 311 U.S.-listed firms from 2010 to 2017, we examine the bidirectional relationships between IT investment, security investment, and data breaches using the panel vector autoregression (PVAR) model. We follow the approach proposed by Gordon et al. (2010) to capture the effect of security awareness, in which a firm's voluntary disclosure of security activities indicates its security awareness. We suggest that such awareness—categorized into threat and countermeasure awareness—strengthens the communications and collaborations between security and business functions, which helps develop a clear view of the threat landscape and devise suitable and practical solutions through IT and security. Thus, security awareness moderates the relationship between IT and security investment and security performance; we measure the latter measure in terms of the number of data breaches.

We find that threat awareness stimulates firms to invest more in IT than in security after data breaches, possibly because threat awareness broadens the scope at which firms can assess security threats, which makes them more likely to identify root causes stemming from the underlying IT systems. As a result, firms allocate more resources to IT rather than upgrading specific security measures. We also find that with more IT investment and a higher level of countermeasure awareness, firms can curb data breaches more effectively. One explanation is that countermeasure awareness presents firms with a holistic view of their interconnected IT systems so that firms can consolidate different resources to support the effective implementation of IT and security. Furthermore, redesigning IT systems to align with business and security provides more comprehensive protection than solely upgrading security measures. Accordingly, we demonstrate that security awareness plays an essential moderating role in firms' decisions on IT resource allocation and security performance.

---

## Hypothesis Development

### Security Investment: Mindset Trap in Treating the Symptoms

Firms often invest in security solutions when facing cybersecurity threats; such actions may influence future security performance. Addressing cybersecurity risk, conceptually speaking, involves a dyadic interaction between firms' investments and their security performance. In this study, we use breach incidents as the trigger for investments in security and IT. These investments, in turn, may affect the outcome of future breach incidents.

Although data breaches or other security incidents should motivate firms to enhance their security practices, previous studies reveal that firms often manage security with symbolic gestures. One contributing factor is that, without the benefit of hindsight, firms tend to take a myopic view of security incidents (Angst et al., 2017; Kwon & Johnson, 2014). Moreover, firms are under constant pressure to fulfill requirements from external entities such as regulatory bodies and business partners, which leads them to neglect fundamental security issues (Herath et al., 2020; Kwon & Johnson, 2018; Nazareth & Choi, 2015). Hence, the ways in which firms manage security threats may not be consistent with their fundamental security objectives due to common mindset errors.

Even when firms understand the need to achieve specific security objectives, the extant literature shows that not all types of security investment lead to better security performance (Panel A of Table A1 in Appendix A). Several factors explain these failures to implement effective security measures: (1) the misallocation of security budgets (Sen & Borle, 2015), (2) the inability to integrate security measures into organizational systems and processes effectively (Li et al., 2021; Tanriverdi et al., 2020), and (3) the inability to align employees with organizational security objectives (Kwon & Johnson, 2014; Li et al., 2021). These failures demonstrate that there may be gaps in how firms leverage resources to develop workable security solutions.

In summary, incoherent objectives and actions may lead to discrepancies between perceived and actual effectiveness in security investment; that is to say, firms often fall into the trap of treating the symptoms but not the root causes of data breaches.

### IT Investment: A Comprehensive Approach

Data breaches trigger firms to invest in security solutions, which may include not only security measures but also general IT investments. Previous studies have argued that incorporating IT into security solutions broadens firms' perspectives in dealing with security issues and hence serves as an essential component in effective security management (Chen et al., 2011; Hsu, 2009; Sun et al., 2006). Several facts further support this argument. First, IT aids firms in identifying and addressing vulnerabilities that arise from an inefficient and flawed IT design (Heidt et al., 2019; Herath et al., 2020; Hole & Netland, 2010; Kraemer et al., 2009; Loft et al., 2021). Second, creating strong IT infrastructures helps firms better integrate IT and security objectives (D'Arcy et al., 2009; Palanisamy et al., 2022; Silic et al., 2017). Third, various IT solutions can nurture a security culture among different business units when they are deployed to address security issues (Herath et al., 2020). In fact, security issues have often been found to be rooted in flawed IT implementation in practice (e.g., system glitches, misconfiguration, and human error/negligence). Nurturing a security culture can make employees more careful when planning, implementing, and using IT.

Previous studies (Kayworth & Whitten, 2010; Loft et al., 2021; Soomro et al., 2016) have highlighted the importance of aligning IT with security arrangements. Such studies note that information security is a process rather than a product, which requires constant alignment with the underlying environments (e.g., enterprise architecture) (Loft et al., 2021). Misalignment between IT and security objectives may weaken the deterrent effect of security measures (Li et al., 2020). Furthermore, some suggest that a security mindset in IT implementation is necessary to bridge the disconnect between IT and security initiatives³. Such a belief is consistent with previous research findings that an organizational-security mindset is a prerequisite for enhancing the effectiveness of security measures (Angst et al., 2017; Chang & Ho, 2006; Hsu et al., 2012).

In summary, previous research reveals that IT and the effectiveness of security measures are closely connected. Hence, treating IT and security as separate processes may not be ideal. Instead, a holistic and diverse understanding of the interplay between IT and security issues can more effectively address the fundamental causes of security breaches.

### The Moderating Role of Security Awareness

Our literature review suggests that designing suitable security measures requires a diverse knowledge base to connect a firm's security environment with its business processes (Boss et al., 2009; Spears & Barki, 2010; Straub & Welke, 1998). Such a comprehensive understanding is often referred to as a state of security awareness, which assists firms in aligning their evolving security objectives in dynamic business landscapes (Olt et al., 2019; Straub & Welke, 1998). A notable mechanism is that having security awareness can facilitate communication and collaboration among internal and external stakeholders in the internal audit and governance processes (Gelbstein, 2016; Ruighaver et al., 2007). For instance, security awareness can help improve IT and security governance (AlGhamdi et al., 2020; Fazlida & Said, 2015; Johnston & Hale, 2009) and strengthen collaboration between internal audit functions (IAF) and other business units (Islam et al., 2018; Steinbart et al., 2018). Security awareness can also encourage firms to prepare for adversarial actions through better internal audit and governance implementations (Berkman et al., 2018; Kark et al., 2009; Kwon & Johnson, 2014), which is often achieved by integrating sound security policies and practices into business routines (Barton et al., 2016; Hsu et al., 2012).

Previous studies have generally treated security awareness as a one-dimensional construct (Hsu et al., 2012; Kwon et al., 2012), thus overlooking the extensive role of security awareness in moderating firms' reactions to breach incidents. Essentially, there is a lack of research on the relationship between security awareness and the dyadic interaction between firms' investments and their security. In view of this gap, we argue that effective investments to address breach incidents involve two different kinds of security awareness. The first is that the organization is aware of potential threats and vulnerabilities related to possible breach incidents (Hanus & Wu, 2016; Herath et al., 2020; Zhuang et al., 2020); the second is that firms possess a deep understanding of IT solutions to devise appropriate security solutions (Gopalakrishna-Remani et al., 2019; Ravichandran, 2005).

We borrow concepts from user-level studies that draw on protection motivation theory (PMT) (Hanus & Wu, 2016; Olt et al., 2019) to further classify security awareness into threat awareness (TA) and countermeasure awareness (CA). TA encompasses businesses' mindfulness of local threats in their processes; such attention enables firms to identify their valuable digital assets and to promote effective security measures to protect them (Fenz et al., 2014; Olt et al., 2019). CA is a thorough understanding of the solutions available to address security concerns effectively. This, in turn, helps firms deploy appropriate solutions to meet their business objectives (Straub & Welke, 1998) by infusing the most suitable technologies into their business activities (Claybaugh et al., 2017; Malhotra & Galletta, 2005; Purvis et al., 2001).

By differentiating the concepts of TA and CA, our study expands on the conventional understanding of how security awareness (or a security mindset) moderates the relationship between data breaches and IT (or security) investment. Figure 1 presents the conceptual model.

![Figure 1. Conceptual Model](conceptual-model-placeholder)

#### The Moderating Effect of Threat Awareness

Data breaches (and their accompanying losses) may trigger firms to rethink their future investment strategies regarding IT and security (Lee & Larsen, 2009; Say & Vasudeva, 2020). As mentioned above, security awareness may affect senior management's evaluation of investments. Out of the two types of security awareness, TA is more directly associated with senior management's assessment of security-related threats (Olt et al., 2019). Therefore, different levels of TA may exert varying degrees of moderating effects on the relationship between data breaches and IT (or security) investment.

With strong TA, firms may adopt a more comprehensive approach to assessing their security threats (symptoms) and associated environment (Herath et al., 2020). Such an approach may extend the assessment beyond security measures adopted by the firm to the IT environment where security measures reside (Johnson et al., 2007). In fact, some security issues may not be easily addressed by fixing the symptoms (e.g., adopting the latest security measures) (Loft et al., 2021). The root causes of data breaches (e.g., human errors in manual processes; legacy or incompatible systems) may stem from the underlying IT environment (Cram et al., 2019; Kraemer et al., 2009). Therefore, strong TA may trigger firms to scrutinize the underlying IT systems to identify the root causes rather than examining the related security measures alone. This argument is supported by Straub and Welke (1998), who found that a comprehensive understanding of the threat landscape, which includes extensive examination of existing IT systems, is necessary to effectively address security problems. Thus, firms may devote more resources to improving the core IT systems with particular attention paid to the prevention or mitigation of future data breaches. This type of reaction differs from a narrow focus on allocating more security resources to specific security measures to solve particular security problems.

Differences in TA may trigger firms to adopt different IT investment strategies when facing significant security problems (e.g., data breaches) (Loft et al., 2021; Soomro et al., 2016). Hence, we posit that TA motivates firms to allocate more resources toward IT investment than security investment as mindful firms could be more inclined to consider an extensive range of solutions, including IT. To this effect, we propose the following hypothesis:

**H1: Threat awareness positively stimulates the positive effect of data breaches on IT investment more than security investment.**

#### The Moderating Effect of Countermeasure Awareness

Devoting more resources (IT or security) to deterring security-related threats may lead to a greater reduction in data breaches. However, the degree of effectiveness may hinge on senior management's awareness of appropriate resources or solutions to neutralize threats. This argument is supported by previous research, which shows that without awareness of the complexity and interdependency of these interconnected systems, firms may be unable to fully address security risks even if senior managers dedicate considerable resources to mitigating such risks (Li et al., 2021; Tanriverdi et al., 2020). In this case, CA may be the missing link that helps firms effectively leverage IT and security resources to devise practical solutions (Herath et al., 2020; McEvilley, 2002). We argue that CA equips firms with the necessary knowledge and experience to consolidate their resources (e.g., human resources, knowledge management), such that IT and security implementation is more effective in preventing security problems (Herath et al., 2020; Hirt & Swanson, 2001; Purvis et al., 2001; Somers & Nelson, 2004).

We also posit that IT investments made by countermeasure-aware firms deter more breaches than security investments for various reasons. First, IT revamped with embedded security features may provide more comprehensive protection than vulnerable systems with security patches (Baskerville, 2009; Herath et al., 2020). Furthermore, redesigning IT to align business and security is more likely to resolve the root causes of security issues, e.g., human errors or security violations, than solely upgrading security measures (Sarkar et al., 2020; Silic & Lowry, 2020; Tarafdar et al., 2015). Thus, we propose the following hypothesis:

**H2: Countermeasure awareness positively stimulates the negative effect of IT investment on data breaches more than the effect of security investment.**

---

## Data and Methodology

### Data Description

We collected three types of data—data breaches, security investment budgets, and IT investment budgets—from different sources, which are discussed below.

#### Source of Data Breach Information

We collected data on reported breaches from the Privacy Rights Clearinghouse (PRC) database4, which has been widely used in similar research (Angst et al., 2017), and aggregated all breach incidents for each firm on an annual basis in our analysis. We also used the number of breached records5 to better capture the seriousness and magnitude of the data breach events.

#### Source of Security and IT Investment Information

We obtained the data on IT investment budgets from the Computer Intelligence Technology Database (CiTDB) of Harte-Hanks Market Intelligence. This database contains detailed annual IT investment information, including that of Fortune 1,000 companies gathered through surveys and interviews. The database has been widely used in information systems (IS) studies (Arora & Forman, 2007; Forman, 2005), and we aggregated these site-level data to the firm level. We used the weighted average of IT budgets with the number of employees at the site level as a weight to characterize the overall IT investment made by a firm. In the same way, we used the weighted average of security budgets6 with the number of employees at the site level as a weight to measure security investment.

#### Data and Measures of Firms' SA

To capture security awareness at the senior management level, we collected annual 10-K reports from firms listed by the Securities and Exchange Commission (SEC). For each firm with an annual 10-K report, we checked whether the firm had disclosed any security threats or identified any risk-related factors or security update activities in the corresponding fiscal year. The self-disclosure of information-security activities underscores the senior executives' level of attention to protecting information assets and positively affects firms' market value (Berkman et al., 2018; Chai et al., 2011; Gordon et al., 2010). Steelman et al. (2019) used a similar approach to capture firms' emphasis on or commitment to IT. Similarly, a firm's voluntary disclosure of security activities can serve as a proxy for its security awareness at the senior management level.

Following the methods used by Gordon (2010), we identified annual 10-K reports that contained at least one cybersecurity-related keyword7. Based on previous studies (Berkman et al., 2018; Steelman et al., 2019), we further constructed the level of awareness by counting the number of keywords in the reports. We regard the voluntary disclosure of security threats in the 10-K reports as a sign that the firm was aware of potential security threats, which we refer to as TA. The interaction term Breach × TA thus captures the moderating effects of TA on a firm's efforts. The voluntary disclosure of security activities in the 10-K reports also signals a firm's commitment to actively preventing security breaches, which we refer to as CA. Thus, the interaction term IT (Security) × CA captures the moderating effect of CA when firms implement IT (security) investment. Examples of security awareness as seen in the annual reports in terms of threats and countermeasures are provided in Appendix F.

We further collected data on exogenous variables, including firms' total assets and advertising expenditures from Compustat, search volume growth rate8 from Google Trends, and the number of issued patents from Google Patent, which were used to control for firm size (Dewan et al., 1998) and performance (Aral & Weill, 2007), online popularity (Burtch et al., 2013)?, and capability (Vandaie & Zaheer, 2014), respectively.

After matching the data from the various sources, we identified 160 U.S. firms (treated firms) that experienced breaches between 2010 and 2017 and for which data were available across all the datasets during the observed period. To control for selection bias and ensure a consistent model estimation, we used propensity score matching (PSM) to construct a control group of firms with no breaches from 2010 to 2017. PSM has been widely used in other IS research (Chang & Gurbaxani, 2012) to control for the selection bias issues caused by observed heterogeneity. For example, fundamental differences between treatment and control firms, such as online popularity and firm size, may affect the likelihood that firms will be breached and influence their investment budgets in both IT and security.

Following the standard PSM procedure (Chen et al., 2015; Kim et al., 2016), our control firms were selected from among firms having no data breaches during the observed time period (2010-2017). In the matching process, we used data for the year before the breach incident. We applied a probit model where the dependent variable (whether a firm has been breached from 2010 to 2017) is binary. We used variables such as total assets, advertising expenditures, and Google Patent and Google Trend ratios to control for firm size, firm capability, and online popularity, which may influence the likelihood of data breaches. To obtain more accurate estimation results of firms' reactions, we matched firms by industry (based on the Fama-French 10 industries). We then calculated the estimated propensity score based on the regression results of the probit model and used the nearest-neighbor method to match each treated firm with a counterpart that has never been breached. Meanwhile, we set the caliper (the maximum allowable difference between two participants) to equal to or less than 0.05. Over 90% of treatment firms were successfully matched, providing a total of 166 control firms and 145 treatment firms as the final sample¹°.

After implementing PSM, we ran a t-test to check the similarity of the matching results by comparing the means of each matching characteristic variable in the treatment and matched groups. As shown in Table 1, the PSM matching variables between the two groups are not significantly different from each other after matching, suggesting that they are statistically balanced.

### Model

#### The Rationale for Using a Panel Vector Autoregression Model

A vector auto-regression (VAR) model can be used to test models with undefined or hard-to-define restrictions, such as causality (Backus, 1986). Each variable is expressed as a linear function of its own lagged values, the lagged values of other variables, and an uncorrelated error term. Panel VAR (PVAR) adds a cross-sectional dimension to the standard VAR model and can be used to examine the relationships in a system of interdependent variables without imposing ad hoc model restrictions (Dewan & Ramaprasad, 2014). Exogenous variables that influence endogenous variables can also be incorporated into the model, allowing us to address unobserved individual heterogeneity (Chen et al., 2015), thus complementing the PSM approach, which, as mentioned above, only considers observed heterogeneity issues.

Endogenous relationships (two-way causal relationships)—such as that between a firm's number of data breaches, its IT (or security) investment budget, and its level of security awareness—may exist between variables. For example, previous studies have documented that prior breach experience affects the likelihood of future breaches and investment decisions through the following competing mechanisms: (1) signaling a lower level of security control, thus attracting more adversaries and increasing the likelihood of a breach (Wang et al., 2015), and (2) revealing vulnerabilities, thus inducing firms to implement proper solutions and reducing the likelihood of a breach (Lankton et al., 2021). PVAR is an appropriate tool because it can model bidirectional and dynamic relationships and requires no restrictions or causal assumptions. This approach has been used to resolve endogeneity issues in prior IS research (Carlo et al., 2012). The model specification is as follows:

$$y_{i,t} = \begin{pmatrix} 
Breach_{i,t-s} \\
Investment_{i,t-s} \\
Security\ Awareness_{i,t-s} \\
Interaction\ Term_{i,t-s}
\end{pmatrix} = \sum_{s=1}^{p} \Phi_s \cdot \begin{pmatrix}
Breach_{i,t-s} \\
Investment_{i,t-s} \\
Security\ Awareness_{i,t-s} \\
Interaction\ Term_{i,t-s}
\end{pmatrix} + \beta \cdot \begin{pmatrix}
Revenue_{i,t} \\
Google\ Trend\ Ratio_{i,t} \\
Expenditure\ in\ Advertisement_{i,t} \\
Number\ of\ Patents\ Issued_{i,t}
\end{pmatrix} + \varepsilon_{i,t}$$

where $y_{i,t} = (Breach_{i,t}, Investment_{i,t}, Voluntary\ Disclosure_{i,t}, Interaction\ Term_{i,t})$ is a four-element column vector for firm $i$ at time $t$ containing the log transformation of the dependent variables, Investment refers to security investment or IT investment, Voluntary Disclosure represents levels of security awareness of either threats or countermeasures, Interaction refers to either Breach × TA or Investment × CA, $\Phi_s$ and $\beta$ are the matrices of the slope coefficients for the endogenous variables, and $p$ is the number of lags.

Following previous PVAR studies, we selected the optimal lag order based on information criteria such as Akaike's information criterion (AIC), the Bayesian information criterion (BIC), and the Hannan and Quinn information criterion (HQIC). The lowest AIC, BIC, and HQIC statistics across 1-4 year lags indicate that the one-year lag is the best lag order for model estimation, as shown in Table 4. The four-element column vector for firm $i$ at time $t$ (ATi,t, Google Trend Ratioi,t, Expenditure in Advertisementi,t, Number of Patents Issuedi,t) controls for firm size, online popularity, advertising expenditure, and firm capability. To control for heteroskedasticity (Kim et al., 2016), we used robust standard errors clustered by industry.

To examine the stationarity of this panel dataset, we conducted the Phillips-Perron (1988) test and the augmented Dickey-Fuller (ADF) (1979) test. The null hypothesis is that all panels contain unit roots. The results in Table 5 show that the null hypothesis was rejected for each time-series variable; there is no unit root and all of the endogenous variables are stationary.

Following prior research using PVAR (Dewan & Ramaprasad, 2014), we also conducted the Granger (1969) causality test. The null hypothesis is that the excluded variable cannot Granger-cause the equation variable. As Table 6 shows, the interaction term Breach × TA can Granger-cause IT investment (p < 0.10), and the interaction term IT × CA can Granger-cause Breach (p < 0.01). The results show clear evidence of a bidirectional relationship among data breach, investment, and the interaction terms (IT × CA, Breach × TA), which supports the use of a dynamic model to address the endogeneity issues between the explanatory variables.

---

## Results and Discussion

### With Heightened Threat Awareness, Data Breaches Stimulate More IT Investment than Security Investment

We first examine the interrelationship among security investment, data breaches, and security awareness when controlling for firm size, advertising expenditure, online popularity, and capability. Table 7 shows the estimation results.

The lagged Breach × TA has a negative and nonsignificant effect (coefficient: -0.002) on security investment, as shown in Column 2 of Table 7¹². Our explanation is that these firms may attempt to avoid complicating their systems and refrain from adding further unnecessary security measures. Alternatively, they may explore a wider range of solutions and identify more efficient approaches (Spears & Barki, 2010). Sen and Borle (2015) suggest that firms should rely on both technical solutions and administrative or physical controls to fully enhance their security capabilities, which are typically not covered by conventional security measures.

Next, we investigate the interrelationship among IT investment, data breaches, and security awareness. As shown in Column 4 of Table 7, the lagged Breach × TA has a positive and significant effect (coefficient: 1.121, p < 0.10) on IT investment, suggesting that firms with greater TA invest more in general IT after identifying security vulnerabilities. This result highlights the importance of using IT to address security incidents for threat-aware firms, which commonly occurs in practice. For example, after its high-profile breach in 2013, Target Corp. underwent a massive upgrade of its in-store payment infrastructure to support the use of the more-secure chip-and-PIN credit cards. A comparison test¹³ of the corresponding coefficients between security investment and IT investment indicates a significant between-group difference (t = 70.02; p < 0.001). The coefficient of Breach × TA for IT investment is significantly larger than that for security investment, which supports H1 that threat-aware firms invest more in IT than in security measures after data breaches.

### With Heightened Countermeasure Awareness, IT Investment Deters More Data Breaches than Security Investment

We further investigate the impact of security and IT investment on breaches, and, as Column 1 of Table 7 indicates, the lagged Security × CA shows no significant effect on breaches (coefficient: -0.030). Thus, there is no evidence that security investment alone can effectively deter data breaches, even when firms are security aware. Although surprising, this result gives credence to doubts regarding the effectiveness of independent security spending as higher budgets do not necessarily lead to fewer data breaches (Sen & Borle, 2015). Our findings support the argument that security investment is only one factor, often a secondary factor, in an overall security solution strategy.

In examining the impact of general IT investment on security performance, we found that CA has an important moderating role. The lagged IT × CA shows a significantly negative effect (coefficient: -0.043, p < 0.01) on Breach, as shown in Column 3 of Table 7. Thus, the importance of CA is demonstrated by the fact that firms with higher levels of CA outperform those with lower levels of CA in preventing data breaches. Their awareness means that they attempt to minimize the potential negative effects of data breaches through their IT solutions. This demonstrates not only the importance of IT solutions in combatting security incidents but also, more importantly, that security awareness plays a significant role in achieving this objective. We conducted a comparison test to compare the coefficients between the security and the IT models. The result indicates a significant between-group difference (t = -10.04; p < 0.001). The coefficient of the lagged IT × CA on breaches is significantly larger than that of the lagged Security × CA, which supports H2 that countermeasure-aware firms exploit IT, rather than security measures alone, to effectively combat data breaches.

---

## Conclusion

Data breaches have significantly negative impacts on firm value (Gwebu et al., 2018), thus prompting firms to carefully consider data protection and increase their security investment budgets. However, breaches persist, which reveals that there may be shortcomings in the mainstream security strategies. This study illustrates the dynamic relationship between IT (security) investment, security awareness, and data breaches: threat-aware firms react to security breaches by allocating more resources to IT than to security alone and countermeasure-aware firms use IT solutions more effectively to reduce data breaches.

### Theoretical Contributions

Our findings have important implications for the information security literature. First, our results demonstrate that threat-aware firms scrutinize the impact of general IT strategies on security protection after data breaches. We enrich the existing information-security literature by offering empirical evidence to support the necessity of examining firms' security efforts beyond the scope of conventional security measures, which advances the recent discussions on the narrowness of the existing definition and measurement of security investment in empirical studies (Kwon & Johnson, 2014; Li et al., 2021). Our work contributes to the security management literature by identifying TA as the factor that alters firms' security mindsets so that they no longer consider security and IT to be mutually exclusive. This is a novel insight, as prior research has confined the reach of security awareness to the domain of security strategies (Hsu et al., 2012; Kwon et al., 2012; Olt et al., 2019). Notably, our study disrupts this inertial thinking by demonstrating that TA extends to IT strategies.

Second, we demonstrate that sufficient knowledge or experience of countermeasures enables effective implementation of IT investment, which provides more comprehensive security protection than security investment. This finding enriches our understanding of the effect of IT investment on security outcomes, which was highlighted as a burden in prior empirical studies (Li et al., 2021; Zhang et al., 2019). Our results highlight the importance of CA in devising practical solutions to align IT and security objectives. Our results also challenge the assumption that security performance is a direct consequence of security investment (Gordon & Loeb, 2002; Wang et al., 2008). The insignificant effect of security investment, regardless of CA, is already supported by some prior findings (Loft et al., 2021; Sen & Borle, 2015). We deepen the understanding of the ineffectiveness of conventional security measures by contrasting security investment with IT investment. Our results reveal that security measures likely treat only symptoms, whereas a thorough assessment and revamping of the underlying IT systems can address the root causes of security issues.

Third, our findings show that security awareness leads to firms' emphasizing IT strategies as the foundation of addressing security issues. Hence, the "security-by-antiquity" approach¹4 may not be the best strategy—firms should instead focus on IT modernization (Pang & Tanriverdi, 2022). This insight echoes observations that security awareness can enhance the internal auditing and security governance process (Gelbstein, 2017; Hartmann & Carmenate, 2021; Ruighaver et al., 2007). Thus, security awareness facilitates better protection through IT and security investments that are responsive to the threat and protection environment.

Altogether, our work closes the loop between investment decisions and security performance and sheds light on the mechanisms underlying the role of security awareness in improving firms' security performance. Unlike recent studies that focus on other types of static or non-security-centric moderating factors (Angst et al., 2017; Kwon & Johnson, 2018), we demonstrate the importance of TA and CA in firms' ongoing attempts to address the root causes of security issues with the comprehensive assessment of the threat landscape and the effective implementation and integration of IT solutions.

### Managerial Contributions

From the managerial perspective, our findings on the importance of IT solutions for security performance have been echoed by many security practitioners. According to a recent survey, many frontline security-related duties are conducted by organizations' IT personnel, implying that IT teams can fundamentally influence security performance. The business value of IT investment has increasingly been linked to security performance through the enforcement of cybersecurity requirements for IT service and product providers, including cybersecurity in due-diligence considerations in M&A transactions. Our empirical results extend these arguments by demonstrating the importance of instilling security awareness among IT personnel to effectively curb data breaches.

Our results also demonstrate that security awareness has a two-way effect on the identification of appropriate IT resources as well as the proper implementation of IT solutions to remediate breaches. Although most senior managers realize the importance of paying attention to security threats, lacking the awareness of proper solutions (e.g., IT resources, security policies) or failing to deliver the message to middle-level managers often results in a narrow scope of security strategies and the unsuccessful remediation of data breaches (Ruighaver et al., 2007). To bridge these gaps, we suggest that firms take initial steps to reduce collaboration hurdles among different business units by improving security governance (Gelbstein, 2016) and expanding internal audit capabilities (Kahyaoglu & Caliyurt, 2018). By so doing, security solutions can be better designed and delivered with greater stakeholder participation (Fazlida & Said, 2015). This would also encourage employees to gain a better grasp of the changing threat landscape so that they can devise suitable solutions (Ruighaver et al., 2007). Furthermore, we suggest that policy makers take proactive approaches to provide relevant knowledge and monetary incentives to foster the adoption of updated IT solutions and security practices, especially for small- and medium-sized enterprises (SMEs).

### Limitations and Future Directions

We conclude by identifying some limitations of our study and directions for future research. To the best of our knowledge, ours is the first study to connect IT investment with security performance. In future studies, scholars could investigate the antecedents of the disconnect between IT and security. One limitation is that our dataset is relatively small and restricted to U.S. listed firms, as it is constrained by the data sources. Our findings could be verified in future research using SMEs or firms outside the U.S. In terms of the business value of IT investment for security performance, identifying the specific IT investments that can reduce particular types of security incidents would be beneficial¹5. We also acknowledge that measuring security awareness based on firms' disclosure of security activities may not be a perfect method. Future studies might consider developing a more comprehensive representation of firms' security awareness.

---

## Tables and Figures

### Table 1. Summary Statistics and Covariate Comparison Before and After Matching

| Variable | Mean | t-stat (p-value) | Treated | Control |
|----------|------|------------------|---------|---------|
| Total asset | Unmatched | 13.20 (0.000) | 9.115 | 6.898 |
| | Matched | 0.66 (0.508) | 8.898 | 8.750 |
| Advertising expenditure | Unmatched | 13.67 (0.000) | 2.544 | 0.850 |
| | Matched | -1.05 (0.296) | 2.186 | 2.496 |
| Google patents | Unmatched | 5.20 (0.000) | 1.036 | 0.546 |
| | Matched | 0.49 (0.627) | 0.884 | 0.810 |
| Google trend ratio | Unmatched | 0.71 (0.477) | -0.050 | -0.068 |
| | Matched | 0.21 (0.835) | -0.045 | -0.052 |

### Table 2. Summary Statistics

| Variable | Obs | Mean | SD | Min | Max | Remark |
|----------|-----|------|----|----|-----|--------|
| Breach | 2,411 | 1.643 | 62.075 | 0.000 | 3000.000 | Total breaches (in million records) |
| IT | 2,411 | 33.174 | 201.683 | 0.000 | 5882.421 | Weighted average IT budget (in millions of dollars) |
| Security | 2,411 | 0.126 | 1.039 | 0.000 | 25.423 | Weighted average security budget (in millions of dollars) |
| Threat awareness (TA) | 2,411 | 35.756 | 38.438 | 0.000 | 336.000 | Firm's voluntary disclosure of security threats (total number of keywords) |
| Countermeasure awareness (CA) | 2,411 | 17.937 | 35.943 | 0.000 | 336.000 | Firm's voluntary disclosure of security countermeasures (total number of keywords) |
| Total assets | 2,411 | 39279.14 | 171314.5 | 11.487 | 2261780.000 | Firm's total assets (in millions of dollars) |
| Ad | 2,411 | 126.532 | 427.433 | 0.000 | 6317.000 | Advertising expenditure (in millions of dollars) |
| GTrGrt | 2,411 | -0.021 | 0.297 | -0.731 | 5.579 | Growth rate of Google Trend volume |
| Patents | 2,411 | 22.068 | 105.4763 | 0.000 | 944.000 | Number of patents issued |

### Table 7. The Interrelationship of Security (IT) Investment, Security Awareness, and Data Breaches

| Independent variable | (1) Breach | (2) Security | (3) Breach | (4) IT |
|---------------------|------------|-------------|------------|--------|
| L.Breach | 0.503**(0.223) | -0.004(0.011) | 0.499*(0.277) | -0.512(0.487) |
| L.(Breach × TA) | -0.251(0.219) | -0.002(0.021) | -0.261(0.250) | 1.121*(0.678) |
| L.Security | -0.010(0.279) | 0.845***(0.234) | | |
| L.(Security × CA) | -0.030(0.054) | 0.084*(0.050) | | |
| L.IT | | | 0.023(0.119) | -0.143(1.960) |
| L.(IT × CA) | | | -0.043***(0.009) | 0.128(0.427) |
| L.CA | -0.007(0.013) | 0.022(0.019) | -0.167***(0.035) | 0.481(2.746) |
| L.TA | -0.021*(0.012) | 0.002(0.008) | -0.018(0.019) | -0.042(0.164) |
| N | 1789 | 1789 | 1789 | 1789 |

*Note: Standard errors are in parentheses; p-values are represented by * p < 0.10, ** p < .05, and *** p < 0.01; L indicates a lagged one-year term*

---

## Footnotes

¹ H. Raghav Rao was the accepting senior editor for this paper. Nirup Menon served as the associate editor. Wei Thoo Yue is the corresponding author.

² These may include, for example, human errors in manual processes, legacy, or incompatible systems.

³ Practitioners coined this as "security by design" to reflect the importance of considering security even in the earliest stages of IT design (Lovejoy, 2020).

4 The PRC provides information on data breaches related to a range of organizations (businesses, educational institutions, governments, the military, medical providers, and nonprofit organizations) from the U.S., which are collected mainly from the list servers of the Open Security Foundation (DataLossDB.org), Databreaches.net, PHI Privacy and NAID, and the California Attorney General's list of data breaches.

5 Like other recent empirical studies on cybersecurity (Angst et al., 2017; Kwon & Johnson, 2014; Sen & Borle, 2015), our reliance on reported breaches is a limitation of our study.

6 As security budgets are not available in CiTDB, we calculate security budgets using a weighted formula based on security software and services adoption.

7 The keyword lists are shown in Table A2 of Appendix A. Over 80% of our original keywords are covered in widely used cybersecurity-related parlance (Ayala, 2016).

8 We calculate the Google Trends search volume growth rate for each firm by dividing the difference between a firm's Google Trends search volume in the current year added to its search volume in the previous year by the firm's search volume in the previous year.

? With a larger internet presence, a firm can become a more obvious and attractive target for adversaries (Ransbotham & Mitra, 2009).

¹° We have 2,411 firm-year observations and 10 variables in the regression, which satisfies the rule of thumb that ten times more observations than the number of variables is sufficient for multiple regression analysis, as noted in the extant literature (Sekaran & Bougie, 2003).

¹¹ The summary table is available upon request.

¹² Our subsample analysis of hi-tech firms shows that Breach × TA has a positive and significant effect on security investment. This finding corroborates with prior findings (e.g., Zhuang et al., 2020) that the security vulnerabilities or even the awareness of the vulnerabilities are prerequisites but not sufficient conditions of firms' incremental adoption of security measures.

¹³ The comparison test was performed based on the formulae employed in Keil et al. (2000). Tan et al. (2014) also used the same approach to compare coefficient estimates of different models.

¹4 A "security-by-antiquity" mindset means that firms consider legacy IT systems to be more stable and believe that upgrading to modernized systems is risky and insecure.

¹5 For example, an efficient human resources system may help reduce insider threats by enabling better oversight of employees' rights to access and control.