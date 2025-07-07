# Health-Care Security Strategies for Data Protection and Regulatory Compliance

**Author(s):** Juhee Kwon and M. Eric Johnson  
**Source:** Journal of Management Information Systems, Vol. 30, No. 2, Information Economics and Competitive Strategy (Fall 2013), pp. 41-65  
**Published by:** Taylor & Francis, Ltd.  
**Stable URL:** https://www.jstor.org/stable/43590128  
**Accessed:** 25-06-2025 18:55 UTC  

**JSTOR Note:** JSTOR is a not-for-profit service that helps scholars, researchers, and students discover, use, and build upon a wide range of content in a trusted digital archive. We use information technology and tools to increase productivity and facilitate new forms of scholarship. For more information about JSTOR, please contact support.jstor.org. Your use of the JSTOR archive indicates your acceptance of the Terms & Conditions of Use, available at https://about.jstor.org/terms. Taylor & Francis, Ltd. is collaborating with JSTOR to digitize, preserve and extend access to Journal of Management Information Systems.

---

## Authors

**Juhee Kwon** is an assistant professor in the Information Systems Department at College of Business, City University of Hong Kong. Her research interests include information security, health-care IT, IT business values, and business-IT alignment. She earned a Ph.D. in management information systems from Krannert School of Management, Purdue University. Her research articles have appeared in academic journals such as *MIS Quarterly*, *Journal of the American Medical Informatics Association*, and *Journal of Information Systems*.

**M. Eric Johnson** is dean of the Owen Graduate School of Management at Vanderbilt University. He holds a Ph.D. in engineering from Stanford University. His teaching and research focuses on the impact of IT on the extended enterprise. Through grants from the National Science Foundation and the Department of Homeland Security, he is studying how IT improves process execution but also how security failures create friction throughout the extended enterprise. His recent book, *The Economics of Financial and Medical Identity Theft* (Springer, 2012), examines the security failures and economic incentives that drive identity theft. He has authored patents on interface design and has testified before Congress on information security.

---

## Abstract

This study identifies how security performance and compliance influence each other and how security resources contribute to two security outcomes: data protection and regulatory compliance. Using simultaneous equation models and data from 243 hospitals, we find that the effects of security resources vary for data breaches and perceived compliance and that security operational maturity plays an important role in the outcomes. In operationally mature organizations, breach occurrences hurt compliance, but, surprisingly, compliance does not affect actual security. In operationally immature organizations, breach occurrences do not affect compliance, whereas compliance significantly improves actual security. The results imply that operationally mature organizations are more likely to be motivated by actual security than compliance, whereas operationally immature organizations are more likely to be motivated by compliance than actual security. Our findings provide policy insights on effective security programs in complex health-care environments.

**Key Words and Phrases:** compliance, data breach, health care, organizational maturity, security.

---

## Introduction

Electronic Health Records (EHRs) have been identified as a key enabler of both healthcare quality improvement and cost reduction. The HITECH Act of 2009 created billions of dollars in incentives for health-care providers to implement EHRs. However, with more records moving into digital form, security of patient data has become a significant concern. As Fichman et al. [25] note, patient data are highly personal, compounding the public fears of data breaches. Accordingly, as part of the HITECH Act, the U.S. Department of Health & Human Services (HHS) implemented a new breach notification regime that requires health-care organizations to publicly post breach announcements, both in local news outlets and on the HHS Web site, for any data losses affecting 500 or more individuals. The HHS also increased the severity of fines for HIPAA (Health Insurance Portability and Accountability Act) violations—both for inadvertent and willful disclosure of unsecured patient information. These new penalties, ranging up to $1.5 million, are linked to the severity of the violation. Likewise, many states have implemented breach notification laws over the past decade [58].

The new regulatory mandates and public concern have dramatically increased the pressure on health-care providers to secure patient data and comply with regulations. Actual data security and compliance seem like natural partners. But this partnership raises an interesting causality question: Which one drives the other? Whatever the driver, both are important because breaches and noncompliance both cause significant reputational damage, remediation costs, or penalties. Thus, firms must invest in both security and compliance. However, questions remain concerning the effectiveness of different security resources and their impact on actual security and compliance [17, 19, 48]. It was shown that in the first two years of HHS breach reporting, over 10 million patients' data were exposed—in many cases by hospitals that had made significant security investments [64].

The adoption of security practices to offset potential information risks is a major challenge for many organizations because information risks originate at different layers across an organization [10, 65]. Recently, researchers and practitioners have argued that security practices should be supported by organizational values that not only improve security awareness but also enhance individuals’ motivation to act responsibly and in accordance with firm policies [34, 50, 56]. Considering the heterogeneity of security practices and organizational values in the highly regulated space, organizations need to be more strategic in their approach to security and compliance, yet it has not always been clear what such an approach looks like in practice [35, 36, 37].

Building on the resource-based view of the firm, our objective is to identify how security resources (i.e., information technology [IT] security systems, prevention, and audit policies) affect actual security performance and perceived regulatory compliance and how the associations between security, compliance, and security resources vary with a health-care organization’s security operational maturity. In doing so, we sharpen the theoretical characterization of “security” and “compliance” by unpacking the effects of security resources and security maturity.

Our results show that the effects of security resources vary with outcomes (i.e., breach occurrence or compliance) and security operational maturity. Security resources seem to be more strategically planned and executed in operationally mature organizations, resulting in complementary effects. Furthermore, the causal link between security and compliance is different for operationally mature and immature organizations. In operationally mature organizations, breach occurrences hurt perceived compliance, but, surprisingly, compliance does not affect actual security. In operationally immature organizations, breach occurrences do not affect perceived compliance, whereas compliance significantly improves actual security. Reflecting on this causality dilemma, our findings suggest that operationally mature organizations are more likely to be motivated by breach occurrences than compliance, whereas operationally immature organizations are more likely to be motivated by compliance than actual security.

Our study makes practical and theoretical contributions to the literature on information security in several ways. First, our study provides a deep practical understanding of the security context, driven by both data protection and compliance. Our findings identify how security resources influence data protection and compliance based on an organization’s security operational maturity. Thus, our analysis provides policy insights on effective security programs in complex environments. Second, this study makes a theoretical contribution by providing evidence that security resources do not always have positive effects on actual security and compliance in the health-care context, where customers or patients are more elastic to reputation than price. Since both data breaches and noncompliance can tarnish a hospital’s reputation, health-care security decisions are more influenced by political or regulatory perspectives than economic perspectives. We empirically examine whether the health-care security context is in line with the predictions of the resource-based view. With the theory and empirical results in hand, we provide some answers to the question of whether the theoretical perspective oversimplifies security issues.

The rest of the paper is organized as follows. We review the relevant theoretical background and then propose our research hypotheses. Next, we describe the data collection and research methodology, followed by our results and discussion. Finally, implications and conclusions are presented.

---

## Theoretical Background

Our focus is to empirically identify the causal relationship between actual security and perceived compliance and the effects of security resources on data protection and compliance.

### Security and Compliance

There has been a very active debate regarding the causal link between actual security and compliance. First, drawing on fear appeal [36], researchers have argued that some degree of fear arousal induces managers’ motivations to alleviate possible threats. Since noncompliance and data breaches result in fines, public disclosure, stock price volatility, and loss of business, fears of these negative outcomes motivate organizations to take action to protect their data and comply with security regulations. Thus, while the fear of noncompliance punishments is a catalyst for improving actual security, fear of the potential loss arising from data breaches also motivates organizations to comply with regulatory requirements [12, 67].

Second, some researchers argue that involuntary actions forced by regulations induce organizations to just meet the specifics of compliance mandates [50, 56]. Such a “checkbox” approach to doing the minimum to meet the standards rarely, if ever, provides the kind of protection required to prevent a serious breach from occurring. Thus, although organizations have invested heavily in security practices in response to compliance drivers, these mandates may simply waste firm resources and create a compliance mind-set rather than a security mind-set.

Furthermore, breach experiences may influence perceived compliance, since managers often recognize noncompliant processes through a breach experience [23, 52]. However, security regulations also include requirements for postbreach remediation as well as breach prevention. Thus, although an organization may fail to comply with breach prevention requirements, if it complies with the postbreach remediation requirements, its perceived compliance may remain unharmed (e.g., postbreach compliance builds a feeling of overall compliance).

### Security Resources

In order to identify how security resources influence security performance and compliance, we employ the resource-based view of the firm. This view links organizational performance to resources [27, 69, 70]. It conceptualizes organizations as bundles of resources [42, 45] that are likely to be heterogeneously distributed due to differences in organizational capabilities [5, 44]. Such heterogeneity drives differences in organizational performance. The resource-based perspective provides a fundamental theoretical background for investigating how various security resources are associated with actual security and compliance.

Generally, firm resources include facilities, equipment, technology, human resources, or procedural practices. In the security context, security resources can be defined as security personnel, IT security applications, physical/technical equipment, or security procedures or policies. Thus, organizations with high security performance are likely to have more security resources [15, 30, 43].

### Security Operational Maturity

Researchers and practitioners have tried to assess organizational maturity in various management areas. Measuring the maturity of strategic choices and alignment practices makes it possible for an organization to see where it stands and how it can improve [24, 41]. Information systems (IS) researchers have argued that organizations must assess their own maturity in addition to the capabilities of IT resources to ensure the success of implementations, migrations, and major upgrades [11]. Organizational researchers have demonstrated that similar strategies using the same resources can result in diverse outcomes, leading them to conclude that it is difficult to know how resources contribute to performance without understanding organizational differences tied to their internalization [22, 44, 69]. These perspectives provide compelling theoretical reasons for investigating how security resources perform in organizations that exhibit different levels of security operational maturity [2, 51].

From a practice perspective, there are several maturity models that have been proposed to help organizations measure maturity, such as the capability maturity model (CMM) (http://cmmiinstitute.com) [47] and the privacy maturity model (PMM) [1]. For instance, the PMM measures an organization’s privacy practices accounting for legislative requirements, corporate policies, and the status of the organization’s privacy initiatives. The PMM uses five maturity levels: ad hoc, repeatable, defined, managed, and optimized. These levels can be further dichotomously categorized into the low (ad hoc, repeatable, and defined) and high levels (managed and optimized) based on whether the organization has a regular review process to assess the effectiveness of security-focused controls (e.g., [1, 6, 29]).

In our context, a key indicator of maturity is the existence of a regular review process to evaluate the security program. Although health-care organizations have made investments in security resources to fulfill regulatory checklists, their security operational maturity may affect security outcomes [38]. Recent surveys by industry groups and the HHS noted wide disparity in both security resources and compliance with federal (HITECH, HIPAA) and state regulations [40]. Thus, it would not be surprising if security resources perform differently based on security operational maturity [39].

---

## Hypotheses Development

While security regulations have evolved rapidly to address transparency and data protection, compliant organizations still experience security breaches. Although it is common to see organizations investing in security resources to achieve compliance, they often fail to proactively manage security exposure. Focusing on internal and external audits, the goal of proving compliance becomes the goal at the expense of holistically assessing, preventing, and mitigating risks [12, 70]. Even if all the regulatory requirements are met, malicious hackers can compromise a target by exploiting elements not addressed by the compliance standards.

While good compliance does not always result in good data protection, good data protection based on risk management leads to good compliance [14]. Organizations using a risk-based approach can reap the benefits of uniting compliance and risk management in a single solution. Nonetheless, organizations have to describe how whatever they are doing helps meet regulatory requirements; otherwise it is hard to acquire security budgets. So, many organizations start with compliance and work backward to security. Such an approach is the easy short-term path, since coping with uncertain risks is less straightforward than working to meet specific, measurable compliance goals. This path from compliance to actual data protection often appeals to immature organizations, which fear auditors more than attackers [46, 50]. On the contrary, mature organizations maintain security activities with their own security action plans rather than simply meeting regulatory requirements [18]. The analysis required for developing and reviewing a security action plan pushes the organization to consider unique potential security risks beyond routine compliance [55].

Thus, the path between actual security and compliance depends on security operational maturity and the effects of security resources [12, 13, 44]. An organization generally approaches security to suit to its own needs, realities of available resources, and operational maturity. This leads to the following:

- **Hypothesis 1a (The Maturity and Security Hypothesis):** An operationally mature organization is more likely to be motivated by actual security than by regulatory compliance.
- **Hypothesis 1b (The Maturity and Compliance Hypothesis):** An operationally immature organization is more likely to be motivated by regulatory compliance than by actual security.

According to the resource-based view, large organizations are likely to have more resources than small ones [43], such as IT security applications, procedures, and IT security staff. These differences produce heterogeneous outcomes such as regulatory compliance and breach occurrences [16]. With limited security budgets, organizations need to understand the most effective approach to achieving security and compliance goals while saving time and resources. Historically, organizations have followed technically focused strategies for designing effective information security solutions because security has been perceived to be a technical problem [66]. IT security equipment and applications are generally believed to improve an organization’s ability to monitor suspicious activities and prevent data breaches.

However, security is not just a technical but also a managerial problem. Thus, our study further includes the strategic importance of security procedural resources. Security education programs, policies, and procedures are available and useful in detecting and responding to information threats. Security procedural resources involve preventing security breaches and auditing all information flow controls [69]. In an analogous area of operations management, Ittner et al. [33] studied defect rates in manufacturing organizations and showed the impact of prevention and audit activities on quality performance. Likewise, the security context requires prevention and audit processes to detect and respond to information threats. With increased risks and more regulations, health-care organizations have increasingly implemented security resources, including IT security applications, prevention, and audit procedures.

Despite the widespread adoption of security resources, security threats and vulnerabilities continue to evolve with the rapidly changing technology. Given these challenges, today’s security problems are different from last year’s or even last month’s problems. Such shifting risks make it difficult for organizations or policymakers to know which security resources need to be adopted and the required path to better compliance and breach prevention. Thus, without regular reviews of security action plans, organizations adopting security resources with a compliance mind-set (check the box) often waste firm resources. Nevertheless, more resources should improve outcomes for both mature and immature health-care organizations because the healthcare industry lags in adoption of security technologies. Thus, we hypothesize:

- **Hypothesis 2a (The Security Resources in Mature Organizations Hypothesis):** The more security resources (i.e., IT security resources, prevention, and audit resources) that an operationally mature organization possesses, the better the security outcomes (i.e., fewer breaches and higher compliance).
- **Hypothesis 2b (The Security Resources in Immature Organizations Hypothesis):** The more security resources (i.e., IT security resources, prevention, and audit resources) that an operationally immature organization possesses, the better the security outcomes (i.e., fewer breaches and higher compliance).

In the security context, there is no single solution that can address every known and unknown security threat. Best practice indicates that successful security programs employ a multilayered approach having technical security resources coupled with nontechnical security capabilities [37]. In particular, considering the technical and procedural nature of security and compliance, the combination of IT security resources and procedural practices is important. For example, IT intrusion detection applications combined with security education programs likely create better outcomes than the adoption of IT applications alone. The combination of security systems and abilities to use them enables the organization to communicate its ultimate goals and strategies and leads to a common understanding of security strategies. In particular, IT security resources combined with embedded security policies and procedures form daily routines for enduring information security throughout business operations. Organizations that successfully invest in such IT security resources and procedural practices are thought to enjoy superior security performance [4, 63, 72].

While IT security resources and procedural practices have their own roles, they are also interdependent and mutually support and reinforce each other [60]. The value of complementary IT security resources and procedural practices is greater than the sum of their individual values [7]. Tanriverdi and Venkatraman [61] argued that the relatedness and the complementarity of IT security resources and procedural practices could be advantageous. They explained that complementarities among the related IT security resources and procedural practices could create additional performance synergies. Likewise, IT security infrastructures, human resources, and third-party security management are complementary. Therefore, the complementarity of IT security resources and procedural practices creates synergistic value (e.g., [53]). The benefits of such an approach include improved compliance and fewer security incidents.

Generally, prevention procedural practices represent daily operational abilities closely combined with IT security resources, while audit practices focus on regular audit policies and procedures. Hence, the investments in both IT security resources and prevention procedures related to the IT security resources enable organizations to gain synergies from the combination [10, 72]. In other words, while IT security resources and prevention practices have their own roles, they are interdependent and mutually reinforce each other. The benefits of such an approach could include improved compliance and fewer information security incidents.

Moreover, as we noted earlier, although organizations implement the same IT security resources and prevention policies, they may have different synergistic effects based on their security operational maturity. When organizations are operationally mature, their security resources are more strategically planned and executed, creating synergistic effects and thus resulting in better information security and compliance. This directly leads us to our final hypothesis:

- **Hypothesis 3 (The Synergistic Effect in Mature Organizations Hypothesis):** Security operational maturity enables synergistic effects of IT security resources and related policies.

---

## Data Description

We drew on data from the Kroll/HIMSS hospital survey on patient data safety [64]. This telephone-based survey of 250 health-care organizations polled respondents on hospital security practices, compliance, and breach occurrence. The respondents included IT executives, chief security officers (CSOs), health information management (HIM) directors, compliance officers, and privacy officers. Of the 250 hospitals, we dropped 7 hospitals whose security resources had been adopted because of their data breaches (to control for reverse causality between breach occurrence and security resources). Our remaining sample of 243 hospitals included information on compliance, breach occurrences, and security resources. Table 1 shows variable definitions.

### Dependent Variables

Our study has two security outcomes: **Breach** and **Compliance**. The level of regulatory compliance was self-reported by the IT managers who play a role in patient data security (e.g., senior IT executives, CSOs, and HIM directors). For Compliance, a scale of one to seven (1 = “not at all prepared” and 7 = “extremely prepared”) was employed to measure the level of compliance on five security regulations: HITECH, HIPAA, state security laws, red flag rules, and Centers for Medicare & Medicaid Services (CMS) regulations. Considering CMS regulations as a baseline, four dummy variables were used to indicate compliance with the other regimes. Breach, as a measure of actual security, was measured by whether an organization experienced any breach in the past 12 months.

### Independent Variables

Our independent variables include various security resources. In the IT area, researchers distinguish between technical components (e.g., IT security applications and measures) and nontechnical components (e.g., employee training, policies, systematic processes, and procedures) [5, 53]. Following this categorization, we define security resources as technical (**ITSecRes**) and nontechnical components (**Prevention** and **Audit** policies).

The number of adopted IT security applications, physical controls, and technical measures represents **ITSecRes** at organization *i*. These resources become the framework for all security activities (e.g., [57, 62]). IT applications provide security functions that monitor the access and use of patient information. Physical controls include security locks, guards, badge access controls, and scanners. Technical IT security measures include firewalls, encrypted e-mails, network monitoring, intrusion detection, and so forth.

```
ITSecRes_i = Σ IT security systems_i = (IT applications_i + Physical security measures_i + Technical IT measures_i).
```

Information security involves both preventing security breaches and auditing possible failure events [68]. Security researchers have argued that organizations improve information security through a combination of preventive and audit activities that reduce internal and external failures [31, 59]. These aspects have parallels in quality management, where researchers have classified improvement initiatives into prevention (e.g., preventive maintenance, training, and process engineering) and appraisal/audit activities (e.g., manufacturing inspection, audits, product testing) [8, 32, 49].

**Prevention** is measured by the number of adopted policies, including security procedures, human resources monitoring for hiring and continuing education tasks, hiring practices (i.e., background checks), data access minimization (i.e., giving employees only the information they need), and ensuring that patients are who they say they are through ID checks:

```
Prevention_i = Σ Prevention policies_i = (Security procedures_i + HR monitoring_i + HR practices_i + Data access minimization_i + Ensuring who they say they are_i).
```

**Audit** is the number of adopted appraisal and auditing policies at organization *i*. This includes regular audits on systems using patient data, specific audit policies in place to monitor patient data access and sharing, IT audit logs to detect inappropriate access to patient data, regular audits on data processes, regularly scheduled meetings for security review, and breach notification procedures:

```
Audit_i = Σ Appraisal/Audit policies_i = (Regular audit on systems_i + Audit policies_i + IT audit logs_i + Regular audit on processes_i + Regular security review meetings_i + Breach notification procedures_i).
```

### Table 1. Variable Definitions

| **Variable** | **Definition** |
|--------------|---------------|
| **Breach** | Whether a hospital experienced any breach in the past 12 months. |
| **Compliance** | The level of regulatory compliance with respect to patient data security regulations (a scale from one to seven). |
| **Security cultural value** | The level of organizational culture for ensuring patient data safety (a scale from one to seven). |
| **OpMaturity** | Whether hospitals regularly review their security action plans or not. This regular review reflects a hospital’s security operational maturity. |
| **Security resources to execute daily operations for ensuring and evaluating patient data safety** | |
| **ITSecRes** | Whether a hospital has the following practices (3): <ul><li>IT applications have audit functions that monitor the access and use of patient information</li><li>Physical security measures (locks, guards, badge access, scanners)</li><li>Technical IT security measures (firewalls, encrypted e-mails, network monitoring, intrusion detection, etc.)</li></ul> |
| **Prevention** | Whether a hospital has the following practices (5): <ul><li>Security policy/procedures</li><li>Human resources monitors completion of courses on confidential patient data for hiring and continuing education tasks</li><li>Hiring practices (background checks)</li><li>Data access minimization (giving employees only the information they need)</li><li>Ensuring that the patients are who they say they are through ID checks when service is initiated</li></ul> |
| **Audit** | Whether a hospital has the following practices (6): <ul><li>Regular audits are conducted of systems that generate, collect, and transmit patient data</li><li>Specific policy in place to monitor electronic patient health information access and sharing</li><li>IT audit logs are created and analyzed for inappropriate access to patient data</li><li>Regular audits are conducted for processes where patient information is shared with other external organizations, agencies, or entities</li><li>Regularly scheduled meetings are conducted to specifically review the status of information security policies, procedures, and current operations</li><li>Process in place for reporting breaches in patient information</li></ul> |
| **Control variables** | |
| **General** | General institutes (1 if experienced, 0 otherwise) |
| **Critical** | Critical access (1 if experienced, 0 otherwise) |
| **Academic** | Academic institutes (1 if experienced, 0 otherwise) |
| **BedSize** | Size (1: <100, 2: 100-299, 3: 300+ beds) |
| **TopMgmt** | The support level of a top executive in charge of information security (a scale from one to seven). |
| **Instrumental variables (1 if yes, 0 otherwise)** | |
| **Device** | Risks at portable device |
| **ThirdParty** | Risks at external parties |
| **Internet** | Risks at Internet access |
| **DataCoord** | The level of data sharing/coordination among the departments that manage clinical, financial, and demographic information |
| **Legal** | Whether a security decision is affected by advice of legal counsel |
| **Reg** | Whether a security decision is affected by changes in external policies and regulations |

By simplifying the five levels of the PMM, security operational maturity (**OpMaturity**) was dichotomously measured by whether a hospital regularly reviewed its own security action plan. A hospital’s security action plan and regular review of that plan enable the organization to utilize its security resources based on its needs and idiosyncratic environment. The existence of a security action plan and regular review process reflects a hospital’s security operational maturity. Through the procedures for developing a security action plan, organizations can become mature by learning their own potential risks and security posture.

### Instrumental Variables

To account for the endogeneity of breach occurrences and compliance, we estimated a system of equations by employing indicators as instruments. For compliance, two instruments, **Legal** and **Reg**, were employed. **Legal** is 1 if advice of legal counsel triggers a hospital’s security actions, otherwise 0. **Reg** is 1 if any change in external regulations triggers a hospital’s security actions, otherwise 0.

Breach occurrences have four instrumental variables, including **Device**, **ThirdParty**, **Internet**, and **DataCoord**, which are closely related to a breach occurrence. **Device** is 1 if a hospital has any risk factors in a portable device (laptop, PDA), otherwise 0. **ThirdParty** is 1 if a hospital thinks that sharing information with external parties (third-party vendor, regional health information organizations, etc.) puts patient information at risk, otherwise 0. **Internet** is 1 if Internet access (physician access from home, patient access of information such as laboratory results) puts patient information at risk, otherwise 0. **DataCoord** represents the level of coordination between departments to maintain a secure environment as the patient data move across the organization. It was measured on a scale from one to seven (1 = “no coordination” and 7 = “high level of coordination”).

### Control Variables

Our model includes control variables that have been commonly used to control for the size and type of health-care organizations: **BedSize** and health-care organization types, including **Critical**, **General**, and **Academic**, with **Others** as the base case. **BedSize** was measured by the number of licensed beds in a health-care facility [4].

Although our data set consists of seemingly homogeneous units, organization-specific factors may give rise to potential confounds [20, 21]. When reviewing differences in the survey responses by hospital type—general medical and surgical, academic medical center, and critical access—critical access facilities generally lagged behind the others in terms of electronic patient health information security policy implementation and ongoing review and audit. Thus, the data were controlled by hospital type.

In our data set, slightly more than half of the organizations (56 percent) were general medical/surgical hospital, with a third being critical access hospitals. Four percent were part of an academic medical center. The remaining 7 percent were hospitals classified as “others,” which includes pediatric or other specialty hospital. U.S. hospitals are categorized into four types: **General**, **Critical**, **Academic**, and **Others**. Our model considers **Others** as a base case. **Critical**, **General**, and **Academic** are all dummy variables that describe organizational type. **General** is 1 if a hospital is a general medical institute. **Critical** is 1 if it is a critical access institute, **Academic** is 1 if it includes an academic program; otherwise 0. Furthermore, we controlled for the level of top-management support using a scale of one to seven (1 = “not at all supported by top-level management” and 7 = “highly supported by top-level management”).

---

## Econometric Model

One of our main research interests is the relationship between actual security and compliance. Our argument is that security and compliance are coupled, but the relationship may vary with the security operational maturity. Economically, this suggests a model where security and compliance are simultaneously determined, and our model should treat these two variables as jointly endogenous (e.g., [3, 26]). Breach occurrence and compliance also should be posited as a function of security resources (i.e., IT security resources, prevention, and audit).

Although it is widely believed that information security and compliance simultaneously influence each other when employed as regressors in the explanation of the other, this simultaneity must be tested to confirm whether the simultaneity is statistically significant. The Hausman test statistic for the residual coefficients was used to test for endogeneity in breach occurrences and compliance. In the test of the endogeneity of compliance, the null hypothesis that the coefficient on the residuals is zero was rejected at the 1 percent level. Thus, compliance is endogenous in an explanation of breach occurrences. A similar estimation routine was conducted to test for the endogeneity of breach occurrences. The null hypothesis of an exogenous breach occurrence for compliance was rejected at *p* < 0.001. As expected, the endogeneity of breach occurrences and compliance were statistically significant. Thus, our model should employ simultaneous equations: two-stage least squares (2SLS) or three-stage least squares (3SLS).

Next, the Breusch-Pagan test was used to examine the independence of the two error terms from breach occurrences and compliance as a function of security resources. The result rejected the null hypothesis (cross-equation correlation) that two error terms were independent at *p* < 0.01. The result from the Breusch-Pagan test suggested that the 3SLS approach—which applies the usual feasible generalized least squares (FGLS) method to take account of the cross-equation correlations between equations—was more appropriate than 2SLS [28, 71].

Thus, using 3SLS, we consider compliance as a function of security resources and breach occurrences, and at the same time we consider breach occurrences as a function of security resources and compliance. The structural form of the model can be simplified as follows:

```
Breach_i = α_{1,1} + δ_1 Compliance_i + α_{1,1} ITSecRes_i + α_{1,2} Prevention_i + α_{1,3} Audit_i
           + α_{1,4} ITSecRes_i * Prevention_i + ζ_{1,1} Device_i + ζ_{1,2} ThirdParty_i + ζ_{1,3} Internet_i
           + ζ_{1,4} DataCoord_i + κ_{1,1} BedSize_i + κ_{1,2} General_i + κ_{1,3} Critical_i + κ_{1,4} Academic_i
           + κ_{1,5} TopMgmt_i + φ_{1,1} HITECH_i + φ_{1,2} HIPPA_i + φ_{1,3} State_i + φ_{1,3} RedFlag_i + ε_{1i}

Compliance_i = α_{2,1} + δ_2 Breach_i + α_{2,1} ITSecRes_i + α_{2,2} Prevention_i + α_{2,3} Audit_i
               + α_{2,4} ITSecRes_i * Prevention_i + ζ_{2,1} Legal_i + ζ_{2,2} Reg_i + κ_{2,1} BedSize_i
               + κ_{2,2} General_i + κ_{2,3} Critical_i + κ_{2,4} Academic_i + κ_{2,5} TopMgmt_i
               + φ_{2,1} HITECH_i + φ_{2,2} HIPPA_i + φ_{2,3} State_i + φ_{2,3} RedFlag_i + ε_{2i}
```

Changes in compliance will lead to changes in Equation (1), and the resulting changes in Equation (1) will directly lead to changes in Equation (2). As a result, these equations can identify the simultaneous effects of breach occurrence and compliance.

The estimators of the system described by Equations (1) and (2) include instrumental variables (ζ), instrumenting for **Breach** in Equation (1) and **Compliance** in Equation (2). Equation (1) has **Device**, **ThirdParty**, **Internet**, and **DataCoord** as the instruments, and Equation (2) has **Legal** and **Reg** as the instruments. The idea behind the instrumental variables approach is that these variables are uncorrelated with stochastic disturbances in the dependent variable to be measured but are correlated with the jointly endogenous variable.

The instrumental variables (ζ_{j,k}, j = 1 and 2) directly affect a dependent variable in a particular equation and indirectly affect the other through a second-order effect (through the rest of the system). For example, Internet access that puts patient information at risk is more directly associated with breach occurrence, and it influences a hospital’s perceived compliance through the change in breach occurrence as a second-order effect. Also, the risks of portable devices and data sharing directly affect breach occurrence but are uncorrelated with unexplained variation in compliance. Similarly, legal counsel or external regulations affect the level of regulatory compliance, and they are uncorrelated with unexplained variation in breach occurrence. Our model uses cross-sectional data to identify the causal relationship between breach occurrences and compliance by using instrumental variables, including weak links and legal factors. Our instruments passed the overidentification tests of all the instruments (Sargan statistic) as a conventional validity test [54]. The *p*-values for the instruments of breach occurrences and compliance were 0.580 and 0.908, respectively. The results cannot reject the null hypothesis that the instruments of breach occurrence and compliance are uncorrelated with the error term, suggesting that we should be satisfied with this specification.

---

## Empirical Results

We first assessed the correlations between the explanatory variables of our models. Table 2 displays the correlation matrix with the condition number (the square root of the maximum eigenvalue divided by the minimum eigenvalue). Most of the correlations among the variables show low values, and the multicollinearity diagnostics produce the condition number, 24.5, which is below the common cutoff threshold of 30 [9].

Next, we ran our simultaneous equations on samples stratified using the variable **OpMaturity** for operationally mature and immature organizations. To ensure that the two samples were not otherwise different, we ran *t*-tests to compare them. Table 3 shows descriptive statistics and the results from our *t*-tests on the focal variables (including breach, compliance, and security resources). We can see that all the *p*-values are larger than 0.1. This indicates that the two samples are indistinguishable in terms of the adoption of security resources and security outcomes.

Tables 4 and 5 show the results from the simultaneous equations for operationally mature and immature hospitals, respectively. While **Model 2** examines the direct and indirect effects of the independent variables, including the main-effect and interaction-effect terms, **Model 1** includes only the main-effect terms. We first investigated how security and compliance influence each other. From our results, we can see that the causality between compliance and information security depends on the operational maturity of the hospitals. In operationally mature hospitals, breach occurrences erode regulatory compliance (-0.642 and -0.636 at *p* < 0.1 in Table 4). But surprisingly, compliance does not affect breach occurrence. This supports the hypothesis that an operationally mature organization is more likely to be motivated by data security than regulatory compliance (**H1a**, The Maturity and Security Hypothesis).

In operationally immature hospitals, compliance significantly reduces breach occurrences (-0.314 and -0.315 at *p* < 0.05 in Table 5), and breach occurrences do not affect compliance. This supports the hypothesis that an operationally immature organization is more likely to be motivated by regulatory compliance than actual security (**H1b**, The Maturity and Compliance Hypothesis). This may imply that immature hospitals do not consider a breach as representing noncompliance, once they have fulfilled ex post remediation activities. But the mature hospitals perceive that breaches indicate other hidden failures in compliance.

Next, we examined how security resources work for compliance and security in order to test **H2a** and **H2b**, The Security Resources in Mature and Immature Organizations Hypotheses. We found that the effects of security resources vary with breach occurrences and compliance. The adoption of IT security resources always decreases breach occurrence regardless of security operational maturity (-0.544 at *p* < 0.01 in Table 4 and -0.498 at *p* < 0.01 in Table 5). However, IT security resources improve compliance only in mature hospitals (0.376 at *p* < 0.05 in Table 4). Furthermore, we see that the adoption of prevention policies in procedural resources consistently and significantly improves security and compliance. Prevention policies decrease breach occurrence (-0.462 at *p* < 0.01 in Table 4 and -0.468 at *p* < 0.01 in Table 5) as well as increase compliance (0.599 at *p* < 0.01 in Table 4 and 1.685 at *p* < 0.01 in Table 5) in all the hospitals.

For all the hospitals, audit policies are significantly associated with breach incidents (0.451 at *p* < 0.01 in Table 4 and 0.239 at *p* < 0.01 in Table 5). This is likely because hospitals with more audit resources find and report more breaches than others that do not even realize they have been breached. However, in terms of compliance, the effects are not consistent. Audit policies significantly improve compliance in operationally mature hospitals (1.108 at *p* < 0.01 in Table 4), but they do not have any effect in operationally immature hospitals. Keep in mind that hospitals adopt audit policies to monitor for illegal activities or evaluate the level of compliance. Thus, audit policies may provide comfort to operationally mature hospitals. As a result, **H2a** and **H2b** (The Security Resources in Mature and Immature Organizations Hypotheses) are partially supported.

Last, using **Model 2**, we investigated whether security resources have synergistic effects, including the interaction term of IT security resources and prevention policies. The results show that operationally mature hospitals enjoy synergies between IT security and prevention resources resulting in fewer breaches (-0.310 at *p* < 0.01 in Table 4). This implies that the interaction of IT security resources and prevention practices increases actual security performance more than either type alone. In other words, the effect of IT security resources becomes greater when implemented in conjunction with proper education, hiring practice, policies, and procedures. Thus, we find support for our argument that security operational maturity leads to synergistic effects between IT security resources and related policies (**H3**, The Synergistic Effect in Mature Organizations Hypothesis). Notice that immature hospitals do not experience these synergies (-0.068, not significant in Table 5). Also notice that there is no synergistic effect for compliance. From this, we can infer that the systematic execution of security resources influences breach occurrence more than compliance. Our results are summarized in Table 6.

### Table 4. Results from Operationally Mature Hospitals

| **Variables** | **Model 1** |  | **Model 2** |  |
|---------------|-------------|-------------|-------------|-------------|
|               | **Main Effects** |  | **Main and Interaction Effects** |  |
|               | **Breach** | **Compliance** | **Breach** | **Compliance** |
| **Compliance** | -0.012 (0.248) |  | 0.127 (0.260) |  |
| **Breach** |  | -0.642* (0.383) |  | -0.636* (0.383) |
| **Security resources** |  |  |  |  |
| **ITSecRes** | -0.544*** (0.057) | 0.376** (0.149) | -0.237*** (0.075) | 0.210 (0.189) |
| **Prevention** | -0.462*** (0.075) | 0.599*** (0.197) | -0.288*** (0.084) | 0.496** (0.211) |
| **Audit** | 0.451*** (0.067) | 1.108*** (0.174) | 0.475*** (0.070) | 1.090*** (0.175) |
| **Synergistic effect** |  |  |  |  |
| **ITSecRes * Prevention** |  |  | -0.310*** (0.047) | 0.170 (0.120) |
| **Instrumental variables** |  |  |  |  |
| **Device** | 0.119*** (0.038) |  | 0.136*** (0.040) |  |
| **ThirdParty** | -0.151*** (0.031) |  | -0.168*** (0.032) |  |
| **Internet** | -0.022 (0.060) |  | -0.044 (0.063) |  |
| **DataCoord** | -0.045 (0.067) |  | -0.063 (0.070) |  |
| **Legal** |  | 0.006 (0.063) |  | 0.001 (0.064) |
| **Reg** |  | 0.070 (0.078) |  | 0.064 (0.079) |
| **Control variables** |  |  |  |  |
| **BedSize** | 0.039 (0.026) | -0.089 (0.066) | 0.047* (0.027) | -0.089 (0.066) |
| **General** | 0.006 (0.050) | 0.017 (0.132) | 0.010 (0.053) | 0.011 (0.132) |
| **Critical** | -0.008 (0.069) | -0.109 (0.131) | 0.020 (0.073) | -0.111 (0.131) |
| **Academic** | -0.008 (0.096) | 0.416** (0.205) | -0.027 (0.100) | 0.404** (0.206) |
| **TopMgmt** | 0.000 (0.021) | 0.083*** (0.029) | -0.029 (0.022) | 0.091*** (0.030) |
| **Regulations** |  |  |  |  |
| **HITECH** | -0.014 (0.218) | -0.873*** (0.094) | 0.107 (0.228) | -0.873*** (0.094) |
| **HIPAA** | -0.005 (0.036) | -0.003 (0.094) | -0.006 (0.037) | -0.003 (0.094) |
| **State Security Laws** | -0.004 (0.055) | -0.171* (0.094) | 0.020 (0.057) | -0.172* (0.095) |
| **Red Flag Rules** | -0.015 (0.117) | -0.467*** (0.096) | 0.045 (0.122) | -0.465*** (0.096) |
| **Weighted R²** | 0.238 |  | 0.250 |  |

**Notes:** The number of total observations is 924. Standard errors are in parentheses. * Significant at *p* < 0.1; ** significant at *p* < 0.05; *** significant at *p* < 0.01.

### Table 5. Results from Operationally Immature Hospitals

| **Variables** | **Model 1** |  | **Model 2** |  |
|---------------|-------------|-------------|-------------|-------------|
|               | **Main Effects** |  | **Main and Interaction Effects** |  |
|               | **Breach** | **Compliance** | **Breach** | **Compliance** |
| **Compliance** | -0.314** (0.155) |  | -0.315** (0.154) |  |
| **Breach** |  | -1.111 (1.095) |  | -1.256 (1.111) |
| **Security resources** |  |  |  |  |
| **ITSecRes** | -0.498*** (0.113) | 0.026 (0.347) | -0.426*** (0.130) | -0.221 (0.397) |
| **Prevention** | -0.468*** (0.149) | 1.685*** (0.429) | -0.452*** (0.157) | 1.423*** (0.477) |
| **Audit** | 0.239*** (0.098) | 0.292 (0.276) | 0.264*** (0.099) | 0.228 (0.283) |
| **Synergistic effect** |  |  |  |  |
| **ITSecRes * Prevention** |  |  | -0.068 (0.068) | 0.289 (0.204) |
| **Instrumental variables** |  |  |  |  |
| **Device** | 0.005 (0.108) |  | 0.036 (0.107) |  |
| **ThirdParty** | -0.140 (0.166) |  | -0.149 (0.165) |  |
| **Internet** | -0.327* (0.185) |  | -0.460* (0.189) |  |
| **DataCoord** | 0.062 (0.058) |  | 0.078 (0.058) |  |
| **Legal** |  | -0.161 (0.231) |  | -0.212 (0.235) |
| **Reg** |  | 0.024 (0.138) |  | 0.093 (0.140) |
| **Control variables** |  |  |  |  |
| **BedSize** | -0.056 (0.048) | 0.053 (0.204) | -0.071 (0.050) | 0.084 (0.209) |
| **General** | -0.089 (0.149) | -0.503 (0.415) | -0.073 (0.148) | -0.463 (0.421) |
| **Critical** | -0.273** (0.138) | -0.549* (0.299) | -0.278* (0.137) | -0.483 (0.306) |
| **Academic** | -0.050 (0.211) | -0.429 (0.665) | -0.027 (0.211) | -0.439 (0.673) |
| **TopMgmt** | 0.112*** (0.034) | 0.302*** (0.115) | 0.095*** (0.035) | 0.334*** (0.119) |
| **Regulations** |  |  |  |  |
| **HITECH** | -0.291* (0.154) | -0.893*** (0.204) | -0.294* (0.152) | -0.896*** (0.206) |
| **HIPAA** | -0.008 (0.065) | -0.041 (0.197) | -0.009 (0.064) | -0.038 (0.200) |
| **State Security Laws** | -0.084 (0.080) | -0.288 (0.199) | -0.086 (0.079) | -0.283 (0.202) |
| **Red Flag Rules** | -0.191* (0.111) | -0.603*** (0.198) | -0.193* (0.110) | -0.599*** (0.201) |
| **Weighted R²** | 0.295 |  | 0.303 |  |

**Notes:** The number of total observations is 262. Standard errors are in parentheses. * Significant at *p* < 0.1; ** significant at *p* < 0.05; *** significant at *p* < 0.01.

### Table 6. Hypotheses Supports

| **Hypotheses** | **Results** |  |
|----------------|-------------|-------------|
|                | **Breach Occurrences** | **Compliance** |
| **H1a** The maturity and security hypothesis |  | Supported |
| **H1b** The maturity and compliance hypothesis |  | Supported |
| **H2a** The security resources in mature organizations hypothesis |  |  |
| **ITSecRes** | Supported (–)* | Supported (+)** |
| **Prevention** | Supported (–)* | Supported (+)** |
| **Audit** | Supported (+)** | Supported (+)** |
| **H2b** The security resources in immature organizations hypothesis |  |  |
| **ITSecRes** | Supported (–)* | Not supported |
| **Prevention** | Supported (–)* | Supported (+)** |
| **Audit** | Supported (+)** | Not supported |
| **H3** The synergistic effect in mature organizations hypothesis | Supported (–)** | Not supported |

---

## Conclusion

This study examined how security resources influence actual security and compliance and how they influence each other. We utilized qualitative and quantitative survey data provided by senior IT managers from 243 hospitals. The data provide a snapshot of patient information security in the surveyed health-care organizations. Considering the causality between data security and compliance, we formulated our models using simultaneous equations. Our findings indicate that data security and compliance do not always have the same effect. Rather, their causality depends on a hospital’s security operational maturity. Furthermore, the effects of security resources on breach occurrences are different than on compliance, and the effects vary with security operational maturity, which drives synergistic effects between security resources.

Our analysis of causality demonstrates that regulatory compliance significantly decreases breach occurrences only for operationally immature hospitals, and breach occurrences hurt perceived compliance only for operationally mature hospitals. This may be because immature hospitals do not consider breach occurrences as noncompliance once they fulfill ex post remediation activities. The result further indicates that immature hospitals are motivated by meeting compliance mandates rather than actually protecting information. In operationally immature hospitals, compliance may depend more on checklists of adopted security resources. Although this effort for compliance at least helps actual security, this checklist mentality may prevent organizations from developing the more comprehensive and sustainable capabilities needed for meaningful improvements in the day-to-day handling of patient data. By contrast, operationally mature hospitals seem to be more motivated by actually protecting their patient data rather than fulfilling minimal regulatory requirements.

We further found that security resources have a different effect on security and compliance depending on a hospital’s security operational maturity. In terms of compliance, with security operational maturity, all the security resources have significant effects. Without security operational maturity, the effects of security resources are diminished. Only prevention resources have significant effects on compliance. In terms of breach occurrence, the effects of all the security resources are statistically significant for all the hospitals, and these resources have synergistic effects in mature hospitals but have no synergistic effects in immature hospitals. This indicates that mature hospitals that balance investment between IT security and prevention resources can experience synergies that lead to higher levels of data security.

In addition, we found that audit resources have conflicting effects on breach occurrence and compliance. Since audit resources enhance compliance by finding and making notifications about illegal activities and breaches, breach occurrences and compliance are affected in the opposite way, especially in immature organizations. This finding provides insights into security regulations. Security regulations should provide incentives for immature organizations to adopt auditing measures and properly disclose data breaches: the value of carrot (e.g., breach disclosure) versus stick policies (e.g., nondisclosure). Also, policymakers should focus on providing guidelines to invest in developing security resources coupled with security operational maturity rather than simply imposing single-solution compliance requirements regardless of organizational heterogeneity. They need to encourage organizations to actively develop and maintain their own action plans rather than providing checkbox requirement lists.

Furthermore, these various effects of security resources on security outcomes demonstrate that the theoretical perspective of the resource-based view oversimplifies security problems. This suggests that a better system of security resources can be designed based on security operational maturity and that security regulations need to be flexible based on the heterogeneity of organizational security resources and operational maturity. Considering breach occurrences of compliance with causality, our results further reveal which initiator (breach occurrences or compliance) can better utilize security resources and achieve better security performance. This is important because hospitals need to understand how effective and efficient they are (or are not) in order to reduce wasteful investments in security resources.

Although this study provides a new perspective on the variation of security resources and performance, there are some limitations. First, our measures were based on ordinal self-reported data from security managers in hospitals. These measures might be vulnerable to the respondents’ subjective assessments of their organizations and to single-respondent bias. Second, actual security was measured by whether a hospital had experienced any breach in the past 12 months. The financial loss or breach remediation cost could provide additional insight on the effects of various security resources.

---

## Acknowledgments

This research was partially supported by the National Science Foundation, Grant Award no. CNS-0910842, under the auspices of the Institute for Security, Technology, and Society (ISTS). The authors are grateful for the many helpful comments from the participants of the 25th Anniversary Symposium for the Competitive Strategy, Economics and Information Systems. They also thank Rob Kauffman and five anonymous referees for their constructive input to the development of this paper. An earlier version of this paper appeared in the *Proceedings of the 46th Annual Hawaii International Conference on System Sciences*.

---

## Notes

1. As required by section 13402(e)(4) of the HITECH Act, the secretary must post a list of breaches of unsecured protected health information affecting 500 or more individuals.
2. Since 2003, 46 states, the District of Columbia, Guam, Puerto Rico, and the Virgin Islands have enacted legislation requiring notification of security breaches involving personal information.
3. Regulatory compliance in health care should be thought of as “perceived” compliance because there are no certifying bodies, so it is not possible to externally assess “objective” compliance. Hospital managers can obtain outside opinions and run internal assessments, but they cannot obtain a certification of regulatory compliance. Thus, compliance is really a manager’s assessment of an organization’s adherence to the regulation.
4. **Ad hoc**—procedures or processes are generally informal, incomplete, and inconsistently applied. **Repeatable**—procedures or processes exist; however, they are not fully documented and do not cover all relevant aspects. **Defined**—procedures and processes are fully documented and implemented and cover all relevant aspects. **Managed**—reviews are conducted to assess the effectiveness of the controls in place. **Optimized**—regular review and feedback are used to ensure continuous improvement toward optimization of the given process.
5. Kroll is a leader in health-care information security and has helped some of the largest health-care providers in the country respond to information security breaches. The survey was conducted in partnership with the Healthcare Information and Management Systems Society (HIMSS) Analytics, the leading organization representing the health information management systems and services industry.
6. We implemented our 3SLS model using “Proc model” in SAS and conducted the Hausman test. For the other tests, the Breusch-Pagan test and Sargan statistic, we employed Stata.

---

## References

1. AICPA/CICA privacy maturity model. American Institute of Certified Public Accountants, Inc., New York, March 2011 (available at www.aicpa.org/interestareas/informationtechnology/resources/privacy/downloadabledocuments/10-229_aicpa_cica%20privacy%20maturity%20model_finalebook_revised0612.pdf).
2. Alavi, M.; Kayworth, T.R.; and Leidner, D.E. An empirical examination of the influence of organizational culture on knowledge management practices. *Journal of Management Information Systems*, 22, 3 (Winter 2005-6), 191–224.
3. Anderson, M.C.; Banker, R.D.; and Ravindran, S. Value implications of investments in information technology. *Management Science*, 52, 9 (2006), 1359–1376.
4. Anol, B.; Hikmet, N.; Menachemi, N.; Kayhan, V.O.; and Brooks, R.G. The differential performance effects of healthcare information technology adoption. *Information Systems Management*, 24, 1 (Winter 2007), 5–14.
5. Aral, S., and Weill, P. IT assets, organizational capabilities, and firm performance: How resource allocations and organizational differences explain performance variation. *Organization Science*, 18, 5 (2007), 763–780.
6. Balbastre, F., and Moreno-Luzon, M. Self-assessment application and learning in organizations: A special reference to the ontological dimension. *Total Quality Management & Business Excellence*, 14, 3 (2003), 367–388.
7. Barua, A., and Whinston, A.B. Decision support for managing organizational design dynamics. *Decision Support Systems*, 22, 1 (1998), 45–58.
8. Behara, R.; Derric, C.; and Hu, Q. A process approach to information security: Lessons from quality management. In *Proceedings of the 2006 Americas Conference on Information Systems*. Acapulco: Association for Information Systems, 2006, pp. 169–178 (available at http://aisel.aisnet.org/amcis2006/169/).
9. Belsley, D.A.; Kuh, E.; and Welsch, R.E. *Regression Diagnostics: Identifying Influential Data and Sources of Collinearity*. New York: John Wiley & Sons, 2004.
10. Bharadwaj, S.; Bharadwaj, A.; and Bendoly, E. The performance effects of complementarities between information systems, marketing, manufacturing, and supply chain processes. *Information Systems Research*, 18, 4 (2007), 437–453.
11. Brown, C.V., and Vessey, I. Managing the next wave of enterprise systems: Leveraging lessons from ERP. *MIS Quarterly Executive*, 2, 1 (2003), 45–57.
12. Bulgurcu, B.; Cavusoglu, H.; and Benbasat, I. Information security policy compliance: An empirical study of rational-based beliefs and information security awareness. *MIS Quarterly*, 34, 3 (2010), 523–548.
13. Carmeli, A., and Tishler, A. The relationships between intangible organizational elements and organizational performance. *Strategic Management Journal*, 25, 13 (2004), 1257–1278.
14. Casaretto, J. Security compliance does not equal security. *Wikibon Blog*, July 2011 (available at http://wikibon.org/blog/security-compliance-does-not-equal-security/).
15. Cavusoglu, H.; Raghunathan, S.; and Yue, W.T. Decision-theoretic and game-theoretic approaches to IT security investment. *Journal of Management Information Systems*, 25, 2 (Fall 2008), 281–304.
16. Chang, K.C., and Wang, C.P. Information systems resources and information security. *Information Systems Frontiers*, 13, 4 (2011), 579–593.
17. Cremonini, M., and Nizovtsev, D. Risks and benefits of signaling information system characteristics to strategic attackers. *Journal of Management Information Systems*, 26, 3 (Winter 2009–10), 241–274.
18. D’Arcy, J., and Herath, T. A review and analysis of deterrence theory in the IS security literature: Making sense of the disparate findings. *European Journal of Information Systems*, 20, 6 (2011), 643–658.
19. D’Arcy, J.; Hovav, A.; and Galletta, D. User awareness of security practices and its impact on information systems misuse: A deterrence approach practice. *Information Systems Research*, 163–175 (2010).
20. Devaraj, S., and Kohli, R. *Information technology payoff in the health-care industry: A longitudinal study*. Information Systems Journal, 16(4), 41–58 (Spring),2000.
21. Devaraj, S.; and Kohli, R. Performance impacts of information technology: Is actual usage the missing link? *Management Science*, 49, 3 (2003), 273–283.
22. Dierickx, I., and Cool, K. Asset stock accumulation and sustainability of competitive advantage. *Management Science*, 35, 12 (1989), 1504–1511.
23. Donovan, F. Protection strategies: A.k.a. alphabet soup. *Infosecurity*, 8, 6 (2011), 22–25.
24. Fehle, F., and Tsyplakov, S. *Dynamic risk management: Theory and evidence*. Management Journal of Financial Economics, 78(1), 3–58 (2005).
25. Fichman, R.; Kohli, R.; and Krishnan, R. *The role of information systems in healthcare: Current trends and future trends*. Information Systems Research, 22(3), 419–428 (2011).
26. Goh, K.H., and Kauffman, R.J. Strategic necessity and advantage? The case of Internet banking in the U.S. banking sector. *Paper presented at the 25th Anniversary Symposium of the Competitive Strategy, Economics and Information Systems Mini-Track*, 2013 Hawaii International Conference on System Sciences, Maui, HI, January 7–8, 2013.
27. Grant, R.M. Toward a knowledge-based theory of the firm. *MIS Quarterly, Strategic Management Journal*, 17(4), 109–122 (Winter),1996.
28. Greene, W.H. *Econometric Analysis*. Englewood Cliffs, NJ: Prentice Hall, 2003.
29. Harter, D.E.; Slaughter, S.A.; and H. D.E. *Quality assurance and infrastructure activity costs in software development: A longitudinal analysis*. Management Science, 49(6), 784–800 (2003).
30. Herath, H.S.B.; Herath, T.C.; and B. H.S. *Investments in information systems security: A real options perspective with Bayesian postaudit*. Journal of Management Information Systems, 25(3), 337–375 (Winter),2008–9.
31. Hong, K.; Chi, Y.; Chag, L.R.; and Tang, J. An integrated systems theory of information systems security management. *Information Management & Security*, 11(5), 243–248 (2003).
32. Ittner, C.; Larcker, D.F.; and C.D. *The performance characteristics of process management techniques*. Management Science, 43(4), 347–522 (1997).
33. Johnson, M.E.; Goetz, E.; and Pfleeger, S.L. *Information security through information risk management*. MIS Quarterly, IEEE Security & Privacy, 7(3), 45–52 (2009).
35. Johnston, A.C.; Hale, R.; and A.C. *Improved information security through information governance*. MIS Quarterly, Communications of the ACM, 52(1), 126–129 (2009).
36. Johnston, A.C.; Warkentin, M.; and A.C. *Information security behaviors and fear appeals: An empirical study*. MIS Quarterly, 34(2), 549–566 (2010).
37. Kayworthy, T.; Whitten, D.; and R. *Effective information policies requires a balance of social and technological factors*. MIS Quarterly, 8(3), 163–175 (2012).
38. Kumar, R.L.; Park, S.; Subramaniam, C.; and L. R.L. *Information systems security: Understanding the value of countermeasure strategies*. Journal of Management Information Systems, 25(2), 233–279 (2008).
39. Laffey, D. *Understanding organizational and transforming organizational information security culture*. Information Management Systems & Computer Security, 18(4), 4–13 (2010).
40. Largest U.S. compilation of *private-sector health comments on nationwide interoperable health information exchange to date*. Press Release. U.S. Department of Health & Human Services, Washington, DC, June 3, 2005 (available at http://archive.hhs.gov/news/press/2005pres/20050603.html).
41. Luftman, J. *Managing business-IT alignment maturity*. Communications of the Association for Information Systems, 4(1), 1–51 (2000).
42. Mahoney, J.T.; Pandian, J.R.; and T. J. *Resource-based view within the conversation of strategic management*. Strategic Management Journal, 13(5), 363–380 (1992).
43. Marcus, A.A.; Nichols, M.L.; and A. *On the edge: Risking the warnings of unusual events*. Organization Science, 10(4), 482–499 (1999).
44. Maurer, C.; Bansal, P.; Crossan, M.; and P. *Creating sustainable economic value through social values: Culturally informed resource-based view*. Organization Science, 22(2), 432–448 (2011).
45. Oliver, C.; and R. *Sustainable competitive advantage: Integrating institutional and resource-based views*. Strategic Management Journal, 18(9), 697–713 (1997).
46. Pironti, J.P.; and P. *Changing organizational mind-set: Creating a risk-conscious security-aware culture*. ISACA Journal, 2(1), 1–7 (2012).
47. Ply, UK; Moore, J.E.; Williams, C.K.; Thatcher, J.B.; and K. *IS management attitudes and employee perceptions at varying organizational levels of software process maturity*. MIS Quarterly, 36(2), 601–624 (2012).
48. Png, I.; Wang, Q.H.; and L. *Information systems security: Facilitating compliance precautions vis-à-vis enforcement against attackers*. Journal of Management Information Systems, 26(2), 97–121 (2009).
49. Powell, T.C.; and C. *Total quality management as competitive advantage: A review and empirical study*. Strategic Management Journal, 16(1), 15–37 (1995).
50. Puhakainen, P.; Siponen, M.; and M. *Improving organizational employees’ compliance through information systems training: An action research study*. MIS Quarterly, 34(4), 757–778 (2010).
51. Rai, A.; Maruping, L.M.; Venkatesh, V.; and A. *Information systems project success: The offshore role of social embeddedness and cultural characteristics*. MIS Quarterly, 33(3), 617–641 (2010).
52. Rhee, H.; Ryu, S.; Kim, C.Y.; and Y. *Unrealistic optimism about information systems management*. Computers & Security, 31(2), 221–232 (2012).
53. Ross, J.W.; Beath, C.M.; Goodhue, D.L.; and W. *Develop long-term organizational competitiveness through IT assets*. Sloan Management Review, 38(1), 31–42 (1996).
54. Sargan, J.D.; and J. *Estimation of organizational resources using econometric instrumental variables*. Econometrica, 26(3), 393–415 (1958).
55. Smith, S.; Welch, D.; Winchester, D.; Bunker, D.; Jamieson, R.; and R. *Circuits of organizational power: A study of mandated information systems compliance to an information security de jure standard in a government organization*. MIS Quarterly, 34(3), 463–486 (2010).
56. Spears, J.; Barki, J.L.; H.; and L. *User information participation in organizational systems security risk management*. MIS Quarterly, 34(3), 503–522 (2010).
57. Srivastava, R.; K.; Shervani, A.; T.A.; Fahey, L.; and R. *Market-based organizational systems and shareholder value: A framework for analysis*. Journal of Marketing, 62(1), 2–18 (1998).
58. State security legislation breach notification laws. *National Conference of State Legislatures*, Denver, CO, 2012 (available at www.ncsl.org/issues-research/telecommunications-information-technology/security-breach-legislation-notices.aspx).
59. Straub, D.W.; Goodman, S.; Baskerville, R.; and W. *Information Security: Policies, Processes, and Practices*. OrganizationArmonk: M.E. Sharpe, 2008.
60. Tanriverdi, H.; and H. *Organizational performance characteristics of information technology synergy in multi-business organizations*. MIS Quarterly, 30(1), 57–58 (2006).
61. Tanriverdi, H.; Venkatraman, N.; and H. *Management knowledge base and the organizational performance of multi-business organizations*. Strategic Management Journal, 26(2), 97–117 (2005).
62. Teece, D.J.; Pisano, G.; Shuen, A.; and A. *Organizational capabilities and dynamic management*. Strategic Management Journal, 18(7), 509–533 (1997).
63. Tiwana, A.; Konsynski, B.; and A. *Organizational complementarities between IT architecture and governance structure*. Information Systems Research, 21(2), 288–304 (2010).
64. 2010 Healthcare Information and Management Systems Society analytics report: Security of organizational patient data. *HIMSS Analytics*, Chicago, April 2010 (available at www.krollcybersecurity.com/media/2010_Kroll-HIMSS_Study_FINAL.pdf).
65. 2012 Healthcare Information and Management Systems Society analytics report: Security of organizational patient data. *HIMSS Analytics*, Chicago, April 2012 (available at www.krollcybersecurity.com/media/Kroll-HIMSS_2012_-_Security_of_Patient_Data_040912.pdf).
66. Urbaczewski, A.; Jessup, L.M.; and A. *Does management electronic monitoring of organizational employee Internet usage work?* Communications of the ACM, 45(1), 80–83 (2002).
67. von Solms, S.H.; and B. *Information systems security governance: Operational compliance management vs. compliance*. Computers & Security, 24(6), 443–447 (2005).
68. Weber, R.; and R. *Information Systems Audit and Control*. Englewood Cliffs, NJ: Prentice Hall, 1999.
69. Wernerfelt, B.; and A. *Resource-based organizational view of the firm*. Strategic Management Journal, 5(2), 171–180 (1984).
70. Whitman, M.E.; Mattord, H.J.; and E. *Principles of Organizational Information Security*. Boston: Course Technology, 2011.
71. Wooldridge, J.M.; and M. *Econometric Analysis of Organizational Cross Section and Panel Data*. OrganizationCambridge: MIT Press, MA, 2002.
72. Zhu, K.; and *Information technology infrastructure and e-commerce capabilities complementarity*: A. Organizational Dynamics resource-based assessment of business value. Journal of Management Information Systems, 21(1), 167–202 (Summer),1984.