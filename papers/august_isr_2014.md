# Cloud Implications on Software Network Structure and Security Risks

**Terrence August**
Rady School of Management, University of California, San Diego, La Jolla, California 92093; and
Korea University Business School, Seoul 136-701, Korea, taugust@ucsd.edu

**Marius Florin Niculescu**
Scheller College of Business, Georgia Institute of Technology, Atlanta, Georgia 30308,
marius.niculescu@scheller.gatech.edu

**Hyoduk Shin**
Rady School of Management, University of California, San Diego, La Jolla, California 92093,
hdshin@ucsd.edu

## Abstract

By software vendors offering, via the cloud, software-as-a-service (SaaS) versions of traditionally on-premises application in the greatly increase the value associated with the software. In an environment where negative security externalities are present and users make complex consumption and patching decisions, we construct a model that clarifies whether and how SaaS versions should be offered by vendors. We find that the existence of version-specific security externalities is sufficient to warrant a versioned outcome, which has been shown to be suboptimal in the absence of security risks. In high security-loss environments, we find that SaaS should be geared to the middle tier of the consumer market if patching costs and the quality of the SaaS offering are high, and geared to the lower tier otherwise. In the former case, when security risk associated with each version is endogenously determined by consumption choices, strategic interactions between the vendor and consumers may cause a higher tier consumer segment to prefer a lower inherent quality product. Relative to on-premises benchmarks, we find that software diversification leads to lower average security losses for users when patching costs are high. However, when patching costs are low, surprisingly, average security losses can increase as a result of SaaS offerings and lead to lower consumer surplus. We also investigate the vendor's security investment decision and establish that, as the market becomes riskier, the vendor tends to increase investments in an on-premises version and decrease investments in a SaaS version. On the other hand, in low security-loss environments, we find that SaaS is optimally targeted to a lower tier of the consumer market, average security losses decrease, and consumer surplus increases as a result. Security investments increase for both software versions as risk increases in these environments.

**Keywords:** cloud computing; software-as-a-service; network economics; security; versioning; on-premises software
**History:** Rahul Telang, Senior Editor; Karthik Kannan, Associate Editor. This paper was received on August 22, 2012, and was with the author(s) 8 months for 2 revision(s). Published online in Articles in Advance July 21, 2014.

## 1. Introduction

With broadband access becoming faster and more pervasive, there has been a shift back toward models where computing is centralized and accessed via thin clients. Both firms and governments are starting to implement cloud-based systems to support business processes and increase operational efficiency. For example, the U.S. government, which has an $80 billion federal IT budget, has championed a Federal Cloud Computing Initiative to encourage agencies to move toward cloud computing solutions, supporting this transition with Apps.gov (Claburn 2009).¹ Gartner estimates that the cloud computing industry will grow to $149 billion by 2015 (Kundra 2011). Vivek Kundra, former U.S. Chief Information Officer, also suggested that cloud computing will help increase productivity in healthcare, financial services, and education, pointing out that a 1% productivity increase in healthcare over the next 10 years represents $300 billion in value (e.g., shifting electronic medical records to the cloud).

Cloud computing is not likely to be an end all solution. Rather, for many firms, it will become an on-demand network access to a shared pool of configurable computing resources (e.g., networks, servers, storage, applications, and services) that can be rapidly provisioned and released with minimal management effort or service provider interaction" (Mell and Grance 2011, p. 2).

increasingly important component of an overall IT strategy, augmenting the traditional models currently used (O'Neill 2011). Among the many opportunities for engagement, cloud computing can be leveraged across diverse service models: infrastructure as a service (IaaS), platform as a service (PaaS), and software as a service (SaaS). Of particular interest to application software companies and the consumers of their products is the SaaS model.² This model has emerged from economic efficiency and to satisfy users' additional preferences that their data and applications be ubiquitous. Over the last two decades, consumers have harnessed SaaS applications for personal email, online gaming, photo sharing, and social networking. Businesses are also using SaaS versions of productivity software, enterprise resource planning software, and more; according to a recent survey by InformationWeek, three quarters of the "companies using SaaS consider application services extremely or critically important to their organizations” (Biddick 2010). For example, to address these market needs, Microsoft has added Microsoft Office 365, a SaaS variant of its well known Microsoft Office suite, which offers enterprise browser-based Office Web Apps to its product portfolio (El Akkad 2011). Similarly, SAP offers SAP Business ByDesign, targeting this version to small businesses (Farber 2007).

When software vendors such as Microsoft and SAP offer SaaS versions of traditionally locally hosted software (often called on-premises because such software is installed on premises at the customer's location), there are significant security risk implications. This versioning strategy greatly affects users' incentives, which in turn determines how aggregate use is spread across the versions and to what extent users engage in secure behaviors such as patching. To better understand the impact of versioning on security risk, it is useful to first discuss the nature of attacks faced by application software products. Security attacks can be broadly categorized into two classes: directed (targeted) and undirected (nontargeted).³ A directed attack occurs when a malicious actor expends effort in an attempt to compromise a specific target (Villeneuve 2011). An undirected attack typically involves self-propagating malware (e.g., a computer worm) designed to spread to and infect many vulnerable hosts, which are often running a common software application that contains an exploitable vulnerability.

Users and organizations are generally exposed to a wide range of directed and undirected attacks due to flaws in hardware and software technologies, poor configurations, and weaknesses in individual decision making. However, to isolate the differential impact on security risk associated with a software vendor offering distinct on-premises and SaaS versions of a software product, it is preferable to focus only on the attacks that specifically exploit vulnerabilities in the code of one of these two versions (essentially holding constant all other attacks unrelated to vulnerabilities in the variants of this product). With this lens, a directed attack refers to an attack explicitly directed toward a particular system running one of these versions and exploiting a vulnerability specific to the version. Similarly, an undirected attack indiscriminately exploits one of these versions on any system running a copy of the version's software.

Focusing on a single software product and the idiosyncratic security risk stemming from each of its versions, the on-premises version has relatively higher undirected risk and the SaaS version has relatively higher directed risk. To see why, suppose SAP Business One (on-premises) contains vulnerability V1, SAP Business ByDesign (SaaS) contains vulnerability V2, and a firm is considering the risks associated with each version. If the firm, along with many other companies with similar needs, chooses to use SAP Business ByDesign, the firm is exposed to considerable directed risk. In particular, a directed attack on SAP's systems (running Business ByDesign) that exploits vulnerability V2 enables a malicious attacker to affect many organizations all at once. On the other hand, if the firm uses SAP Business One, its exposure to directed risk is much lower; the attacker's incentive to exploit vulnerability V1 on the firm's system (running Business One) is reduced because it would only affect an individual organization. Instead, because on-premises versions such as Business One are often widely deployed on independent but interconnected systems, each containing vulnerability V1, a malicious hacker could inflict significantly more damage by using the same vulnerability to attack the entire network in one broad, undirected move, affecting many users.

Because of the large number of installations associated with on-premises software, a software vendor usually manages vulnerabilities by creating and distributing software patches to users. However, it has been historically difficult to incentivize users to patch their own installations when security patches are released. Thus, for on-premises offerings, the user network is characterized by a large number of widespread nodes where individual instances of the software are running with many remaining unpatched (Lemos 2004, Keizer 2008). Even six years after the Conficker worm first struck, the malicious program is still infecting computers (Robertson 2014). Poor user patching behavior increases the risk of other users and, as a result, reduces the value of the software vendor's product. Code Red, SQL Slammer, Sasser, and Conficker are all examples of malware that spread across vulnerable software networks and caused sizable economic damage (Moore et al. 2002, Lemos 2003, Keizer 2004, Markoff 2009).⁴ Microsoft's webserver software, Internet Information Services (IIS), and its database management system, SQL Server, are examples of software products being compromised by these undirected attacks.

Because systems servicing large populations of consumers are attractive targets to hackers incentivized by economic and/or political motivations, SaaS versions have considerable exposure to directed risk as discussed above. Recently Adallom, a SaaS security company, observed an exploited vulnerability in Office 365's token management that enables an attacker to steal a user's token and thus the user's access to the software (Messmer 2013, Liran 2013). Similarly, Office 365 also had a cross-site scripting vulnerability that would enable an attacker to gain administrator access to an organization's Office 365 account and configuration (Lee 2014). In both cases, users can incur substantial economic losses from directed attacks on Microsoft's systems to exploit vulnerabilities in the implementation of Office 365.

When a SaaS variant of an on-premises product is introduced into the market, the aggregate security risk can be affected in several ways. First, as discussed above, users of the SaaS version are exposed to significantly less product-specific undirected risk. Second, an increase in SaaS use helps reduce total risk by diversifying exposure across undirected and directed attacks and limiting the size of populations that malware can effectively target; this, in turn, may indirectly reduce the incentives of malware developers to target diversified software (Bain et al. 2002 and Kannan et al. 2013). Third, a software vendor who expands its product line to offer distinct SaaS and on-premises versions may further expand use through pricing, which indirectly affects security risk. Finally, such a product line expansion to include SaaS may act as a substitute to investments in making on-premises software products more secure.

In recent years, software companies have invested substantial resources in (i) developing SaaS versions of their existing, on-premises software products, and (ii) increasing the security of their on-premises products (Charney 2012). Because of inherent risk interdependencies, it is important for companies such as Microsoft to better understand how versioning and security are intimately related. For example, when Microsoft brought its SaaS service Office 365 to the market, it faced a challenging question of how to manage both Office 365 and its on-premises counterpart, Office, so as to cater to consumers' heterogeneous preferences and harvest the risk diversification benefits that stem from having two versions with separate user populations. One question is which consumer segments should be the targeted users of the SaaS and on-premises versions. Given the strong market for Office 365, Microsoft may also have reconsidered whether its substantial investments in security are still necessary when its product line expands to achieve security through diversity.

Similar challenges are being faced by providers of enterprise application server software (e.g., Oracle WebLogic Server, IBM WebSphere, etc.), database management systems (e.g., Oracle Database, SQL Server, MySQL, etc.), and customer relationship management software (e.g., Microsoft Dynamics, SAP 360, Oracle CRM, etc.).⁵ Because of differences in fixed development costs, business strategy, and individual expertise, not every on-premises software provider will find it economical to offer SaaS alternatives in addition to their traditional on-premises offerings. However, for the software vendors who are either already or in the process of providing both on-premises and SaaS solutions, better product design, consumer segment targeting, and pricing decisions can be made with an improved understanding of the security implications of this type of versioning.

In this paper, we study the security impact of an application software vendor's versioning strategy to include a SaaS variant of its on-premises product. Several research goals drive our study. First, when both SaaS and on-premises offerings are available, we want to better understand how consumers separate across product variants to diversify security risk. Thus, we account for how directed and undirected attacks generate distinct security externalities under each paradigm. We then build a model that captures consumer incentives to use either variant recognizing that (i) users of the on-premises alternative who choose not to patch impose undirected risk on other users, and (ii) directed risk associated with the SaaS alternative is proportional to the size of the total consumer population who opt for the SaaS variant. With this model of consumer behavior, we fully characterize the equilibrium consumer market structure in which the idiosyncratic security externalities are endogenously determined by consumption choices.

Using this equilibrium characterization, a second research goal is to develop an understanding of how a software vendor approaches the versioning problem when the vendor has the potential to offer both SaaS and on-premises versions. The first question is whether a vendor should version its software or simply offer a single on-premises product. Second, we comment on which consumer market segments should be the intended users of each version if the vendor finds it optimal to pursue a versioning strategy. Because of the distinct security externalities, we study whether the vendor's strategic behavior can yield unexpected strategies in the product differentiation and pricing problem.

A final research goal is to quantify the risk diversification benefits of a versioning strategy in this context. Using our framework, we compare measures of profitability, security losses, consumer surplus, and social welfare against benchmark measures stemming from a model of a single, on-premises product that faces only undirected security risk. Using these comparisons, we can clarify the risk environments under which versioning has greater potential. We can also show how a software vendor's security investment decision interacts with the versioning strategy being used.

We then summarize the main findings of our study. One important implication highlighted by our model is that a software vendor may set prices to target an inherently lower quality SaaS product to consumers with higher valuations (i.e., types) than those who use a higher quality on-premises version. In a standard vertical product differentiation setting, the lower quality product typically serves consumers with low types. We demonstrate that strategic interactions between the software vendor and consumers can drive the opposite result where the vendor prices the SaaS product high so as to create a small SaaS user population, thus limiting the directed security risk associated with this product. By offering a lower inherent quality product but with better, endogenously-determined security properties at a higher price, the vendor makes its consumption incentive compatible for the higher type consumers who neither (i) find it cost effective to consume the higher inherent quality on-premises product in a patched state nor (ii) want to be exposed to the significant undirected risk associated with the on-premises product in an unpatched state.

By studying how the software vendor sets SaaS and on-premises product prices and the consumer market structures induced as a result, our findings contribute to a better understanding of digital goods versioning problems. We establish that even with uniformly distributed types and zero marginal costs (a case where the literature has established that vendors do not offer separate versions), a software vendor will find it optimal to version its product as long as each version has some idiosyncratic risk. Our finding remains valid even as the level of risk becomes small. Because the argument only requires that each version have minimal idiosyncratic risk (i.e., subtle differences between software versions), our finding offers some explanation of the many versions being offered by most software producers.

When comparing economic measures between the versioned (SaaS and on-premises) outcomes with those of a benchmark scenario (on-premises only), we highlight several interesting implications. First, we formally establish that average security losses per user can increase when a software vendor introduces a SaaS version in high security-loss environments. The risk diversification benefits are outweighed by the vendor's pricing behavior with regard to inducing risky consumption. We also show that consumer surplus can decrease in these cases if the inherent quality of the SaaS alternative is sufficiently high. We demonstrate that these effects exist only in high security-loss environments. Thus, in low security-loss environments, security losses always decrease and consumer surplus always increases as a result of the vendor's versioning decision. We also establish that the potential gains in profitability and social welfare relative to benchmarks stemming from a versioning strategy are much larger for high security-loss environments. In fact, in such environments, because of the software vendor's strategic behavior with regard to how it targets its SaaS version to the various consumer market segments, we highlight an opportunity to increase social welfare if the vendor can be encouraged to target SaaS to higher consumer types in cases where it prefers its SaaS version to serve the lower tier of the consumer market.

## 2. Literature Review

Our paper bridges three distinct research areas from the literature on the economics of information systems, information security, and computer science. These three areas are the versioning of information goods, interdependent security risk, and software diversification, respectively. In this section, we describe the current research landscape in each of these areas and discuss in detail the contribution of our paper, which ties the areas together and advances our understanding of the interaction between SaaS versioning and security. We also discuss several papers that are connected to our work and study security and SaaS business models.

Versioning of information goods. Product differentiation is an important research topic in economics. Similarly, the information systems community actively studies the versioning of information goods. Given the ease with which information goods can be versioned and reproduced, digital content owners typically offer several versions of their content. This is readily evident in the software, movie, and music industries. When and how to version, pricing, and which consumer segments to target with each version are all relevant concerns. There is a rich stream of literature on these topics, examining how the versioning decision relates to cost-to-quality ratios, consumer heterogeneity, positive network effects, competition, asymmetric information, group tastes, and free disposal concerns (see, e.g., Bhargava and Choudhary 2001, 2008; Johnson and Myatt 2003; Jing 2007; Jones and Mendelson 2011; Wei and Nault 2011, 2014; Chellappa and Jia 2011; Chellappa and Mehra 2013; Niculescu and Wu 2014). In this literature, a common concern is that when consumers are heterogeneous in their taste for quality, and this taste parameter is uniformly distributed, a software vendor will not find it optimal to version its product. This holds true for information goods where the marginal costs of reproduction are zero. Because such a result is not readily observed in practice, the papers listed above demonstrate conditions under which versioning is optimal by introducing realistic adaptations from this base model. We contribute to this understanding by examining how the software vendor reacts if each version of its product carries some idiosyncratic security risk that endogenously arises as a result of pricing and consumption behaviors in equilibrium. Using our model, we formally establish that even with uniformly distributed tastes and zero marginal costs, a software vendor will always find it optimal to version its product provided that each version has some idiosyncratic risk, even as this risk becomes negligible. Our finding is consistent with the nature of versions being offered by software providers that typically differ on various functionalities, and satisfies the criteria of minimal idiosyncratic risk. In this sense, one contribution of our paper is to demonstrate that security differences in product versions can swing the versioning decision.

Software diversity. Beyond this contribution to the versioning literature, one of the main goals of our paper is to show that for software exposed to security threats, versioning can have substantial implications for the equilibrium security levels faced by consumers. In this vein, our work connects to the literature on software diversity. There is considerable research on the risks of having an IT monoculture and on determining methods that can achieve diversity. IT monoculture refers to deploying similar systems running similar software (Lala and Schneider 2009). Both within and across organizations, a monoculture strategy reduces the cost of learning, management, configuration, and maintenance. However, similar systems share common vulnerabilities that put entire networks of systems running common software at risk from large scale attacks. In this literature, researchers have explored how to introduce artificial diversity via memory randomization (Forrest et al. 1997, Xu et al. 2003, Schneider and Birman 2009), additional redundancy with N-variant systems (Cox et al. 2006, Weatherwax et al. 2009, Gherbi et al. 2011) and, more recently, how diversity results from equilibrium actions in game-theoretic settings (Neti et al. 2012). In Chen et al. (2011), the authors are the first to construct a model that explores the trade-offs among increased security through software diversity, lost network effects, and economies of scale. They find that a firm can benefit more from diversification as software begins to use more standardized interfaces and when adapters and middleware are available to keep applications compatible.

An important consequence of the movement toward cloud-based SaaS offerings is that it can indirectly introduce diversity. For example, Microsoft Office 365 includes enterprise Office Web Apps; this is a virtual version of the most common Office tools such as Word, Excel, and PowerPoint. By providing both a typical on-premises version and a SaaS one, Microsoft achieves software diversity in its Office suite as a consequence of naturally catering to its heterogeneous customer preferences. With the current movement, there is a fitting opportunity to add to the discussion on software diversity by examining settings where consumer demands have driven the need for a particular type of diversity, which can then be leveraged as an opportunity to simultaneously improve security. Our paper contributes to this stream of literature by formally studying the impact of software diversity stemming from SaaS on the security risk properties of the network of users, as driven by benefits from use diversified across versions and changes in security behaviors (e.g., patching and security investment). We quantify these benefits by comparing measures of profitability, security losses, consumer surplus, and social welfare to analogous measures in benchmark scenarios in the absence of software diversity.

Interdependent security risk. A third stream of research closely related to our work centers on security interdependence. One particularly relevant type of interdependence relates to how users of software running on interconnected networks impose security externalities on one another through their usage choices and patching decisions. We examine the diversification benefits associated with having two separate types of risk, directed and undirected, noting that with undirected risk users typically make decisions on whether to patch their individual systems. Therefore, it is important for us to build on prior work that focuses specifically on the trade-off between patching and being exposed to undirected risk. In particular, we build on the foundational model in August and Tunca (2006) which captures how risk faced by unpatched users is related to the number of users who choose to be unpatched in equilibrium. August and Tunca (2006) focus on how patching rebates, mandates, and taxes can improve software security, whereas our research goals focus on security risk diversification through versioning. However, by extending the model in August and Tunca (2006), we can compare security properties of the risk-diversified network, when jointly offering SaaS and on-premises versions, to benchmarks from the base model.

While there are many other studies of the phenomena that involve interdependent security risks (e.g., Kunreuther and Heal 2003, Heal and Kunreuther 2007, August and Tunca 2008, Choi et al. 2010, August and Tunca 2011, Hui et al. 2013, Nochenson et al. 2014), we contribute to this literature by investigating how risk interdependence can be mitigated by designing product substitutes with separate, idiosyncratic risks and allowing users to make choices that endogenously determine the aggregate security risk on the network. Given the scale of economic damage associated with security attacks and the substantial investments in security being made by software providers (Judge 2002, Lewis and Baker 2013), our paper provides insights into the value of software versioning strategies for overall security. These insights are useful to software managers who (i) are making decisions about whether to offer SaaS variants of traditional software packages, and (ii) have also traditionally determined investment levels in product security of on-premises products, which can act as substitutes for versioning strategies for risk diversification. Thus, our research goals are unique, but clearly complement this body of knowledge which aims to put forth a better understanding of managing security risk in the presence of security externalities.

Our paper is related to the broad research area that examines the economics of information security.⁶ We complement research streams on piracy (August and Tunca 2008, Lahiri 2012, Kannan et al. 2013), software liability (Cavusoglu et al. 2008; Kim et al. 2010, 2011; August and Tunca 2011), vulnerability disclosure (Cavusoglu et al. 2007, Arora et al. 2008, Choi et al. 2010), and markets for security (Kannan and Telang 2005, Dey et al. 2012, Ransbotham et al. 2012, Lee et al. 2013) which, similar to our work, all study particular facets of the security problem and recommend strategies to manage risk and improve the value derived from software.⁷ Png and Wang (2009) examine the role of government in facilitating end-user precautions and enforcing laws against attackers, considering both directed and undirected attacks. In our model, we examine how a diversification strategy (releasing both SaaS and on-premises versions) affects directed and undirected attacks on product-specific vulnerabilities to analyze its aggregate impact on security risk.

Last, our work is related to several papers that study various aspects of SaaS versus on-premises business models. Choudhary (2007) examines how SaaS versus perpetual licensing affect a software vendor's incentives to invest in quality. In a two-period model, he establishes that the vendor tends to invest more in quality under a SaaS scheme and that both profits and welfare increase as a result. Zhang and Seidmann (2010) study the licensing problem under network effects and quality uncertainty. They demonstrate that under strong network effects, hybrid models are favorable; in our model, we establish a similar result driven by security risk diversification benefits in contrast to multiperiod dynamics. Huang and Sundararajan (2005) take a more general approach to pricing to characterize optimal nonlinear prices of on-demand computing, while Ma and Seidmann (2014) study competition between various software providers. In our model, we simplify the structure of the SaaS and on-premises alternatives, using a static model that abstracts away from upgrade cycles and multiperiod pricing to elegantly capture software security risk concerns which are the focus of our paper.

## 3. Model Description

A vendor produces software and offers it to a continuum of consumers. The software can be made available in two formats: (i) as a product to be installed at the consumer's location (on-premises), and (ii) as a service installed only on the vendor's systems and accessible by users over the Internet (SaaS). SaaS versions of common software products (e.g., SAP Business ByDesign, Microsoft Office 365, and Microsoft Dynamics CRM On-Demand) are typically streamlined for easier use but include less functionality, require less setup, and offer less integration. In other words, a SaaS version consumer tends to forgo some flexibility in integration with business systems, in the ability to control data, and to manage upgrades (Chow et al. 2009). On the other hand, consumers can derive greater value through a more comprehensive integration with an on-premises version of software that is installed internally and can connect with other systems. Therefore, we model consumer valuations for the on-premises version to be uniformly distributed on V = [0, 1] and assume that if a given consumer has valuation v ∈ V for the on-premises version, she has valuation δv for the SaaS version where 0 < δ < 1.

We assume that the software is used in a network setting, thereby exposing purchasing consumers to additional risk associated with the software's use. This risk comes in the form of directed and undirected security attacks, which are both described in §1. We denote the probability that a directed attack occurs on the network with 0 < πd < 1 (we use d to signify directed). Conditional on a directed attack having occurred on the network, we assume that the likelihood that any given network location (node) is victimized is proportional to the mass of consumers at that node (Greenemeier and Hoover 2007, Roy 2011). Therefore, the total likelihood of a node that services d consumers being attacked is πdd. Similarly, we denote the probability that a patchable security vulnerability arises in the software and that an undirected attack on that vulnerability occurs with 0 < πu < 1 (we use u to signify undirected). Given the spreading mechanics of undirected security attacks such as worms, if the mass of the unpatched population in the network is u, the unconditional probability that the worm will attack an unpatched user's system is given by πuu.

Because the SaaS version is only installed at one node (on the vendor's system), under the above model specification users of the SaaS version are primarily exposed to directed risk, which increases with the size of the total SaaS user population. In contrast, the on-premises version carries minimal directed risk because a given node is negligible compared to the size of the total number of on-premises nodes (a subset of the continuum V). However, because of the many widespread nodes running the on-premises product, this version is exposed to considerable undirected risk, which is proportional to the size of the user base that remains unpatched. In our model specification, we have attempted to maintain the simplest structure where the SaaS and on-premises versions face idiosyncratic security risks, each having a security externality dependent on user behavior. Such a structure will permit us to analytically explore the impact of versioning on security and produce clear insights.

If a user is struck by a directed or undirected security attack, one would expect that she suffers a loss positively correlated with her valuation. That is, consumers with high valuations will incur greater losses than consumers with lower valuations due to higher opportunity costs, higher criticality of data, and loss of business. For simplicity, we assume the correlation is of the first order, i.e., the loss that a consumer with valuation v incurs if she is hit by the attack is either αv for an on-premises product or αδv for SaaS, where α > 0 is a constant. Undirected attacks typically exploit known vulnerabilities for which a patch is already available, hence each consumer has an opportunity to patch in the face of this security risk. If a consumer chooses to patch the software, she will incur an expected cost of patching denoted as 0 < cp < 1, which accounts for the money and effort that a consumer must exert to verify, test, and roll out patched versions of existing systems.

There are three decision periods. In the first, the vendor determines which versions of its software to release and sets a product price p > 0 for a single server license for its on-premises version and a service price ps > 0 for its SaaS version. In the second period, given the price and security risk of each software offering, each consumer makes a decision whether to purchase the software as well as which version to purchase. Finally, in the third period, if a patchable security vulnerability has been discovered, each consumer who purchased the on-premises version determines whether to patch her own system. Subsequent to these decision periods, both directed and undirected attacks may occur on the network and consumers incur losses.

Each consumer makes a purchasing decision to buy the on-premises product version, OP, buy the SaaS version, SaaS, or not to buy either offering, N. Similarly, if a patchable vulnerability arises in the software, each user of the on-premises version makes a decision to patch, P, or not to patch, NP, her own system. If the consumer has chosen SaaS or N, she does not make a patching decision as in the on-premises case, which we denote by ND. We denote the consumer action space by S = ({OP} × {P, NP}) ∪ ({SaaS, N} × {ND}). Given prices, in a consumer market equilibrium each consumer maximizes her expected utility given the equilibrium strategies of all other consumers. For a strategy profile σ: V → S, the expected cost faced by the consumer with valuation v is then defined by

C(v, σ) =
  Cp, if σ(v) = (OP, P);
  πu u(σ)αv, if σ(v) = (OP, NP);
  πd d(σ)αδv, if σ(v) = (SaaS, ND);
  0, if σ(v) = (N, ND),

where the size of the unpatched user population of the on-premises version is given by

u(σ) = ∫V 1{σ(v)=(OP,NP)} dv,

and the size of the user population of the SaaS version (most vulnerable to a directed attack) is given by

d(σ) = ∫V 1{σ(v)=(SaaS,ND)} dv,

where 1 is the indicator function. For expositional convenience, we also define the size of the patched population using the on-premises product as

n(σ) = ∫V 1{σ(v)=(OP,P)} dv.

Our main research goal is to assess the security impact that stems from risk diversification benefits associated with a software vendor's versioning strategy as it extends into SaaS markets. To do so, we use the benchmark model from August and Tunca (2006) to compare security risk characteristics. In their model of undirected security risk, users make use and patching decisions, and the vendor sets the product price. In this paper, we model the on-premises software product so that it is consistent with August and Tunca (2006).¹⁰ However, to study risk diversification in the context of SaaS versioning, we also model a SaaS version with its own idiosyncratic risk. This directed risk reflects a security externality that is structurally different and unique from the externality stemming from unpatched use of the on-premises version. By modeling both on-premises and SaaS versions with separate externalities, we analyze how versioning in this manner affects pricing and user incentives, which then determine the security characteristics of this more complex software network. Finally, by being consistent with prior work, when δ = 0, the SaaS version has no inherent value to users (in which case consumers purchase on-premises products or remain out of the market). Our model then collapses to August and Tunca (2006), which we will refer to as the benchmark case, i.e., having only an on-premises offering.

## 4. Consumer Choice and Vendor Profit Maximization

### 4.1. Consumer Market Equilibrium

To study the software vendor's versioning problem and the subsequent security properties of the network, we first develop an understanding of how consumers strategically determine whether to adopt an on-premises product or a SaaS solution. In this section, we take prices as given and study the choice problem faced by consumers who strategically interact due to version-specific security externalities associated with each alternative. Holding all other consumers' strategies fixed to σ_, the consumer with valuation v determines her optimal action by solving the following maximization problem

max { (v - p) · 1{s=(OP, P), (OP, NP)} + (δv - ps) · 1{s=(SaaS, ND)} – C(v, σ) },
s∈S

where the strategy profile σ is composed of σ_τ (other consumers' strategies) and the choice being made, i.e., σ(v) = s. We denote her optimal action that solves (5) with s*(v). An equilibrium strategy profile σ* must satisfy σ*(v) = s*(v) for all v∈V.

In the following lemma, we provide a full characterization of equilibrium consumer behavior for all prices and exogenous security and quality parameters in our model.

**LEMMA 1.** Given on-premises product and SaaS prices, p∈ (0, 1) and ps ∈ (0, δ), respectively, and other parameters cp, πd, πu, and δ, a unique equilibrium in the consumer market exists.¹¹ The equilibrium consumer strategy profile σ* is characterized by thresholds va, vu, vp ∈ [0, 1] such that for v ∈ V, it satisfies either

σ*(v) =
  (OP, P), if vp < v ≤ 1;
  (OP, NP), if vu < v ≤ vp;
  (SaaS, ND), if va < v ≤ vu;
  (N, ND), if 0 ≤ v≤va,

or

σ*(v) =
  (OP, P) if vp < v ≤ 1;
  (SaaS, ND) if va < v ≤ vp;
  (OP, NP) if vu < v ≤ va;
  (N, ND) if 0 ≤ v≤ vu

Lemma 1 formally establishes that the consumer market exhibits a threshold structure.¹² Common to both possible equilibrium strategy profiles, as seen in (6) and (7), the consumers with highest valuations for the software choose the on-premises product and patch to avoid undirected security attacks in equilibrium. Thus, there is a patching threshold, denoted by vp, such that all consumers with valuations above this threshold value use this strategy, i.e., σ*(v) = (OP, P) for all v > vp. As motivated before, the on-premises product alternative carries the highest inherent quality; this reflects the ability of a consumer to more fully integrate this product with her own systems and take advantage of greater functionality. As a result, we would expect the equilibrium outcome to reflect that the highest valuation users prefer the on-premises product and fully protect their value by patching.

However, one relevant consequence of consumers' strategic behavior highlighted by Lemma 1 concerns the effective quality ordering of the SaaS alternative and the on-premises software in an unpatched state. In particular, for the next consumer valuation interval directly below vu, either unpatched on-premises product users, who choose (OP, NP), or SaaS users, who choose (SaaS, ND), compose the subsequent lower set of valuations, corresponding to the strategy profiles in (6) and (7), respectively. Given that consumers inherently prefer the on-premises product to SaaS (because v > δv), it is more natural to think that the SaaS version would be consumed by the lowest consumer segment remaining in the user population as in (6).

The fact that there can exist a segment of consumers choosing (SaaS, ND) in equilibrium and having higher valuations than consumers in a segment choosing (OP, NP) as in (7) firmly demonstrates the role of idiosyncratic security externalities in shaping the equilibrium outcome. In this case, the effective quality of the SaaS version when adjusted for its exposure to directed security attacks, which is influenced by pricing and the number of users choosing the SaaS version, can actually be higher than the quality associated with using the on-premises version and not patching. For instance, higher valuation users may prefer slightly lower inherent quality software if it is used by very few users and is considerably more secure than higher inherent quality software with a large unpatched population and considerable undirected risk. Significantly, the effective quality of each product is endogenously determined by consumer behavior. Thus, it is the strategic interactions that drive the effective quality ordering found in (7). If the on-premises and SaaS versions did not have unique exposures to different risks, the higher consumer valuation segment would not, ordinarily, consume the lower inherent quality product.

Similar to our definition of the patching threshold vp, the SaaS threshold va marks the valuation above which (up to the next higher threshold) consumers prefer to use SaaS and tolerate exposure to directed security risk. Last, we denote the on-premises purchasing threshold with vu, which marks the valuation above which (again, up to the next higher threshold) consumers prefer to use the on-premises product and not patch in equilibrium. By not patching, these consumers will be exposed to undirected security risk. Because of the threshold structure presented in Lemma 1, there are three distinct consumer market segments represented in equilibrium as characterized by these intervals in the consumer valuation space. For convenience in exposition, we refer to these intervals as high tier, middle tier, and low tier, corresponding to (vp, 1], (vu, vp], and (va, vu], respectively, for (6), and (vp, 1], (va, vp], and (vu, va], respectively, when the characterization in (7) arises in equilibrium. When only two consumer market segments arise in equilibrium (i.e., when vu = 1 meaning no consumer prefers (OP, P) the other alternatives), we simply refer to the two ordered segments as high tier and low tier.

### 4.2. Vendor Profit Maximization

Next, we formally present the software vendor's pricing problem and define measures of security losses, social welfare, and consumer surplus. Using the measures defined in (2)-(4), the vendor's profit function can be written as follows:

Π(p, ps) = p[u(σ*) + n(σ*)]+psd(σ*),

where the size of each population depends on the equilibrium strategy profile which, in turn, is a function of prices, i.e., σ* = σ*(· |p, ps).¹³ The vendor's profit maximization problem can then be expressed as follows:

max Π(p, ps)
(p, ps)∈[0, 1]×[0, δ]
s.t. (va, vu, vp) are given by σ*(·|p, ps).

In addition to characterizing the optimal prices in (9) and the corresponding equilibrium consumer market structures under these prices, we also examine measures of security risk, consumer surplus, and social welfare for these outcomes.

To facilitate the ensuing discussion, under a set of prices (p, ps), we denote the total security losses as SL and define it as the sum of expected losses from undirected security attacks, directed security attacks, and patching costs under the equilibrium strategy profile σ*(· | p, ps), i.e.,

SL = ∫V 1{σ*(v)=(OP, NP)} πu u(σ*)αvdv + ∫V 1{σ*(v)=(SaaS, ND)} πd d(σ*)αδvdv + cpn(σ*).

Social welfare can then be measured as

W = ∫V [1{σ*(v)∈{(OP, P), (OP, NP)}} v + 1{σ*(v)=(SaaS, ND)} δv] dv – SL,

which is the difference between the aggregate value derived from the software and these losses. Finally, consumer surplus is defined by

CS = W – Π(p, ps).

For the benefit of the reader, we briefly outline how we will structure our presentation of results going forward. Using the equilibrium consumer market characterization above, in the next two sections we separately examine high security-loss environments (high α) and low security-loss environments (low α). As noted above, because of the complexity of the general characterization of the equilibrium, it is too extensive to fully include in the exposition. However, when focused on a high or low security-loss environment, this equilibrium characterization simplifies considerably. Thus, for each environment, we first present greater details on parameter boundaries of feasible regions. We then examine the vendor's pricing problem and study its versioning decision. In light of the vendor's optimal pricing and the associated consumer market outcome, we carefully examine how versioning affects security, consumer surplus, and social welfare, as determined by patching costs (cp), SaaS quality (δ), and the security loss factor (α). As part of our analysis, we compare these outcomes with those obtained when only an on-premises solution is offered. We consider this to be the benchmark case. Finally, we conclude our study by examining how the software vendor's security investment decisions interact with its versioning choice, which we present as an extension to our model.

## 5. High Security-Loss Environment

We begin by studying a high security-loss environment where consumers are subject to large economic losses if struck by security attacks. Specifically, in the loss model, the parameter α specifies the magnitude of loss correlation with valuation. In this section we examine the vendor's problem when α is large. High security-loss environments are common and often reflect the reality of current network software security: Some users are patching their on-premises software installations when vulnerabilities arise to prevent potential security breaches; other users do not patch because of the associated costs. Enterprise software is typically classified as a high security-loss environment. This is why many organizations use a planned and systematic approach for deploying patches on such systems (Bloor 2003, Boulton 2013, Kash 2013). Similarly, SaaS providers of enterprise software are diligently addressing vulnerabilities to protect the interests of their customers (Branscombe 2012, Microsoft 2013). Microsoft IIS, Microsoft Dynamics, and SAP Business One are examples of enterprise software that businesses use and rely on for their day-to-day operations. When enterprise systems such as the above are successfully attacked and compromised, the affected businesses often incur large economic losses associated with lost sales, customer goodwill, reputation, IT human resources, and information (Lewis and Baker 2013).

First, following Lemma 1, we present a characterization of the three regions that can arise in the consumer market equilibrium when the security loss factor α becomes high.

**COROLLARY 1 (EQUILIBRIUM UNDER HIGH α).** Given on-premises product and SaaS prices, p ∈ (0, 1 – cp) and ps ∈ (0, δ), respectively, and other parameters cp, πd, πu, and δ, the equilibrium consumer strategy profile σ* satisfies:
Region I (No SaaS). If ps > δcp, p < ps/δ – cp, and α > αβ = cp(1 − cp)/(πu(1 − cp – p)), then p < vu < vp < 1 and σ* is given by either (6) with va = vu or (7) with va = vp.
Region II (SaaS for low tier). If p > max(ps/δ – cp, ps) and α > max(α1 = δ(ps – pδ)²/(πuр²((p + cp)δ – ps)), â1), where â1 is the unique root greater than cp/πu that satisfies g1(α) = 0 where

g1(α) = δ + √πu / (δπα) * (4ραπd + (1 - απu + πd)² - α) / (2(1 - cp))

then ps < va < vu < vp <1 and σ* is given by (6).
Region III (SaaS for middle tier). If ps < δcp/(1 − δ), ps/δ - cp < p < ps, and α > max(cp(1 – δ)²(p - ps + cpδ) / (p - ps)²πu, α2), where α2 is the unique positive root that satisfies g2(α) = 0 where

g2(α) = 1 - 2(p + cp - ps) / (Φπu) + απu / (δπα) * (4ραπd + (1 - απu + πd)² - α) / (2(1 - cp))

and Φ = p − (1 – cp) + (δ – ps), then ps < vu < va < vp < 1 and σ* is given by (7).¹⁴

By Regions II and III of Corollary 1, when the use of SaaS arises in equilibrium, the threshold valuations satisfy vp > vu > va or vp > va > vu, respectively. In the latter case, the SaaS alternative is preferred by the middle tier of the consumer market. Then, by (8), the vendor's profit function in Region III can be expressed as follows:

Π(p, ps) = p(1 − vp + va - vu) + ps(vp – va).

We will subsequently refer to the prices that maximize (15), subject to the constraint that they induce a middle-tier SaaS consumer market structure, with pM and pM. The corresponding profits are denoted by ΠM ≤ Π(pM, pM). Similarly, by (10), security losses are now simplified to

SL = [α(πu(va-vu)(04-02)+δπd(vp-va)(0-0))]/2 + cp(1-vp),

and social welfare can be expressed as follows:

W = [1-03+0-02 +δ(03-02) – α(πu(va - vu) (04-02) +δπd(vp-va) (0-0))]/2-cp(1-p).

On the other hand, when the SaaS alternative is preferred by the lower tier of the market, i.e., vp > vu > va as in Region II of Corollary 1, the vendor's profit function can be expressed as follows:

Π(p, ps) = p(1 – vu) + ps(vu – va).

Analogously, pL and pL will denote the prices that maximize (18), constrained such that they induce a low-tier SaaS consumer market structure; the respective profits will be denoted by ΠL ≡ Π(pL, pL). For this structure, the security losses and welfare are given by

SL = [α(πu(vp-vu)(03-02)+δπd(vu-va)(02-04))]/2 + cp(1-vp),

and

W = [1 - 0² + δ(0 – 02) – α(πu (vp – 1)(03-02) + δπd(0 – 0) (0 – 02))]/2 – cp(1 – vp),

**PROPOSITION 1.** For high security-loss environments,¹⁵ (i) when patching costs and the SaaS alternative's quality are both high, i.e., cp > 1/3 and δ > (2(1 − cp))/(1 + cp), a software vendor can maximize profits by setting prices such that the middle tier of the consumer market prefers the SaaS offering; (ii) otherwise, the vendor sets prices so that the SaaS alternative is geared for the lower tier of the consumer market.

In high security-loss environments, there can be substantial consumer benefits associated with a reduction in the magnitude of security losses. When the consumer population is induced to separate use across on-premises and SaaS offerings, these losses are mitigated through diversification. Proposition 1 establishes that in these environments the vendor should version by setting prices such that all three user populations (patched on-premises users, unpatched on-premises users, and SaaS users) are represented in equilibrium. By inducing a population of SaaS users, the vendor has removed a large mass of potentially unpatched hosts from the network; because of patching costs, in the absence of a SaaS version, many of these users would not patch as on-premises product users. Thus, offering SaaS can help reduce the risk faced by remaining unpatched on-premises product users because, by (1) and (2), the risk these users face is proportional to the size of unpatched users population in equilibrium. Although the SaaS users do not bear undirected risk comparable to on-premises users, they now face considerable directed risk as a large node on the network. However, pricing the SaaS version to induce them to accept some directed risk helps diversify security risk within the network.

First, we discuss part (ii) of Proposition 1. When patching costs are small and security risk is large, consumers have strong incentives to patch when using on-premises software. In this case, the vendor can both charge a high price for its on-premises software and keep the security risk faced by unpatched on-premises users low because they remain a relatively small population within the network. This limits the impact of their security externality. Because of the vendor's pricing power associated with on-premises software, it should set the price of its SaaS offering to prevent cannibalization but still serve the lower tier of the consumer market. Part (ii) of Proposition 1 is illustrated in panels (a) and (b) of Figure 1. Because δ=0.80, the condition δ < 2(1 − cp)/(1 + cp) is satisfied whenever cp < 3/7 as indicated by the area labeled A in the figure. Within this area, the optimal prices are given by pL and pL, satisfying pL < pL, which gives rise to a low-tier SaaS structure characterized by vp > vu > va as is illustrated in panel (b) of Figure 1.

In area A of panel (a), as patching costs (cp) increase, the price of the on-premises version (pL) decreases, but the price of the SaaS version (pL) first decreases and then increases. To see why, first note that an increase in patching costs reduces the patching population of the on-premises version. Moreover, because of the negative security externalities associated with unpatched behavior, overall use will also decline, which reduces vendor profitability. In this case, the vendor must reduce pL to help maintain a sizeable patching population, as well as to encourage unpatched on-premises users, who now face greater risk, to remain in the user population. However, under high security risk, the vendor also needs to throttle growth in the size of the risky populations as more users elect not to patch because of increased patching costs. To achieve this objective, the vendor must carefully adapt its SaaS price, ps. If it lowers ps, more users at the lower end of the valuation space will become SaaS users. This increases the risk associated with SaaS and, in turn, provides disincentives for members of the larger on-premises unpatched population to switch to SaaS. As a result, both of these risky populations could grow substantially. Instead, the vendor must raise ps, which prevents low valuation users from entering and leads to a comparatively smaller increase in the size of the risky populations, as in the right-hand portion of area A in Figure 1. However, when patching costs are low, as in the left-hand portion of area A in panel (a), or when security risk is still high but slightly lower as in panel (c) where α = 20, the impact of a slightly larger unpatched, on-premises user population and SaaS user population is not as detrimental. As a result, the vendor prefers to reduce pL to provide incentives for users to diversify risky use across on-premises and SaaS versions.

Proposition 1 establishes that as patching costs increase, there exists a point at which the vendor alters his strategy, i.e., jumping up its SaaS price from pL to pM, and jumping down its on-premises price from pL to pM. This can be seen in panel (a) of Figure 1 as a move from area A (Region II in Corollary 1) to B (Region III in Corollary 1) for a security loss factor of α = 200. Similarly, in panel (c) of Figure 1, the same effect is shown as a shift from area C to D for a security loss factor one order smaller. At this point, due to substantial patching costs, even though the vendor lowers the on-premises product price, it will face a larger unpatched population and reduced use due to the negative externality these users impose. Although its SaaS product may have slightly lower base quality, when accounting for the security externalities, this may not be the case. This outcome is noteworthy because in typical product differentiation problems, the higher quality product is consumed by the higher value consumers, while the lower quality product is priced for the less quality-sensitive segment (see, e.g., Bhargava and Choudhary 2001, 2008; Johnson and Myatt 2003).

Contributing to the versioning literature above, we establish a unique, inverse versioning result in the presence of two idiosyncratic security externalities; specifically, in our setting, the on-premises version is clearly assumed to be of higher quality (i.e., a type v consumer derives value v from the on-premises product and δv from the SaaS product where δ < 1). However, the security risk associated with each version is endogenously determined in equilibrium, being affected by vendor pricing and strategic consumption behavior. Here, we see that it is possible that the vendor will set prices to induce an outcome where the inherently lower quality SaaS version endogenously has higher effective quality. Specifically, as we cross the aforementioned boundary in patching costs, the vendor strategically prices its SaaS product at a higher level, i.e., it targets a smaller, higher-value population; this is accompanied by a smaller directed risk. Because users of the SaaS option are exposed to negligible undirected risk, the vendor's pricing induces an outcome whereby medium valuation users will prefer the SaaS option over the lower value unpatched on-premises offering that faces considerable undirected security risk. In panel (b) of Figure 1, the area labeled B shows how the thresholds induced by its pricing flip to vu > va > vu, leading to a middle-tier SaaS outcome; portion D of panel (d) is similar.

One final point also illustrated in panels (c) and (d) of Figure 1 is another pricing strategy change at the junction between areas D and E. When the magnitude of security losses is not too high (i.e., α = 20) and patching costs increase to a larger level, the vendor is incentivized to significantly increase its on-premises product price to reduce the size of the purchasing on-premises population thus limiting the negative security externality to an extent wherein these consumers now have much reduced incentives to patch their products. Rather than continuing to cut its on-premises price to ensure that a patching population exists to limit undirected security risk, a substantial price increase allows the vendor to serve only the highest valuation market with its on-premises product. Complementing this strategic price increase is a drop in its SaaS price to capture more of the market at the lower end. However, for any level of patching costs, as the security loss factor grows high enough, area E as depicted in Figure 1 disappears due to the large losses users incur when being unpatched; this is the essence of Proposition 1.

Having developed an understanding of the conditions under which the vendor targets its SaaS product to the middle and lower tiers of the consumer market, we next study how its versioning strategy affects social welfare. We aim to highlight which of the two consumer market characterizations that arise under optimal vendor pricing, as fully described in Proposition 1, is socially preferable. We also particularly identify regions in which welfare can be increased if the vendor were incentivized to induce the market outcome that goes against its preference.

**PROPOSITION 2.** For high security-loss environments, when patching costs are within an intermediate range and the SaaS alternative's quality is high, i.e., cp < cp <1/3 and δ > η, social welfare can be increased if incentives are provided to encourage the software vendor to target its SaaS alternative to the middle tier rather than the lower tier of the consumer market. However, for most other levels of patching costs and SaaS quality, the vendor-preferred outcome is also better for welfare. Technically, there exist cp > (17–4√15)/7 and η > (2(7 – 14cp + 3c²))/((7 – cp)(1+cp)) such that
(i) If cp < cp <1/3 and δ > η, then W|p*, p* < W|pM,pM;
(ii) If δ < (2(7 – 14cp + 3c²))/((7 – cp)(1 + cp)), or cp > 1/3 and δ > (2(1 − cp))/(1 + cp), then W|p*, p = max(WL, WM),
where WL and WM denote the welfare associated with equilibrium outcomes in Regions II and III, respectively.¹⁶

Proposition 2 establishes that there exists an interval of patching costs where the vendor will prefer to induce a low-tier SaaS outcome characterized by vp > vu > va (Region II of Corollary 1) with its pricing, whereas social welfare would be strictly higher if it is priced at pM and pM to induce the middle-tier SaaS, vp > va > vu (Region III of Corollary 1) consumer market outcome. The rationale here is that when the vendor adapts its strategy to target the SaaS offering to the middle tier of the consumer market, it effectively increases the size of the patched population by dropping the on-premises price and restricts the size of the SaaS user population by increasing the SaaS price. Combining these effects, the total security losses on the network are smaller which, in aggregate, leads to higher welfare, despite the negative impact of restricted use. Part (i) of Proposition 2 establishes that there exist intervals near the upper bound on patching costs and near the lower bound on the SaaS quality parameter where providing external incentives to the vendor and/or users may help encourage the socially-preferable outcome. However, part (ii) of the proposition also establishes that, in many cases, an outcome wherein the SaaS alternative is directed to the lower tier of the consumer market is also consistent with welfare considerations.

### 5.2. Comparison to Benchmark

In this section, we examine how a software vendor's decision to release SaaS versions of its traditionally on-premises software product (as detailed in §5.1) affects profitability, social welfare, and the security properties of the network relative to benchmark outcomes where only an on-premises offering is made. Additionally, we study the impact of introducing SaaS on consumer surplus. For convenience, we use the subscript BM to denote that the measure is under the benchmark outcome where the on-premises version is the sole offering.

**Lemma 2 (BENCHMARK UNDER HIGH α).** For high security-loss environments without SaaS versioning (i.e., δ = 0), under optimal pricing there always exists a positive mass of customers who prefer patching on-premises software (OP, P) and a positive mass of consumers who prefer to use on-premises software but not patch it (OP, NP). The equilibrium purchasing and patching thresholds satisfy 0 < vu < vp < 1.

Lemma 2 shows that when the quality of the SaaS offering goes to zero, or equivalently SaaS is not offered, the vendor will set the on-premises price to induce both patched and unpatched populations in equilibrium. In a high security-loss environment, the unpatched population is exposed to significant undirected security risk and shrinks to help limit the security externality. The case where δ = 0 is a special case where our model converges to the model in August and Tunca (2006), hence the equilibrium pricing and market structure characterization are both consistent. This case is an appropriate benchmark for comparison of economic and security measures when δ > 0 and versioning occurs.¹⁷

First, we examine profitability and welfare comparisons with the benchmark solution. Proposition 1 establishes that, for high security-loss environments, the software vendor will release both alternatives and target the SaaS version to the middle tier when patching costs (cp) are high; the SaaS version has similar quality (i.e., high δ). In the following proposition, we demonstrate that a joint offering strategy substantially increases profits and social welfare. Furthermore, we characterize how cp, δ, and the likelihood of a directed attack on the SaaS offering (πd) affect the extent to which the outcome of the joint offering improves these measures.

**PROPOSITION 3.** For high security-loss environments, both vendor profits and social welfare can increase substantially under a joint offering strategy. Both relative measures of improvement are increasing in patching costs and the quality of the SaaS version, but decreasing in the likelihood of directed attacks. Technically, there exists ῳ, κ > 0 such that for all α > ῳ,

(Π* – ΠBM) / ΠBM < κ / α²
and
(W* - WBM) / WBM < κ / α²

are satisfied.

Proposition 3 establishes that the introduction of a SaaS offering can result in substantial percentage increases in profits and social welfare. Examining the inequalities in (21) and (22), it is straightforward to see that both normalized measures decrease in πd but increase in cp and δ. A decrease in πd corresponds to reduced directed security risk for consumers who use the SaaS alternative in equilibrium. In a similar vein, an increase in δ also reflects a higher quality SaaS offering, which is beneficial to both vendor profitability and social welfare. On the other hand, for cp, the potential improvement associated with a SaaS release stems from consumers' patching behavior of the on-premises solution. In particular, as patching costs increase, consumers find it incentive compatible to bear more undirected security risk rather than incurring these patching costs. Given the negative externalities unpatched users can inflict on the network, under these circumstances, introducing the SaaS alternative can have an even stronger effect by inducing consumers to split use across alternatives and diversify this security risk to include more directed risk (and less undirected risk).

Next, focusing on high security-loss environments, which have the greatest potential for improvement, we examine how introducing a SaaS alternative affects the security properties of the network as well as consumer surplus. By (10), we can define the average per-user security losses as follows:

SL / (u(σ*) + d(σ*) + n(σ*)),

which simplifies to either SL/(1 − va) or SL/(1 − vu) in Regions II and III of Corollary 1, respectively.

**PROPOSITION 4.** When a SaaS version is introduced in high security-loss environments:
(i) The average security losses per user decrease under high patching costs, i.e., cp ≥ δ/(4 – δ), but actually increase otherwise;
(ii) Despite the substantial increase in welfare stemming from a SaaS release, when patching costs are low, i.e., cp ≤1/3, and the SaaS offering quality parameter satisfies δ > 2 − (64cπd (1 – cp (4-cp)))/(πu(1+cp)²), consumer surplus decreases in equilibrium.

Part (i) of Proposition 4 reveals an important insight: A vendor's diversification of software use by offering both on-premises and SaaS versions can actually increase per-user security losses. One would expect that introducing a SaaS alternative would split the undirected risk being faced in the benchmark case into two smaller risks (undirected and directed), as a portion of the consumers adopt the SaaS alternative instead. However, part (i) of Proposition 4 establishes that a software vendor may influence use and patching behavior through pricing in such a way that the average security losses per user is higher in the joint offering.

In high security-loss environments, when SaaS is introduced, some consumers who would have elected to buy the on-premises product and remain unpatched, i.e., (OP, NP), in the benchmark case now have incentives to switch to SaaS, i.e., (SaaS, ND). Because this reduces the size of the unpatched population, consumers who were buying the on-premises product and patching, i.e., (OP, P), are no longer facing as large a negative externality. Therefore, they have overall reduced incentives to patch, and some of these consumers will now elect to remain unpatched. Also, because introduction of SaaS splits risk into undirected and directed types, some consumers who had opted out in the benchmark case will now become users. Thus, in comparison to the benchmark case, when both on-premises and SaaS versions are offered, overall use increases while overall patching decreases.

Part (i) of Proposition 4 establishes that when patching costs are small, the aforementioned cumulative effect of increased use and decreased patching associated with the introduction of SaaS results in higher average per-user security losses. When patching costs are small, the consumer market structure is already characterized by a large patching population in the benchmark case. The population of unpatched on-premises users is, by contrast, relatively small. Hence, when SaaS is introduced, although patching slightly decreases, the proportional increase in either unpatched or SaaS use is substantial. A relatively large increase in these two types of use, which are exposed to undirected and directed security risk, respectively, can lead to higher average per-user security losses because of the accompanying negative externalities. On the other hand, when patching costs are large, the benchmark case is characterized by a small patching population and large unpatched population. In this case, aggregate SaaS and unpatched on-premises use still increases while patching decreases. However, the reduction in patching behavior has a relatively minor negative effect on an already substantial unpatched population. In contrast to the case above, the diversification benefits of splitting security risk into undirected and directed types now outweighs the minor increase in the externality. Thus, for large patching costs, per-user security losses decrease when SaaS is made available.

One might expect that consumer surplus would increase when a software vendor offers a menu of differentiated products with idiosyncratic security risks, but that is not always the case as we establish in part (ii) of Proposition 4. Because, surprisingly, average per-user security losses can increase when a software vendor introduces a SaaS version of its on-premises product, from a consumer perspective such a release may not necessarily be beneficial. Part (ii) of Proposition 4 suggests that for software with relatively lower patching costs (such as client applications), a vendor will release a SaaS version not for the benefits of reduced security risk but rather to expand its market at the lower end and price discriminate. The net effect of its joint offerings on consumer surplus is negative, which is partly driven by the increase in security losses formalized in part (i) of Proposition 4.

## 6. Low Security-Loss Environment

For additional insight into the overall security landscape, we next examine environments where consumers are subject to smaller economic losses associated with security attacks. Here we focus on a class where α is small, and study software applications belonging to this class such as client applications that are less mission critical to business operations. Some examples include anti-virus client software, media players, document readers, and perhaps even productivity software such as Microsoft Office 365. We take a similar approach to §5 by further characterizing the consumer market equilibrium, which is simplified when considering only a low security-loss environment. Subsequently, we examine the vendor's versioning decision and compare profitability, social welfare, security losses, and consumer surplus to the benchmark measures for this case.

As the security loss factor α decreases, users of on-premises software will find it better to assume undirected security risk than to incur patching costs. Thus, a patching population will not arise in equilibrium as is formalized in the following corollary.

**COROLLARY 2 (EQUILIBRIUM Under Low α).** Given on-premises and SaaS prices, p ∈ (0, 1) and ps ∈ (0, δ), respectively, and other parameters cp, πd, πu, and δ, the equilibrium consumer strategy profile σ* satisfies:
Region I (No SaaS). If p ≤ ps/δ and α ≤ min(αβ, αA) ⇒ δ(ps-pδ)/(psπd(δ−ps)), αC ≡ (1−p+ps – δ)(p – ps + δ)/(πu(δ – ps)), then p < vu <1 and σ* is given by either (6) with va = vu and vu =1 or (7) with va = vp=1.
Region II (SaaS for low tier). If ps/δ < p < 1 + ps – δ and α ≤ â1, then ps < va < vu <1 and σ* is given by (6) with vu = 1.
Region III (SaaS only). If 1+ps − δ < p and α ≤ αP = (1 − p + ps)(p − 1 − ps + δ)/(δπd(1 − p)), then ps < va < 1 and σ* is given by either (6) with vu = vp =1 or (7) with vu = va and vp = 1.

As can be seen in Corollary 2, in equilibrium, there are three possibilities for the consumer market structure: the on-premises version is preferred by all users and not patched (Region I); higher valuation users prefer the on-premises version and do not patch while lower valuation users prefer SaaS (Region II); and finally all users prefer SaaS (Region III). Given this consumer market outcome, we next analyze the vendor's versioning problem.

### 6.1. Versioning Strategy

As presented in Proposition 1, in high security-loss environments, the vendor has strong incentives to release a SaaS offering to change the structure of the network and reduce security risk by splitting the user population; this helps to limit both directed and undirected security attacks, which are influenced by total SaaS user and unpatched on-premises population sizes, respectively. In high security-loss environments, the margin for improvement is large. However, as the security loss factor decreases, the benefit of risk diversification becomes more limited. An open question in the literature is whether versioning makes sense in the presence of security externalities as their impact decreases.

**PROPOSITION 5.** In low security-loss environments,¹⁸ a software vendor still prefers to offer both on-premises and SaaS versions of its software.

In contrast to Proposition 1, one might expect that as the security risk associated with software decreases a software vendor would shift toward a strategy where it prices its offerings in such a way that only the higher quality offering is consumed. This outcome would be consistent with the literature on versioning of information goods. Specifically, in the absence of unit costs and when consumer valuations (or quality sensitivities) are uniformly distributed, a monopolist with two different quality substitutes will price them such that only the high quality substitute is consumed in equilibrium. In other words, in such a case, the vendor will not version its product. Because versioning is frequently observed with information goods, the literature on versioning of information goods has worked to reconcile this inconsistency.

Proposition 5 examines this versioning issue from a security perspective. Specifically, in the absence of the negative security externalities present in our model, because consumers have uniform valuations and the SaaS offering has a quality reduction factor, consistent with the versioning literature, the vendor would optimally offer only the higher quality information good. However, when consumers of both versions are exposed to negative security externalities in the form of directed risk for the SaaS offering and undirected risk for the on-premises offering, Proposition 5 establishes that it is still optimal for the vendor to offer both versions even in low security-loss environments. In fact, as α diminishes, we analytically demonstrate that it is always profitable to introduce the SaaS offering. In our case, the fact that each product is exposed to a unique externality (directed or undirected risk) creates the separation necessary for versioning to become optimal. From a practical standpoint, this result provides another alternative explanation for the commonplace existence of multiple versions of software products: As long as the versions have some idiosyncratic risk stemming from their respective user populations, however small, it is profit-maximizing to set prices such that both versions are consumed in equilibrium.

### 6.2. Comparison to Benchmark

Analogous to §5.2, next we examine how a software vendor's optimal decision to release a SaaS version of its product (as established in Proposition 5) affects profitability, social welfare, security losses, and consumer surplus in comparison to a benchmark. As before, for an appropriate benchmark, we use measures computed under the equilibrium solution to the case wherein δ = 0, which is to say that the on-premises software is the sole offering. These benchmark measures then coincide with those computed in August and Tunca (2006).

**LEMMA 3 (BENCHMARK Under Low α).** For low security-loss environments without SaaS versioning (i.e., δ = 0), under optimal pricing there is only a positive mass of customers who prefer not to patch on-premises software (OP, NP) in equilibrium. The equilibrium purchasing and patching thresholds satisfy 0 < vu < vp = 1.

The benchmark equilibrium characterized in Lemma 3 is similar to the outcome that unfolds from Corollary 2 and Proposition 5 in that no consumer will find it optimal to patch her on-premises software in equilibrium. Thus, all users face some degree of undirected security risk even though it is low, while under the versioning outcome in Proposition 5, risk is diversified as users separate into on-premises and SaaS user populations. Next, we compare these two outcomes.¹⁹

For low security-loss environments, we characterize the relative benefit of introducing SaaS in the following proposition.

**PROPOSITION 6.** For low security-loss environments, introduction of a SaaS version will provide a limited increase in vendor profits and social welfare. Both relative measures of improvement are increasing in the quality of the SaaS version and the likelihood of undirected attacks. Technically, there exists ῶ, η > 0 such that for all α < ῶ,

(Π* – ΠBM) / ΠBM < ηα³
and
(W* - WBM) / WBM < ηα³

are satisfied.

Although Proposition 5 demonstrates that a vendor should optimally release both on-premises and SaaS versions of its product in low security-risk environments, Proposition 6 suggests that the benefits stemming from diversification are much more limited in these environments. In contrast to Proposition 3, by comparing (21) and (24), the percentage increase in profits associated with releasing the SaaS alternative is an order of magnitude smaller. In this sense, security concerns alone may not justify the additional costs of managing two separate versions of the software.

The findings in Propositions 3 and 6 are illustrated in Figure 2. We depict three curves plotting the measure (Π* – ΠBM)/ΠBM computed numerically under parameter sets A: cp = 0.30, πu = 0.23, B: cp = 0.50, πu = 0.23, and C: cp = 0.30, πu = 0.55, respectively. As can be seen, near α = 30, the percentage improvement in profits ranges from approximately 10%-30% under these parameter sets; however, near α = 1/30, the percentage improvement is negligible. This is the essence of the two propositions, i.e., diversification of security risk by offering SaaS has much greater potential for moderate to high security-loss environments. Comparing curve B to A, one can see that an increase in patching costs from cp =0.30 to cp = 0.50 can change the potential profit improvement of a SaaS release strategy substantially because of the poor patching behavior induced on the network at this higher cost level.²⁰ This characteristic is consistent with the results presented in Proposition 3, in particular from (21). Similarly, for lower α, Proposition 6 and specifically (24) suggest that an increase in the likelihood of an undirected attack (πu) will also increase the potential benefit of a diversification strategy. In Figure 2, we can see this effect by comparing curve C to A within the lower range of α.

Next, we examine security losses and consumer surplus. In low security-loss environments, the effect of versioning on these two measures differs considerably from what we established for high security-loss environments.

**PROPOSITION 7.** When a SaaS version is introduced in low security-loss environments, the average security losses per user decrease and consumer surplus increases in equilibrium.

For high security-loss environments, in Proposition 4, we established that when patching costs are low, the average security losses per user actually increase when the vendor versions by introducing a SaaS solution. When potential security losses become limited, Proposition 7 formally establishes that a similar type of outcome cannot happen; that is, by offering a SaaS version in addition to an on-premises version, the vendor can effectively diversify the undirected risk under the benchmark case into two smaller risks of the undirected and directed variety, which reduces the average security losses. Because the potential security losses are inherently limited, the negative impact of a reduction in the patching population is smaller than the positive diversification effect. Moreover, the introduction of SaaS benefits consumers in terms of security risk considerations and differentiated pricing.

## 7. Extension: Security Investment

In this section, we study a setting where the software vendor can invest to increase the security of its SaaS and on-premises offerings. We assume the firm can invest effort levels eu, ed ∈ [0, 1) to reduce the security risks associated with the on-premises and SaaS versions, respectively. An effort investment of eu yields a risk reduction from πu to (1 − eu)πu. Similarly, ed being exerted reduces πd to (1 − ed)πd. Because eu reduces the likelihood of a vulnerability in the on-premises product, it also reduces the expected patching cost from an initial value of cp to (1 – eu)cp. The respective costs associated with effort investments to improve security are denoted as Cu(eu) and Cd(ed), where both cost functions are twice-differentiable, convex, increasing, and satisfy Cu(0) = Cd(0) = C(0) = Cu(0) = 0. For technical reasons, we assume there exists a constant T > 0 such that C″(·), C″(·) > T.

As we have seen thus far, versioning is an effective way to achieve risk diversification. Hence, pricing SaaS and on-premises versions can also be used as a tool by the software vendor to influence consumption decisions toward profitable consumer market structures. In this extension, we aim to understand how the vendor's additional ability to invest in the security of both products influences outcomes. In particular, we examine the interaction between the vendor's versioning decision and security investments. In the following proposition, we first explore how the vendor's security investments differ across high and low security-loss environments.

**PROPOSITION 8.** In low security-loss environments, the firm increases its security-improving investments for both on-premises and SaaS versions as risk increases in the market, i.e., e(α) and e(α) are increasing in α. However, in high security-loss environments, if the likelihood of an undirected attack relative to a directed attack, patching costs, and SaaS quality are all sufficiently high, the vendor increases security-improving efforts for the on-premises version and decreases efforts for the SaaS version as risk increases in the market. Technically, there exists î > 0 such that if πu/πd > î, cp > 1/2, τ > 1/2, and δ > δ = 2(1 - cp)/(1+cp-2c) are satisfied, then eu(α) increases in α whereas ed(α) decreases in α.

Figure 3 illustrates the results in Proposition 8 and the underlying intuition. In low security-loss environments, consumers tend to prefer a limited, undirected security risk rather than incurring the costs of patching. For this reason, the vendor does not need to increase security investment in the on-premises product with a goal of reducing the expected patching costs. However, it may invest effort in the on-premises product to slightly reduce the risk consumers face in equilibrium. Its incentives to invest in SaaS security are similar. Both equilibrium effort levels are illustrated in panel (b) of Figure 3 in the area labeled A. As α increases, the vendor increases both of its investment levels to throttle equilibrium risk; this can increase quickly because no one patches in equilibrium as illustrated in panel (a) of Figure 3 in area A.

In high security-loss environments, the vendor's investment behavior differs substantially from that described above. Remarkably, its security investments in on-premises and SaaS versions diverge. Under potentially high security losses, consumers have much stronger incentives to patch and protect themselves if using the on-premises product. In fact, the vendor also wants to reduce the expected patching costs by increasing its effort to improve on-premises security. As we saw earlier in Proposition 1, under high patching costs and high SaaS quality, the vendor pursues a strategy wherein SaaS is targeted to the middle tier of the consumer market. An essential element of this strategy is that the vendor must limit equilibrium directed security risk such that the SaaS version is consumed by this middle tier segment. The vendor can accomplish this in two ways, i.e., investing in security of the SaaS product directly, or limiting the SaaS population to indirectly achieve greater security. As α increases, because of its strong incentives to invest in the on-premises product to reduce patching costs, high tier consumers shift toward patched, on-premises use away from SaaS. Because the SaaS population becomes more limited and achieves greater security as a result, the vendor can decrease its investment in SaaS product security to reduce costs. Its investment behavior is illustrated in area B of panel (b). Area B of panel (a) shows how the patching population increases while the SaaS population shrinks. The following result is connected to this discussion.

**PROPOSITION 9.** In high security-loss environments, when baseline consumer patching costs and SaaS quality are high, and the firm's security-improving costs are sufficiently convex, the vendor invests greater effort in addressing on-premises product security than SaaS, i.e., eu is greater than ed, while also targeting SaaS to the middle tier of the consumer market in equilibrium.

Proposition 9 formalizes our finding that the software vendor may continue to target its lower inherent quality SaaS product to the middle tier even when it can invest to improve security instead. Significantly, its behavior in this case hinges on the convexity of its investment costs not being too low. In the alternative case, the vendor would have incentives to make its on-premises product extremely secure, leading to a strategy wherein SaaS is geared to the lower tier of the market.

## 8. Concluding Remarks

In this paper, we explore how a vendor's offering of on-premises and SaaS versions of application software affects users' consumption incentives. In particular, we analytically demonstrate how users segment across products to manage the endogenously determined security externalities associated with unpatched on-premises behavior (undirected risk) and SaaS use (directed risk). Using our characterization of equilibrium consumer behavior, we rigorously study the software vendor's versioning problem and reveal several interesting insights. First, the vendor is sometimes incentivized to market its lower inherent quality SaaS version to a higher valuation consumer segment than the segment to which it targets its higher inherent quality on-premises version. In this case, the vendor strategically sets a high SaaS price to reduce its use and the associated level of directed security risk such that it offers a more secure product, albeit with fewer features, to a more quality-sensitive consumer segment. Panel (a) of Table 1 illustrates that this result is obtained in high security-loss environments when patching costs are high and the inherent quality of the SaaS version is not too low, i.e., ΠM > ΠL in the cell corresponding to High cp/High δ. We also analytically establish that when patching costs are within an intermediate range and the inherent quality of the SaaS version is still reasonably close to its on-premises counterpart, the vendor will prefer to target its SaaS product to the low tier when it is advantageous to social welfare if it would instead target it to the middle tier; additional vendor incentives can lead to welfare-superior outcomes in this region. This result can be seen in the cell in panel (a) of Table 1 corresponding to Medium cp/High δ.

In the versioning literature, for uniformly distributed consumer types and zero marginal costs, the standard result is that a software vendor will find it optimal to offer only its higher quality product to consumers. In our study, we formally demonstrate that because of risk diversification benefits, the vendor will always offer both versions of its product as long as the risks associated with each version are idiosyncratic. Interestingly, this versioning result holds even as the security risk becomes negligible. In panel (a) of Table 1, we indicate that for low security-loss environments, the software vendor always gears its SaaS version to the lower tier of the market, pricing its higher quality on-premises version to serve the higher tier. Because a patching population does not exist in equilibrium, we use IH and WH to refer to measures of profit and welfare if SaaS were targeted to the higher tier instead, which is shown to be a dominated strategy.

We compare economic measures (profitability, social welfare, security losses, and consumer surplus) under a versioning strategy against analogous measures in a benchmark case where the on-premises version is solely offered to consumers. We demonstrate that the potential improvement in profits and social welfare associated with a SaaS release and its corresponding security risk diversification are substantial in high security-loss environments, but more limited in the low security-loss environment. In spirit, introduction of a SaaS version with a different exposure to directed and undirected attacks than the on-premises version can help reduce the overall security risk to the network because of these diversification benefits. As can be seen in panel (b) of Table 1, for low security-loss environments and for high security-loss environments when patching costs are high, average per-user security losses indeed decline as a result of versioning. However, our study also highlights that because of opportunistic pricing by the vendor, the security risk diversification benefits are sometimes outweighed by market expansion, leading to higher average per-user security losses. This result can be seen in the cell corresponding to Low cp/High δ. In this case, introduction of a SaaS version can even lead to depressed consumer surplus as indicated in Table 1. For high security-loss environments, when the inherent quality of the SaaS offering and patching costs are low, with SaaS versioning average per-user security losses can go in either direction as is established in Proposition 4.

In recent years, companies have invested millions to provide SaaS versions of on-premises application software. Our study focuses on the security benefits of SaaS offerings in terms of risk-mitigated versioning. Given our research goals, we abstract from modeling concerns that are outside of our paper's scope. For example, to implement SaaS alternatives in addition to their traditional on-premises offerings, software vendors would necessarily need to incur additional costs in practice. These costs would have a fairly large fixed-variable cost ratio. One potential future research trajectory is to develop a better understanding of why we observe the existence of vendors who do not offer both SaaS and on-premises versions (e.g., Salesforce.com). By understanding the vendor's incentives outside of security concerns that underlie this type of behavior, we could also explore what leads to outcomes in a single market where competing firms each offer one version, SaaS or on-premises, and choose to differentiate themselves by specializing.

The benefits of cloud computing and, particularly, SaaS applications are driving businesses and governments to migrate many internally supported systems and software to the cloud. However, such a paradigm shift can have major consequences on security risks as consumers make choices on software deployment and protection. We hope that the model and insights presented in this paper provide a stepping stone toward a broader understanding of how security risk can be managed as cloud computing matures and becomes an integral part of IT strategies.

## Supplemental Material

Supplemental material to this paper is available at http://dx.doi.org/10.1287/isre.2014.0527.

## Acknowledgments

The authors thank Rahul Telang (the senior editor), the associate editor, and the anonymous reviewers for their helpful suggestions throughout the review process. The authors also thank Sridhar Narasimhan, D. J. Wu, Subodha Kumar, Ali Tafti, Ramnath Chellappa, the participants at the Conference on Information Systems and Technology 2012, INFORMS 2012 Annual Meeting, the Workshop on the Economics of Information Security 2013, as well as the participants in the research seminar at the University of California, Irvine for their helpful comments and discussions. This material is based on work partially supported by the National Science Foundation [Grant CNS-0954234].

## References

Anderson R (2001) Why information security is hard—An economic perspective. Proc. 17th Annual Comput. Security Appl. Conf. (IEEE Computer Soc., Washington, DC), 358–365.
Anderson R, Moore T (2006) The economics of information security. Science 314(5799):610-613.
Arora A, Telang R, Xu H (2008) Optimal policy for software vulnerability disclosure. Management Sci. 54(4):642-656.
August T, Tunca TI (2006) Network software security and user incentives. Management Sci. 52(11):1703-1720.
August T, Tunca TI (2008) Let the pirates patch? An economic analysis of software security patch restrictions. Inform. Systems Res. 19(1):48-70.
August T, Tunca TI (2011) Who should be responsible for software security? A comparative analysis of liability policies in network environments. Management Sci. 57(5):934–959.
Bain C, Faatz DB, Fayad A, Williams D (2002) Diversity as a defense strategy in information systems. Does evidence from previous events support such an approach? Proc. IFIP TC11/WG11.5 Fourth Working Conf. Integrity, Internal Control Security Inform. Systems: Connecting Governance Tech. (Kluwer, B.V., Deventer, The Netherlands), 77-94.
Beil D, Wan Z (2009) RFQ auctions with supplier qualification screening. Oper. Res. 57(4):934–949.
Bhargava HK, Choudhary V (2001) Information goods and vertical differentiation. J. Management Inform. Systems 18(2):89–106.
Bhargava HK, Choudhary V (2008) Research note: When is versioning optimal for information goods? Management Sci. 54(5):1029–1035.
Biddick M (2010) Why you need a SaaS strategy. InformationWeek (January). http://www.informationweek.com/cloud/software-as-a-service/why-you-need-a-saas-strategy/d/d-id/1086146?
Bloor B (2003) The patch problem: It's costing your business real dollars. White paper, Baroudi Bloor, Arlington, MA. http://www.netsense.info/downloads/PatchProblemReport_BaroudiBloor.pdf.
Boulton C (2013) American airlines outage likely caused by software quality issues. Wall Street Journal (April). http://blogs.wsj.com/cio/2013/04/17/american-airlines-outage-likely-caused-by-software-quality-issues/.
Branscombe M (2012) Salesforce talks security: From passwords to animatronic ponies. ZDNet (September). http://www.zdnet.com/salesforce-talks-security-from-passwords-to-animatronic-ponies-7000004454/.
Cavusoglu H, Cavusoglu H, Raghunathan S (2007) Efficiency of vulnerability disclosure mechanisms to disseminate vulnerability knowledge. IEEE Trans. Software Engrg. 33(3):171-185.
Cavusoglu H, Cavusoglu H, Zhang J (2008) Security patch management: Share the burden or share the damage? Management Sci. 54(4):657-670.
Charney S (2012) Trustworthy computing next. White paper, Microsoft. http://www.microsoft.com/en-us/download/confirmation.aspx?id=29084.
Chellappa RK, Jia J (2011) Competition and versioning. Working paper, Emory University and Hong Kong University of Science and Technology.
Chellappa RK, Mehra A (2013) Versioning 2.0: A product line and pricing model for information goods under usage constraints and with R&D costs. Working paper, Emory University and Indian School of Business.
Chen P-Y, Kataria G, Krishnan R (2011) Correlated failures, diversification, and information security risk management. MIS Quart. 35(2):397-422.
Choi JP, Fershtman C, Gandal N (2010) Network security: Vulnerabilities and disclosure policy. J. Indust. Econom. 58(4):868-894.
Choudhary V (2007) Comparison of software quality under perpetual licensing and software as a service. J. Management Inform. Systems 24(2):141-165.
Chow R, Golle P, Jakobsson M, Shi E, Staddon J, Masuoka R, Molina J (2009) Controlling data in the cloud: Outsourcing computation without outsourcing control. Proc. 2009 ACM Workshop Cloud Comput. Security, CCSW'09 (ACM, New York), 85-90.
Claburn T (2009) Government embraces cloud computing, launches app store. InformationWeek (September). http://www.informationweek.com/cloud/government-embraces-cloud-computing-launches-app-store/d/d-id/1083137?
Cox B, Evans D, Filipi A, Rowanhill J, Hu W, Davidson J, Knight J, Nguyen-Tuong A, Hiser J (2006) N-variant systems: A secret-less framework for security through diversity. Proc. 15th Conf. USENIX Security Sympos., USENIX-SS'06, Vol. 15 (USENIX Association, Berkeley, CA).
Dey D, Lahiri A, Zhang G (2012) Hacker behavior, network effects, and the security software market. J. Management Inform. Systems 29(2):77-108.
El Akkad O (2011) Microsoft wants you to rent an Office in the cloud. Globe and Mail (June). http://www.theglobeandmail.com/technology/tech-news/microsoft-wants-you-to-rent-an-office-in-the-cloud/article584830.
Farber D (2007) SAP's challenge to NetSuite, Workday and salesforce.com. ZDNet (September). http://www.zdnet.com/blog/btl/saps-challenge-to-netsuite-workday-and-salesforce-com/6327.
Forrest S, Somayaji A, Ackley D (1997) Building diverse computer systems. Proc. 6th Workshop Hot Topics Operating Systems (HotOS-VI), HOTOS'97 (IEEE Computer Soc., Washington, DC), 67–72.
Gherbi A, Charpentier R, Couture M (2011) Software diversity for future systems security. CrossTalk 25(5):10-13.
Gordon LA, Loeb MP (2002) The economics of information security investment. ACM Trans. Inform. Syst. Secur. 5(November):438-457.
Greenemeier L, Hoover JN (2007) How does the hacker economy work? InformationWeek (February). http://www.informationweek.com/how-does-the-hacker-economy-work/d/d-id/1051843?
Grossklags J, Christin N, Chuang J (2008) Secure or insure?: A game-theoretic analysis of information security games. Proc. 17th Internat. Conf. World Wide Web, WWW'08 (ACM, New York), 209-218.
Heal G, Kunreuther H (2007) Modeling interdependent risks. Risk Anal. 27(3):621-634.
Huang K-W, Sundararajan A (2005) Pricing models for on-demand computing. Working paper, National University of Singapore and New York University. http://papers.ssrn.com/sol3/papers.cfm?abstract_id=1281329.
Hui KL, Hui W, Yue T (2013) Information security outsourcing with system interdependency and mandatory security requirement. J. Management Inform. Systems 29(3):117-156.
IBM (2008) IBM Internet security systems X-Force 2008 mid-year trend statistics. IBM Global Tech. Services. https://www-935.ibm.com/services/us/iss/xforce/midyearreport/xforce-midyear-report-2008.pdf.
Jing B (2007) Network externalities and market segmentation in a monopoly. Econom. Lett. 95(1):7-13.
Johnson JP, Myatt DP (2003) Multiproduct quality competition: Fighting brands and product line pruning. Amer. Econom. Rev. 93(3):748-774.
Johnson ME (2008) Managing Information Risk and the Economics of Security, 1st ed. (Springer, New York).
Jones R, Mendelson H (2011) Information goods vs. industrial goods: Cost structure and competition. Management Sci. 57(1):164-176.
Judge P (2002) Microsoft security push cost $100 m for .Net server alone. ZDNet (July). http://www.zdnet.com/microsoft-security-push-cost-100m-for-net-server-alone-3002118314/.
Kannan K, Telang R (2005) Market for software vulnerabilities? Think again. Management Sci. 51(5):726-740.
Kannan K, Rahman MS, Tawarmalani M (2013) Economic and policy implications of restricted patch distribution. Working paper, Purdue University and University of Calgary.
Kash W (2013) Software patches eat government IT's lunch. InformationWeek (September). http://www.darkreading.com/risk-management/software-patches-eat-government-its-lunch/d/d-id/1111379.
Keizer G (2004) Sasser worm impacted businesses around the world. Network Comput. (May). http://www.networkcomputing.com/careers-and-certifications/sasser-worm-impacted-businesses-around-the-world/d/d-id/1208406?
Keizer G (2008) Windows users indifferent to Microsoft patch alarm, says researcher. Computerworld (December). http://www.computerworld.com/s/article/9122599/Windows_users_indifferent_to_Microsoft_patch_alarm_says_researchers.
Kim BC, Chen P-Y, Mukhopadhyay T (2010) An economic analysis of the software market with a risk-sharing contract. Internat. J. Electronic Commerce 14(2):7-39.
Kim BC, Chen P-Y, Mukhopadhyay T (2011) The effect of liability and patch release on software security: The monopoly case. Production Oper. Management 20(4):603-617.
Kundra V (2011) Tight budget? Look to the "cloud." New York Times (August). http://www.nytimes.com/2011/08/31/opinion/tight-budget-look-to-the-cloud.html?_r=0.
Kunreuther H, Heal G (2003) Interdependent security. J. Risk Uncertainty 26(2-3):231-249.
Laffont J-J, Tirole J (1988) The dynamics of incentive contracts. Econometrica 56(5):1153-1175.
Lahiri A (2012) Revisiting the incentive to tolerate illegal distribution of software products. Decision Support Systems 53(2):357-367.
Lala JH, Schneider FB (2009) IT monoculture security risks and defenses. IEEE Security Privacy 7(1):12-13.
Lee CH, Geng X, Raghunathan S (2013) Contracting information security in the presence of double moral hazard. Inform. Systems Res. 24(2):295-311.
Lee M (2014) Microsoft closes Office 365 admin access vulnerability. ZDNet (January). http://www.zdnet.com/microsoft-closes-office-365-admin-access-vulnerability-7000025369/.
Lemos R (2003) Slammer report: More headaches. ZDNet (February). http://www.zdnet.com/news/slammer-report-more-headaches/127449.
Lemos R (2004) MSBlast epidemic far larger than believed. CNET News.com (April). http://news.cnet.com/MSBlast-epidemic-far-larger-than-believed/2100-7349_3-5184439.html.
Lewis JA, Baker S (2013) The economic impact of cybercrime and cyber espionage. Report, Center for Strategic and International Studies, Washington, DC.
Li L, McKelvey RD, Page T (1987) Optimal research for Cournot oligopolists. J. Econom. Theory 42(1):140-166.
Liran N (2013) Severe Office 365 token disclosure vulnerability—Research and analysis. Adallom. https://www.adallom.com/blog/severe-office-365-token-disclosure-vulnerability-research-and-analysis/.
Ma D, Seidmann A (2014) Analyzing software-as-a-service with per-transaction charges. Working paper, Singapore Management University and University of Rochester.
MacLeod WB, Malcomson JM (1993) Investments, holdup, and the form of market contracts. Amer. Econom. Rev. 83(4):811-837.
Markoff J (2009) Defying experts, rogue computer code still lurks. New York Times (August). http://www.nytimes.com/2009/08/27/technology/27compute.html.
McBride S (2005) Zero day attack imminent. Computerworld (February). http://www.computerworld.com.au/article/1535/zero_day_attack_imminent/.
Mell P, Grance T (2011) The NIST definition of cloud computing. Computer Security Division, Information Technology Laboratory, National Institute of Standards and Technology, U.S. Department of Commerce. http://csrc.nist.gov/publications/nistpubs/800-145/SP800-145.pdf.
Messmer E (2013) Identity-theft vulnerability fixed in Microsoft Office 365, says security firm. NetworkWorld (December). http://www.networkworld.com/article/2172555/network-security/identity-theft-vulnerability-fixed-in-microsoft-office-365-says-security-firm.html.
Microsoft (2013) Security in Office 365. White paper, http://www.microsoft.com/en-us/download/details.aspx?id=26552.
Moore D, Shannon C, Brown J (2002) Code-Red: A case study on the spread and victims of an Internet worm. Proc. Second ACM SIGCOMM Internet Measurement Workshop, Marseille, France, 273-284.
Muller HM (2000) Asymptotic efficiency in dynamic principal-agent problems. J. Econom. Theory 91(2):292-301.
Neti S, Somayaji A, Locasto ME (2012) Software diversity: Security, entropy and game theory. Proc. 7th USENIX Conf. Hot Topics Security, HotSec'12 (USENIX Association, Bellevue, WA), 5.
Niculescu MF, Wu DJ (2014) Economics of free under perpetual licensing: Implications for the software industry. Inform. Systems Res. 25(1):173-199.
Nochenson A, Grossklags J, Heimann CFL (2014) How loss profiles reveal behavioral biases in interdependent security decisions. Internat. J. Internet Tech. Secured Trans. Forthcoming.
O'Neill S (2011) Survey: Value of the cloud, telecommuting overstated. CIO (September). http://www.cio.com/article/2404707/cloud-computing/survey-value-of-the-cloud-telecommuting-overstated.html.
Pesendorfer W, Swinkels JM (2000) Efficiency and information aggregation in auctions. Amer. Econom. Rev. 90(3):499-525.
Png IPL, Wang Q-H (2009) Information security: Facilitating user precautions vis-à-vis enforcement against attackers. J. Management Inform. Systems 26(2):97–121.
Ransbotham S, Mitra S, Ramsey J (2012) Are markets for vulnerabilities effective? MIS Quart. 36(1):43-64.
Robertson J (2014) Heartbleed fixes taking longer as websites plug gaps. Bloomberg.com (April). http://www.bloomberg.com/news/2014-04-14/heartbleed-fixes-taking-longer-as-websites-plug-gaps.html.
Roy D (2011) Data on sale. CIO.in 6(10):60–61.
Schneider FB, Birman KP (2009) The monoculture risk put into context. IEEE Security Privacy 7(1):14-17.
Vereshchagina G, Hopenhayn HA (2009) Risk taking by entrepreneurs. Amer. Econom. Rev. 99(5):1808-1830.
Villeneuve N (2011) Trends in targeted attacks. White paper. Trend Micro (October). http://www.trendmicro.com/cloud-content/us/pdfs/security-intelligence/white-papers/wp_trends-in-targeted-attacks.pdf.
Weatherwax E, Knight J, Nguyen-Tuong A (2009) A model of secretless security in N-variant systems. Proc. 39th Annual IEEE/IFIP Internat. Conf. Dependable Systems Networks, DSN'09 (IEEE Computer Soc., Washington, DC).
Wei X, Nault BR (2011) Vertically differentiated information goods: Monopoly power through versioning. Working paper, Fudan University and University of Calgary.
Wei X, Nault BR (2014) Monopoly versioning of information goods when consumers have group tastes. Production Oper. Management. 23(6):1067-1081.
Xu J, Kalbarczyk Z, Iyer RK (2003) Transparent runtime randomization for security. Proc. 22nd Sympos. Reliable Distributed Systems (SRDS 2003), SRDS 03 (IEEE Computer Soc., Washington, DC), 260-269.
Zhang JJ, Seidmann A (2010) Perpetual versus subscription licensing under quality uncertainty and network externality effects. J. Management Inform. Systems 27(1):39–68.

## Appendix

### Online Supplement for ISR Manuscript
“Cloud Implications on Software Network Structure and Security Risks”

Terrence August, Marius Florin Niculescu, Hyoduk Shin

Proof of Lemma 1: We first provide the complete parameter regions and the corresponding consumer equilibrium outcome:

(I) Unpatched On-premises only (0 < vu < 1):
(A) δ ≤ 1 - cp
(i) p ≤ ps(1 – cp)/δ and α ≤αβ;
(ii) ps(1 − cp)/δ <p≤ps/δ and α ≤ αA;
(B) δ > 1 - cp
(i) p ≤ 1 - cp − δ + ps and α≤αβ;
(ii) 1 — cp — δ + ps <p<ps and α ≤ αC;
(iii) ps<p<ps/δ and α≤αA;

(II) SaaS only (0 < va < 1): p > 1 + ps − δ and α ≤ αD

(III) No Patching On-premises with Unpatched On-premises at the bottom (0 < vu < vd < 1):
(A) δ > 1 - cp
(a) ps≤1-cp
(i) 1 + ps – δ - cp < p≤ps and αC < α < â2;
(b) ps > 1 - cp
(i) 1 + ps – δ — cp < p < 1 - cp and αC < α < â2;
(ii) 1 - cp ≤ p≤ps and αC < α;

(IV) No Patching On-premises with Unpatched On-premises at the top (0 < vd < vu < 1):
(A) δ ≤ 1 - cp
(a) ps ≤ δcp/(1 – δ)
(i) ps(1 − cp)/δ < p≤ps/δ and αA < α < â;
(ii) ps/δ <p< 1 + ps − δ and α ≤ â;
(iii) 1 + ps – δ < p < 1 - cp and αP < α <â;
(iv) 1 - cp ≤ p and αP < α;
(b) δ – cp < ps ≤ δ(1 – cp)

(i) ps(1 − cp)/δ < p≤ps/δ and αA < α < â;
(ii) ps/δ <p<1 - cp and α ≤ â;
(iii) 1 - cp <p< 1 + ps − δ and all α;
(iv) 1 + ps – δ < p and αP < α;
(B) δ > 1 − cp
(a) ps ≤ δ – cp
(i) ps <p<ps/δ and αA < α≤â;
(ii) ps/δ <p< 1 + ps − δ and α ≤ â;
(iii) 1 + ps – δ < p < 1 - cp and αP < α <â;
(iv) 1 - cp < p and αP < α;
(b) δ - cp < ps ≤ δ(1 − cp)
(i) ps <p≤ps/δ and αA < α≤â;
(ii) ps/δ <p<1 - cp and α ≤ â;
(iii) 1 - cp <p< 1 + ps − δ and all α;
(iv) 1 + ps – δ < p and αP < α;
(c) δ(1 − cp) < ps≤1-cp
(i) ps <p<1- cp and αA < α≤â;
(ii) 1 - cp <p<ps/δ and αA <α;
(iii) ps/δ <p< 1 + ps − δ and all α;
(iv) 1 + ps – δ < p and αP < α;
(d) 1 - cp < ps
(i) ps <p≤ps/δ and αA < α;
(ii) ps/δ <p<1 + ps − δ and all α;
(iii) 1 + ps – δ < p and αP < α;

(V) No SaaS: 0 < vu < vp < 1
(A) δ ≤ 1 - cp
(a) ps ≤ δcp/(1 – δ)
(i) p≤ps/δ – cp and α > αβ;
(ii) ps/δ - cp <p<ps and αβ < α <αF;
(iii) ps <p≤ps(1 – cp)/δ and αβ < α <αE;
(b) ps > δcp/(1 – δ)

(i) p≤ps/δ – cp and α > αβ;
(ii) ps/δ – cp <p<ps(1 – cp)/δ and αβ < α <αE;
(B) δ > 1 - cp
(i) p≤ps/δ – cp and α > αβ;
(ii) ps/δ – cp <p<1+ps - δ - cp and αβ < α≤αF;

(VI) SaaS in the bottom tier: 0 < vd < vu < vp < 1
(A) δ ≤ 1 - cp
(a) ps ≤ δcp/(1 – δ)
(i) ps <p≤ps(1 − cp)/δ and αE;
(ii) ps(1 − cp)/δ < p < 1 − cp and α > â1;
(b) ps > δcp/(1 – δ)
(i) ps/δ - cp <p<ps(1 − cp)/δ and αE;
(ii) ps(1 – cp)/δ < p < 1 − cp and α > â1;
(B) δ > 1 - cp
(a) ps≤1-cp
(i) ps <p<1- cp and α > â1;

(VII) SaaS in the middle tier: 0 < vu < vd < vp < 1
(A) δ ≤ 1 - cp
(a) ps ≤ δcp/(1 – δ)
(i) ps/δ - cp <p<ps and α > αF;
(B) δ > 1 - cp
(a) ps≤1-cp
(i) ps/δ - cp <p<1 + ps - δ - cp and α > αF;
(ii) 1 + ps – δ - cp < p≤ps and α > â2;
(b) ps > 1 - cp
(i) ps/δ - cp < p < 1 + ps - δ – cp and α > αF;
(ii) 1 + ps – δ - cp < p < 1 - cp and α > â2.

First, we establish the general threshold-type equilibrium structure. Given the size of unpatched user population of the on-premises version u and the size of user population of the SaaS version d, the net payoff of the consumer with type v for different strategy profiles σ is written as

R(v, σ) =
  v - p - cp if σ(v) = (OP, P) ;
  v - p - πu uαv if σ(v) = (OP, NP) ;
  δv - ps - πd dαδv if σ(v) = (SaaS, ND) ;
  0 if σ(v) = (N, ND) .

First, σ(v) = (OP, P), if and only if

v - p - cp ≥ v - p - πu uαv ⇔ v ≥ p + cp / (1 - πu uα) , and
v - p - cp ≥ δv - ps - πd dαδv ⇔ v ≥ p + cp - ps / (1 - δ(1 - πd dα)) , and
v - p - cp ≥ 0 ⇔ v ≥ p + cp ,

which can be summarized as

v ≥ max ( p + cp / (1 - πu uα) , p + cp - ps / (1 - δ(1 - πd dα)) , p + cp ).

By (A.2), in equilibrium, if a consumer with valuation v0 buys and patches the on-premises alternative, then every consumer with valuation v > v0 will also do so. Hence, there exists a threshold vp ∈ (0,1] such that for all v∈V, σ*(v) = (OP, P) if and only if v ≥ vp. Similarly, σ(v) ∈ {(OP, P), (OP, NP), (SaaS, ND)}, i.e., the consumer purchases one of the alternatives, if and only if

v - p - πu uαv ≥ 0 ⇔ v ≥ p / (1 - πu uα) , or
δv - ps - πd dαδv ≥ 0 ⇔ v ≥ ps / (δ(1 - πd dα)) , or

which can be rewritten as

v ≥ min ( p / (1 - πu uα) , ps / (δ(1 - πd dα)) ).

Let 0 < vu < 1 and σ*(vu) ∈ {(OP, P), (OP, NP), (SaaS, ND)}, then by (A.3), for all v > vu, σ*(v) ∈ {(OP, P), (OP, NP), (SaaS, ND)}, and hence there exists a vu ∈ (0, 1], such that a consumer with valuation v∈V will purchase if and only if v ≥ vu.

By (A.2) and (A.3), vu ≤ vp holds. Moreover, consumers with types in [vu, vp] choose either (OP, NP) or (SaaS, ND). A purchasing consumer with valuation v will prefer (OP, NP) over (SaaS, ND) if and only if

v - p - πu uαv > δv - ps - πd dαδv ⇔ v[(1 – πu uα) – δ(1 – πd dα)] > p - ps.

This inequality can be either v > (p - ps)/((1 – πu uα) – δ(1 – πd dα)) or v < (p - ps)/((1 – πu uα) – δ(1 – πd dα)), depending on the sign of (1 – πu uα) – δ(1 – πd dα). Consequently, there can be two cases for (OP, NP) and (SaaS, ND) in equilibrium: first, there exists vu ∈ [vu, vp] such that σ(v) = (OP, NP) for all v ∈ [vu, vp), and σ(v) = (SaaS, ND) for all v ∈ [vd, vu) where vd = vu. Second, there exists vd ∈ [vu, vp] such that σ(v) = (SaaS, ND) for all v ∈ [vd, vp), and σ(v) = (OP, NP) for all v ∈ [vu, vd) where vu = vd. If (1 – πu uα) – δ(1 − πd dα) = 0, then depending on the sign of p – ps, all consumers unilaterally prefer either (OP, NP) or (SaaS, ND); e.g., if p > ps, all consumers prefer (SaaS, ND), and if p < ps, then all consumers prefer (OP, NP). Finally, if p = ps, all consumers are indifferent between (OP, NP) and (SaaS, ND), in which case only the sizes of consumer population u and d matter in equilibrium, i.e., (1 – πu uα) – δ(1 − πd dα) = 0 in equilibrium. Technically, there are multiple equilibria in this case; however, utility of each consumer and the vendor's profit are the same in all equilibria. So, without loss of generality, we focus on the threshold-type equilibrium in this case. We also provide detail discussion for this case when we investigate case (VII) below. In summary, we have established the threshold-type equilibrium structure in (6) and (7).

Next, we characterize in more detail case (VII) in which SaaS arises in the middle tier in equilibrium, i.e., 0 < vu < vd < vp < 1, as well as the corresponding parameter regions. Based on this threshold structure, it follows that d = vp - vd and u = vd - vu. In this case, we prove the following claim first:

Claim: The equilibrium that corresponds to case (VII) arises if and only if the following conditions are satisfied:

p < ps < p + cp <1 and ps < δ(p + cp) and
{ (p ≤ 1 - cp - (δ – ps) and α > αF) or (p > 1 - cp - (δ – ps) and α > â2) }.

Proof: First, we prove that there exists the unique positive â2 that satisfies g2(α) = 0, where function g2 was defined in (14). Taking the derivative of g2 with respect to α, we obtain

dg2(α) / dα = 2δπd(ps – p) / (Φ – αδπd)² + Φπu / (δπd) * (1 + (1 - 2p - απu) / (4ραπu + (1 - απu + πd)²))

The first term in (A.6) is positive because p < ps and Φ > 0, i.e., p > 1 − cp — (δ — ps), in the relevant region of â2. Furthermore, we have

(δπd)² (4ραπu + (1 - απu + πd)²) - (Φπu + δπd(1 - 2p - απu))² = 4ρδπd ((1 – p)δπd + Φπu) > 0.

Hence, the second term in (A.6) is also positive because p < 1 - cp and Φ > 0. As a result, (A.6) is positive, i.e., g2 is increasing in α. In addition,

g2(0) = -2(p + cp - ps + δπd) < 0,
and
lim α→∞ g2(α) = 2(1 − p − cp) > 0,

under the parameter region of p + cp > ps and 1 − p > cp from (A.5). From (14) and (A.6) - (A.9), there exists a unique â2 > 0 that satisfies g2(â2) = 0.

Next, we investigate the characterization of the three thresholds, vp, vd and vu. The consumer with type vp is indifferent between (OP, P) and (SaaS, ND); hence, it satisfies

vp - p - cp = δvp - ps - πd(vp – vd)αδvp ↔ vp(1 − δ(1 − πd(vp – vd)α)) = p + cp - ps.

Similarly, the consumer with type vd is indifferent between (SaaS, ND) and (OP, NP):

δvd - ps - πd(vp - vd)αδvd = vd - p - πu(vd – vu)αvu ↔
vd(δ(1 – πd(vp – vd)α) – (1 – πu(vd - vu)α)) = ps - p.

Finally, the consumer with type vu is indifferent between (OP, NP) and (N, ND), which can be written as

vu - p - πu(vd – vu)αvu = 0 ↔ vu(1 – πu(vd – vu)α) = p .

Next, we prove that under the parameter conditions given in (A.5), there exist the unique set of solutions vu, vd, and vp with 0 < vu < vd < vp < 1 that satisfy (A.10), (A.11) and (A.12).
First, (A.10) can be rewritten as

f1(vp) = δπdαvp² + (1 − δ(1 + πdαvd))vp – (p + cp - ps) = 0.

Then, vd < vp < 1 becomes equivalent to f1(vd) < 0 and f1(1) > 0. The inequality f1(vd) < 0 can be simplified to

vd < p + cp - ps / (1 - δ)

For this inequality to hold, p + cp > ps should be satisfied, i.e., p + cp > ps is a necessary condition. In addition, (A.14) matters only when (p + cp – ps)/(1 − δ) ≤ 1, i.e., Φ≤0. Otherwise, i.e., if Φ > 0, then vd <1. Similarly, the inequality f1(1) > 0 is simplified to

vd < 1 + ps - (cp + p + δ – αδπd) / αδπd ,

and for this inequality to hold, α > Φ/(δπd). In addition, this condition matters only when Φ > 0. Otherwise, i.e., Φ ≤ 0, then vd <1. As a result, if Φ < 0, then (A.14) should hold; otherwise, (A.15) should be satisfied. Furthermore, solving f1(vp) = 0, we obtain

vp = ( (1 – δ – αδπd) + √(1 – δ – αδπd)² + 4αδπd(p + cp - ps) ) / (2αδπd)

Next, (A.12) can be rewritten as

f2(vu) = πuαvu² + (1 – πuαvd)vu – p = 0.

From this equation, it follows that f2(0) = -p < 0; consequently, 0 < vu < vd is equivalent to f2(vd) > 0, which is simplified to vd > p. Moreover, solving (A.17), we obtain

vu = ( (1 – πuαvd) + √(1 – πuαvd)² + 4pαπu ) / (2απu)

By plugging (A.16) and (A.18) into (A.11) and simplifying, (A.11) can be rewritten as f3(vd) = 0 where

f3(vd) = 2(p - ps) / vd + δ + αδπd + πuαvu / (1 - πuαvd) * ( (1 - πuαvd) + √(1 - πuαvd)² + 4pαπu ) / (2απu)

Furthermore, consumer types v ∈ (vd, vp) should prefer (SaaS, ND) over (OP, NP) in equilibrium, i.e.,

v(δ(1 – πdα(vp – vd)) – (1 – πuα(vd – vu))) > ps - p,

for v∈ (vd, vp). Then, from (A.11), it implies that both p < ps and δ(1 – πdα(vp – vd)) > 1-πuα(vd – vu) should be satisfied, which is equivalent to p < ps and vd ≥ 0. In addition, since we have vd > p from f2(vd) > 0, the condition vd ≥ 0 becomes redundant. By taking the derivative of f3 with respect to vd in (A.19), we obtain

d f3(vd) / dvd = -2(p - ps) / vd² + αδπd / (1 - πdα(vp – vd)) * ( (1 - πdα(vp – vd)) + √(1 - πdα(vp – vd))² + 4αδπd(p + cp - ps) ) / (2αδπd) + απu / (1 - πuαvd) * ( (1 - πuαvd) + √(1 - πuαvd)² + 4pαπu ) / (2απu)

for p < ps and p + cp > ps, both of which are satisfied from (A.5). Consequently, in this parameter region, f3(vd) is strictly increasing in vd. We now investigate the remaining conditions to guarantee (A.14), (A.15) and vd > p. We also have necessary conditions: p ≤ ps and p + cp > ps from above. In addition, for consumers who optimally choose (OP, P) to exist in equilibrium, 1 – p – cp > 0, i.e., p < 1 – cp, should be satisfied. From the monotonicity of f3(vd), it follows that (A.14), (A.15) and vd > p are satisfied, if and only if f3((p + cp – ps)/(1 − δ)) > 0, f3((αδπd – Φ)/(αδπd)) > 0 and f3(p) < 0 are satisfied. First, it follows that

f3(p) = 2(ps - p) / p * (1 – δ – αδπd) – √(1 – δ – αδπd)² + 4αδπd(p + cp - ps)
< 2(ps - p) / p * (1 – δ – αδπd) – |1 – δ – αδπd| ≤ 0,

where the first inequality follows from p + cp > ps and the second inequality follows from p ≤ ps and x + |x| ≥ 0.

Note that when p = ps, f3(vd) in (A.19) is equivalent to δ(1 − πdα(vp – vd)) – (1 – πuα(vd - vu)) = 0 in (A.11). Consequently, from (A.20), all consumers are indifferent between (SaaS, ND) and (OP, NP); in this case, in equilibrium, consumer types v ∈ [vp, 1] prefer (OP, P) and consumer types v ∈ [0, vu) prefer (N, ND). Moreover, consumer types v ∈ [vu, vp) choose (SaaS, ND) or (OP, NP) in equilibrium in such a way that the consumer population size with (SaaS, ND) is vp - vd and the population size with (OP, NP) equals vd - vu. Technically speaking, there exist multiple consumer equilibria in this case; however, we resolve this case so that it is consistent with our threshold-type equilibrium structure, i.e., consumer types v ∈ [vd, vp) choose (SaaS, ND), and consumer types v ∈ [vu, vd) choose (OP, NP). Each consumer's utility as well as the vendor's profit are the same in all equilibria in this case; without loss of generality, we focus on this threshold-type equilibrium structure.

Next, f3((αδπd – Φ)/(αδπd)) > 0 is relevant when Φ > 0 from above, and f3((αδπd – Φ)/(αδπd)) > 0 can be rewritten as g2(α) > 0, where g2(α) is in (14). From the definition of â2 and (14), and (A.6) - (A.9), f3((αδπd – Φ)/(αδπd)) > 0 holds, if and only if α > â2, under p + cp > ps, 1 − p > cp and Φ > 0. Moreover, â2 > Φ/(δπd) since g2(α) becomes negative as α approaches Φ/(δπd) from above and g2(α) is increasing in α. Finally, f3((p + cp - ps)/(1 − δ)) > 0 is simplified to

(p + cp - ps)απu / (1 - δ) > √(p + cp - ps)²απu² + (1 - δ)² / (1 - δ)

For this inequality to hold, the left-hand side should be positive, i.e.,

α > (1 – δ)(cp + ps – p – 2cpδ) / (p + cp - ps)²πu

Under this condition (A.24), by squaring (A.23) and simplifying, we have

α((cp + p)δ – ps) > cp(1 – δ)²(p - ps + cpδ) / (p + cp - ps)²πu

If (cp + p)δ – ps > 0, then it follows that

cp(1 – δ)²(p - ps + cpδ) / (p + cp - ps)²πu < (1 – δ)(cp + ps – p – 2cpδ) / (p + cp - ps)²πu

under the region of p < 1 - cp, ps < p + cp and p ≤ ps. However, if (cp + p)δ – ps ≤ 0, then the inequality in (A.26) holds in the opposite direction. Consequently, under the parameter region of p< 1 - cp, ps < p + cp and p < ps, f3((p + cp - ps)/(1 - δ)) > 0 is simplified to

(cp + p)δ – ps > 0 and α > αF = cp(1 – δ)²(p - ps + cpδ) / (p + cp - ps)²πu

In summary, there exist the unique solutions vu, vd, and vp with 0 < vu < vd < vp < 1 that satisfy (A.10), (A.11) and (A.12), if and only if the conditions (A.5) are satisfied.

To complete the proof of case (VII), note that ps/δ - cp < 1 - cp – (δ – ps) < 1 – cp holds since ps < δ. Second, if δ > 1 - cp, then 1 - cp – (δ – ps) < p < 1 - cp. In this case, if ps ≤ 1 – cp, then (A.5) becomes

{ (ps/δ - cp < p < 1 - cp – (δ – ps) and α > αF) or (1 - cp – (δ – ps) < p < 1 - cp and α > â2) }.

whereas if ps > 1 − cp, then (A.5) becomes

{ (ps/δ - cp < p < 1 - cp – (δ – ps) and α > αF) or (1 - cp – (δ – ps) < p < 1 - cp and α > â2) }.

Third, if δ < 1 – cp, then ps < 1 − cp – (δ – ps) < 1 - cp. For this region of ps/δ – cp < p < ps to be non-empty, ps ≤ δcp/(1 − δ). Thus, in this case, (A.5) becomes

(ps ≤ δcp / (1 - δ) and ps/δ - cp < p ≤ ps and α > αF).

Combining (A.28)–(A.30), we then obtain the presented conditions for case (VII).

Next, for case (VI), in which SaaS arises in the low tier in equilibrium, i.e., 0 < vd < vu < vp < 1, based on the threshold-type equilibrium structure, u = vp - vu and d = vu - vd. Following similar steps to the proof of case (VII), we prove the following claim first:

Claim: The equilibrium that corresponds to case (VI) arises if and only if the following conditions are satisfied:

ps < p < 1 - cp and α > â1 and
{ (ps/δ < p < ps/δ + cp / (1 - δ) and α > αE) or (ps/δ + cp / (1 - δ) < p < ps and α > αE) }.

Proof: First, we prove that there exists the unique root â1 greater than cp/πu that satisfies g1(α) = 0. Similar to the proof of case (VII), it follows that g1(α) is decreasing in α under the parameter region of ps < p < 1 - cp and ps/(p + cp) < δ. Furthermore, g1(α) becomes positive as α approaches cp/πu from above and g1(α) becomes negative as α becomes large enough, which proves that there exists a unique â1 greater than cp/πu that solves g1(α) = 0.
From the threshold-type equilibrium structure, in this case, we have u = vp - vu and d = vu - vd. Moreover, the thresholds, vp, vu and vd satisfy the following three equations:

πuα(vp – vu)vu = cp,
vu(1 – πuα(vp – vu)) – δ(1 – πdα(vu - vd)) = p - ps, and
δvdα(1 – πdα(vu - vd)) = ps .

Using (A.32) and vp < 1, we obtain

vu < 1 - cp / (πuα)
and
vp = ( vuαπu + √(vuαπu)² + 4cp ) / (2απu)

In addition, from (A.34) and vd < vu, it follows that

ps / δ < vu
and
vd = ( δ(1 – πdαvu) + √(δ(1 – πdαvu))² + 4psαδπd ) / (2αδπd)

From (A.35) and (A.36), we have

ps / δ < vu < 1 - cp / (πuα) ,

and for this region of vu to be non-empty, α > cpδ/(πu(δ – ps)). Furthermore, by substituting vp and vu in (A.35) and (A.36) respectively into (A.33) and simplifying, we obtain

f4(vu) = 2(p - ps) / vu + (2 − δ + αvu(πu + δπd)) / (1 - πuαvu) * ( (1 - πuαvu) + √(1 - πuαvu)² + 4pαπu ) / (2απu)

By taking derivative with respect to vu, it then follows that

d f4(vu) / dvu = -2(p - ps) / vu² + απu / (1 - πuαvu) * ( (1 - πuαvu) + √(1 - πuαvu)² + 4pαπu ) / (2απu) + δπdα / (1 - πdαvu) * ( (1 - πdαvu) + √(1 - πdαvu)² + 4psαδπd ) / (2αδπd)

which is negative, i.e., f4(vu) is decreasing in vu, when p≥ps. Consequently, (A.37) becomes equivalent to f4(ps/δ) > 0 and f4(1 − cp/(πuα)) < 0. In addition, for (A.37) to be non-empty, we need α > cpδ/(πu(δ – ps)). First, f4(ps/δ) > 0 is simplified to

(δ > ps / (p + cp) or (ps / (p + cp) < δ < ps / (p + cp) and α > αE) ).

Second, f4(1 - cp/(πuα)) < 0 is simplified to α > â1, which completes the proof.

Using (A.31) and noting that f4(cpδ/(πu(δ – ps))) < 0, i.e., cpδ/(πu(δ – ps)) > â1, if and only if p < ps(1 − cp)/δ, and that αE > cpδ/(πu(δ – ps)) if and only if p < ps(1 − cp)/δ, we then obtain the complete characterization of the corresponding regions for case (VI).

For case (V) in which there is no SaaS, i.e., 0 < vu < vp < 1, we prove the following claim related to the corresponding parameter regions in which case (V) arises in equilibrium:

Claim: The equilibrium that corresponds to case (V) arises if and only if the following conditions are satisfied:

p < 1 - cp and α > αβ
and
{ (ps / δ < ps / (p + cp) or (ps / (p + cp) < δ < ps / (p + cp) and α ≤ αE) ) and
( (ps / δ < ps / (p + cp) or (ps / (p + cp) < δ < ps / (p + cp) and α ≤ αF) ) }.

This condition is equivalent to f5(vu) ≤ 0, which is simplified to p < 1 - cp – (δ – ps) and α ≤ αF. As a result, there should be no SaaS segment in the middle-tier if and only if

{ (ps / δ < ps / (p + cp) or (ps / (p + cp) < δ < ps / (p + cp) and α ≤ αF) ) }.

which completes the proof.

Note that (A.41) can be rewritten as

p < 1 - cp and α > αβ and { (ps / δ < ps / (p + cp) or (ps / (p + cp) < δ < ps / (p + cp) and α ≤ αE) ) and
( (ps / δ < ps / (p + cp) or (ps / (p + cp) < δ < ps / (p + cp) and α ≤ αF) ) }.

using ps/δ - cp <1+ps − δ – cp from ps < δ. Moreover, it follows that αE <αF if and only if ps <p in this region. In addition, ps/δ – cp > ps if and only if ps > δcp > (1 – δ). Using these relationship and algebra, and simplifying (A.51), we complete the proof of case (V).

For case (IV) in which there does not exist patching for on-premise purchases and SaaS exists the low tier in equilibrium, i.e., 0<vd < vu <1, from the threshold-type equilibrium structure, it follows that u = 1 - vu and d = vu - vd. Similarly, in this case, we first prove the following claim:

Claim: The equilibrium that corresponds to case (IV) arises if and only if the following conditions are satisfied:

ps ≤ p and
{ (ps / δ < ps / (p + cp) or (ps / (p + cp) < δ < ps / (p + cp) and α > αA) ) and
( (ps ≤ 1 + ps – δ or (1 + ps – δ < p and α > αD) ) ) }.

Proof: First, the threshold types vu and vd satisfy the following two equations:

vdδ(1 – πdα(vu - vd)) = ps,
vu(1 – πuα(1 – vu)) – δ(1 – πdα(vu – vd)) = p - ps.

In this case, the consumers with types greater than vu prefer (OP, NP) over (SaaS, ND), i.e.,

v(1 – πuα(1 – vu)) – δ(1 – πdα(vu – vd)) ≥ p - ps,

for v ∈ (vu, 1]. Therefore, it follows that p > ps and 1 – πuα(1 – vu) – δ(1 – πdα(vu – vd)) ≥ 0. Using (A.53) and the condition vd < vu, we obtain

vu > ps / δ
and
vd = ( δ(1 – πdαvu) + √(δ(1 – πdαvu))² + 4psαδπd ) / (2αδπd)

Substituting vd from (A.56) into (A.54) and simplifying, we have

f6(vu) = 2(p - ps) / vu + δ(1 – πdαvu) + 2πuα(1 – vu) + √(δ(1 – πdαvu))² + 4psαδπd = 0.

By taking derivative with respect to vu, it follows that

d f6(vu) / dvu = -2(p - ps) / vu² + δπdα / (1 - πdαvu) * ( (1 - πdαvu) + √(1 - πdαvu)² + 4psαδπd ) / (2αδπd) + 2πuα / (1 - πuαvu) * ( (1 - πuαvu) + √(1 - πuαvu)² + 4pαπu ) / (2απu)

Thus, f6(vu) is decreasing in vu. Furthermore, from (A.56), we need vu > ps/δ and we also need vu < 1. Those two conditions are equivalent to f6(ps/δ) > 0 and f6(1) < 0. First, f6(ps/δ) > 0 is simplified to α > αA. Note that αA < 0 if and only if p < ps/δ, in which case all non-negative α values satisfy f6(ps/δ) > 0. Second, similarly, f6(1) < 0 is simplified to α > αP. Also, note that αP > 0 if and only if p > 1 + ps – δ. Otherwise, i.e., p < 1 + ps – δ, all non-negative α values satisfy f6(1) < 0. Finally, there should not be any customers who choose (OP, P); first, if p > 1 - cp, then nobody can afford to patch. Otherwise, i.e., if p < 1 – cp, then v = 1 customer should not prefer to patch instead of unpatched on-premise. This condition can be written as 1 - p - cp ≤ 1- πuα(1 – vu) – p, which is simplified to vu ≥ 1 - cp/(πuα). Using (A.57) and (A.58), it follows that vu ≥ 1 − cp/(πuα) is equivalent to α ≤ â1, which completes the proof.

Denote αN ≡ cp/(πu(1 − ps/δ)). Then, it follows that αA > αN if and only if p < ps(1 − cp)/δ. In addition, αN > â1 if and only if p < ps(1-cp)/δ. As a result, αA > â1 if and only if p < ps(1-cp)/δ. Using this relationship and comparing all p-bounds in (A.52) together with α-bounds, we then establish all conditions in case (IV).

For case (III) in which there does not exist patching for on-premise purchases and SaaS consumption is on the high tier in equilibrium, i.e., 0 < vu < vd < 1, from the threshold-type equilibrium structure, it follows that u = vu - vu and d = 1 - vd. Similar to case (IV), in this case, we first prove the following claim:

Claim: The equilibrium that corresponds to case (III) arises if and only if the following conditions are satisfied:

ps > p and { (p > 1 + ps – δ) or (p ≤ 1 + ps – δ and α > αC) } and
{ (p > 1 - cp) or (1 - cp – (δ – ps) < p < 1 - cp and α ≤ â2) }.

Proof: In this case, the threshold types vu and vd satisfy the following two equations:

vd(δ(1 – πdα(1 − vd)) – (1 – πuα(vd - vu))) = ps - p,
vu(1 – πuα(vd – vu)) = p .

First, the consumers with types greater than vd prefer (SaaS, ND) over (OP, NP), i.e.,

v(δ(1 – πdα(1 − vd)) – (1 – πuα(vd – vu))) ≥ ps-p,

for v ∈ (vd, 1]. Therefore, it follows that ps > p and δ(1 – πdα(1 − vd)) – (1 – πuα(vd – vu)) > 0. The second condition is equivalent to vd > 0. By (A.61) and the condition vu < vd, it follows that

vd > p
and
vu = ( (1 – πuαvd) + √(1 – πuαvd)² + 4pαπu ) / (2απu)

Substituting vu from (A.63) into (A.60) and simplifying, we obtain

f7(vd) = 2(ps - p) / vd + 1 − 2δ + 2αδπd(1 – vd) + απu / (1 - πuαvd) * ( (1 - πuαvd) + √(1 - πuαvd)² + 4pαπu ) / (2απu) = 0.

Similar to case (IV), by taking derivative with respect to vd, we have

d f7(vd) / dvd = -2(ps - p) / vd² + 2αδπd / (1 - πdαvd) * ( (1 - πdαvd) + √(1 - πdαvd)² + 4psαδπd ) / (2αδπd) + απu / (1 - πuαvd) * ( (1 - πuαvd) + √(1 - πuαvd)² + 4pαπu ) / (2απu)

Thus, f7(vd) is decreasing in vd. In addition, from (A.63), we need vd > p and we also need vd < 1. Those two conditions are equivalent to f7(p) > 0 and f7(1) < 0. First, f7(p) > 0 holds always since ps > p. Second, f7(1) < 0 is simplified to α > αC. Also, note that αC ≥ 0 if and only if p ≤ 1 + ps – δ. Otherwise, i.e., if p > 1 + ps – δ, then all non-negative α values satisfy f7(1) < 0. Finally, there should not be any customers who choose (OP, P); first, if p > 1 - cp, then nobody can afford to patch. Otherwise, i.e., if p < 1 - cp, then v = 1 customer should not prefer to patch instead of SaaS. This condition can be written as 1 - p - cp ≤ δ – πdα(1 – vd) – ps, which is simplified to vd > 1 − (p + cp + δ − 1 − ps)/(πdα). Using (A.64) and (A.65), it follows that vd > 1- (p + cp + δ−1−ps)/(πdα) becomes equivalent to α ≤ â2 and p > 1 - cp – (δ – ps), which completes the proof.

By comparing all p-bounds in (A.59) together with α-bounds, we then establish all conditions in case (III).

Next, for case (II) in which there exists only SaaS consumption in equilibrium, i.e., 0 < va <1, from the threshold-type equilibrium structure, it follows that u = 0 and d = 1 - vd. We prove the following claim, which then proves the equilibrium characterization of case (II):

Claim: The equilibrium that corresponds to case (II) arises if and only if the following conditions are satisfied:

p > ps + 1 - δ and α < αD.

Proof: The threshold vd satisfies the following equation:

f8(vd) = vdδ(1 – πdα(1 − vd)) – ps = 0.

Since f8(vd) is quadratic in vd, f8(0) = -ps < 0 and f8(1) = δ – ps > 0, there exists the unique vd ∈ (0, 1) that satisfies (A.67). We need to guarantee that no consumer chooses (OP, NP) over (SaaS, ND). Note that in this case, if the highest type consumer does not choose (OP, NP) without security risk over (SaaS, ND), then no consumer will choose (OP, NP). Hence the condition becomes δ(1 – πdα(1 − vd)) ≥ 1 − p, which is simplified to

vd ≥ vd2 = 1 + (1 − p + ps - δ) / (αδπd)

This condition is equivalent to f8(vd2) ≤0, which is simplified to α < αP. Moreover, note that αP > 0 if and only if p > ps + 1 – δ, which completes the proof.

Finally, for case (I) in which there exists only on-premise consumption without patching in equilibrium, i.e., 0 < vu < 1, from the threshold-type equilibrium structure, we have u = 1 - vu and d = 0. First, we prove the claim:

Claim: The equilibrium that corresponds to case (I) arises, if and only if the following conditions are satisfied.

{ (p ≤ ps) or (ps < p < ps / (1 - πuα) and α ≤ αA) } and
{ (p > 1 - cp) or (p ≤ 1 - cp and α ≤ αB) } and
{ (p > ps) or (p ≤ ps and α ≤ αC) }.

Proof: The threshold vu satisfies the following equation:

f9(vu) = vu(1 – πuα(1 – vu)) – p = 0.

Since f9(vu) is quadratic in vu, f9(0) = -p < 0 and f9(1) = 1 − p > 0, there exists the unique vu ∈ (0, 1) that satisfies (A.70). Similar to the previous cases, first, we need to guarantee that SaaS consumption does not come below vu, which is achieved if either p < ps, or p > ps and vu ≤ ps/δ. The condition vu ≤ ps/δ is equivalent to f9(ps/δ) ≥ 0, which is simplified to α ≤ αA. Moreover, αA ≥ 0 if and only if p < ps/δ. Second, we need to guarantee that nobody wants to patch, which is achieved either if p > 1 - cp, i.e., nobody is afford to patch, or if p < 1 - cp and 1 − p − πuα(1 − vu) ≥ 1 − p − cp, i.e., even the highest-type (v = 1) consumer prefers (OP, NP) over (OP, P). The condition 1 - p - πuα(1 – vu) ≥ 1 − p − cp can be rewritten as vu ≥ 1 - cp/(πuα), which is equivalent to f9(1-cp/(πuα)) < 0; consequently, it is simplified to α < αB. In addition, we also need to guarantee that SaaS consumption does not come in above vu. If p > ps, then SaaS consumption cannot arise above vu in equilibrium. Otherwise, i.e., if p ≤ ps, the highest type consumer (v = 1) should prefer (OP, NP) over (SaaS, ND), which can be written as 1 − p − πuα(1 – vu) > δ – ps. This condition can be rewritten as vu ≥ 1 − (1 − p + ps − δ)/(πuα), which is equivalent to f9(1 – (1 − p + ps – δ)/(πuα)) ≤ 0; by simplifying, this inequality becomes α < αC, which completes the proof.

Note that αB < αC if and only if p < 1 - cp - δ + ps. In addition, αA ≤ αB if and only if ps(1 - cp)/δ ≤ p. Using these relationships and (A.69), we can then completely characterize the equilibrium conditions given above for case (I).

Proof of Corollary 1: From Lemma 1, we obtain (No SaaS) equilibrium outcome, i.e., case (V), when p < psδ – cp and α > αB. Note that psδ – cp > 0 if and only if ps > δcp. Second, again, from Lemma 1, (SaaS for low tier) equilibrium, i.e., case (VI), arises when max(ps, ps/δ - cp) < p ≤ ps(1 − cp)/δ and α > αE, or max(ps(1 − cp)/δ,ps) < p < 1 - cp and α > â1. These conditions can then be simplified to max(ps,ps/δ – cp) < p < 1 – cp and α > max(αE, â1). Finally, from Lemma 1, it follows that (SaaS for middle tier) equilibrium, i.e., case (VII), occurs when ps/δ− cp < p < min(ps, 1+ps - δ - cp) and α > αF, or min(ps, 1+ps - δ - cp) < p < min(ps, 1-cp) and α > â2. These conditions are then simplified to ps < δcp/(1-δ), ps/δ-cp < p < min(ps, 1-cp), and α > max(αF, â2), which completes the proof.

Proof of Proposition 1: Technically, we will prove that there exists α > 0 such that when α >α, p* and p* are set so that
(i) If cp > 1/3 and δ > 2(1-cp)/(1+cp), then σ*(v) is characterized by 1 > vp > vd > vu > 0 and given in (7) ;
(ii) Otherwise, σ*(v) is characterized by 1 > vp > vu > vd > 0 and given in (6).

By Lemma 1 and Corollary 1, for sufficiently high α, either vp > vd > vu or vp > vu > vd is satisfied under optimal pricing in equilibrium. Suppose vp > vd > vu. By (A.19), we obtain

vd = p + cp + (cpδπd – πu(p + cp - ps)(δ(p + cp) - ps)) / (αδπuπd(p + cp)²) + O(1/α²)

Substituting (A.71) into (A.18) and (A.16), we have

vu = p + cp + (cpδπd + πups(δ(p + cp) - ps)) / (αδπuπd(p + cp)²) + O(1/α²)

and

vp = p + cp + (cpδπd + πups(δ(p + cp) - ps)) / (αδπuπd(p + cp)²) + O(1/α²)

By substituting (A.71), (A.72), and (A.73) into (15) which applies in this case, it follows that

Π(p,ps) = p(1 − vp – cp) + (cpδπd + πups(δ(p + cp) - ps)) / (αδπuπd(p + cp)²)

By (9) and (A.74), the interior maximizing prices satisfy

pM = (1-cp)/2 + 2cp(3cp-1)/(πu(1+cp)³) + O(1/α²)
and
pM = δ(1-cp)/4 + 16cp(1+cp)³πdα / (πu(1+cp)³) + O(1/α²)

where A1 = 8cpδ(3 – cp(3 + 2δ) + cp(2δ – 5) + cp(5 + 4δ)) + δπu(1 + cp)³(1 + cp(2δ – 3)). By substituting (A.75) and (A.76) into (A.74), the vendor's profits are given by

ΠM = (1-cp)²/4 + cpδ/4 + A2 / (16(1+cp)³πdα) + O(1/α²)

where A2 = 4 + 5cp + 5cp² - 2cp³ and A3 = 8cpδ(3 - cp)(1 − cp) + δπu(1 + cp)³.
On the other hand, suppose vp > vu > vd. Following a similar analysis to the one above and using (18), the interior maximizing prices satisfy

pL = (1-cp)/2 + 2cp(3cp-1)/(πu(1+cp)³) + O(1/α²)
and
pL = δ(1-cp)/4 + δ(1+cp(2δ-3))/(16(1+cp)³πdα) + O(1/α²)

Substituting (A.78) and (A.79) into (18), we obtain

ΠL = (1-cp)²/4 + cpδ/4 + A4 / (16(1+cp)³πdα) + O(1/α²)

where A4 = δ(πu(δ – 2)(1 + cp)³ + 16cpπd(cp – 3)).

Comparing (A.77) and (A.80), it follows that ΠM > ΠL if and only if (64)πd²α² + (1 + cp)³(δ – 2)πu A3)πuα²(1 + cp)³ > 16(1 + cp) πdα² A4, which is satisfied if and only if cp > 1/3 and δ(1 + cp) > 2(1 – cp). This completes the proof.

Proof of Proposition 2: By Proposition 1, when cp > 1/3 and δ > 2(1-cp)/(1+cp) are satisfied, then p* =pM and p*=pM. Substituting (A.75) and (A.76) into (A.71), (A.72), and (A.73) and then subsequently into (17), we obtain

WM = 3(1-cp)²/8 + α/4 * (cpδ(1-cp)(3-cp))/(πu(1+cp)³) + 192(3-cp)²cpδπd / (32πuπd(1+cp)⁷) + O(1/α³)

where A5 = 5cp³-4cp²+5cp - 2 and A6 = 8πdcp(1 - cp)(7 + 3cp² – 14cp) + δπu(1 + cp)⁴.
On the other hand, if it is not the case that both are cp > 1/3 and δ > 2(1-cp)/(1+cp) are satisfied, then, by Proposition 1, p* =pL and p*=pL. Substituting (A.78) and (A.79) into (A.35), (A.36) and (A.38) and then subsequently into (17), we obtain

WL = 3(1-cp)²/8 + α/4 * (cpδ(1-cp)(3-cp))/(πu(1+cp)³) + 63(3-cp)A5 / (32πuπd(1+cp)⁴) + O(1/α³)

where A7 = πu(1+cp)⁴(δ–2)-32πd²(5-cp)(1-cp). However, comparing (A.82) and (A.83), it follows that WM > WL if and only if δ > 2(7-14cp+3cp²)/(7-cp)(1+cp). For cp ∈ (0, 1], note that 2(7-14cp+3cp²)/(7-cp)(1+cp) < 2(1-cp)/(1+cp) is always satisfied and 2(7-14cp+3cp²)/(7-cp)(1+cp) < 1 is satisfied whenever cp > (17 – 4√15)/7.

By Region III of Corollary 1, (A.75), and (A.76), pM ≥ pM/δ - cp is always satisfied and pM < δcp/(1 - δ) is always satisfied for sufficiently high δ. Also, by (A.75) and (A.76), pM <pM is satisfied if and only if

δ + cp(2δ – 3) / 4 + (δ(1 + cp(2δ – 3)) / (16cpπdα)) + O(1/α²) > 0.

Hence, there exist cp, η>0 such that if cp <cp < 1/3 and η <δ <1, then, by Proposition 1, p* = pL and p*=pL, but (A.84) is satisfied; hence, pM and pM can induce Region III of Corollary 1, which completes the proof.

Proof of Lemma 2: Note that the benchmark case corresponds to δ = 0 case. From Corollary 1, it then corresponds to (No SaaS) equilibrium outcome, i.e., 0 < vu < vp < 1. Thus, for the benchmark case, under high α, vu is given by the largest root of the polynomial equation

πuαvu³ + (1 – πuα(p + cp))vu² – 2pvu + p² = 0 .

By (A.85), for sufficiently large α, vu satisfies

vu = p + cp - πuα(p+cp)² / (πuα) + O(1/α³)

Maximizing p(1 – vu), we obtain

ΠBM = (1-cp)²/8 + πuα/4 + πuα²/16 + O(1/α³)

Using (A.108), the respective optimal profit and welfare expressions are given by

ΠBM = πuα/4 + πuα²/8 + O(1/α³)

and

WBM = 3πuα/8 + 5πuα²/128 + O(1/α³)

Moreover, similar to the proof of Lemma 2, using (A.86), (A.87) and (A.88), we obtain the average per-user security losses and the consumer surplus:

SLBM = 3πuα/8 + πuα²/16 + O(1/α³)

and

CSBM = 1/8 + πuα/8 + 3πuα²/128 + O(1/α³)

Finally, note that this case is consistent with August and Tunca (2006).

Proof of Proposition 6: By the proof of Proposition 5, (A.105), and (A.109), it follows that

(Π* – ΠBM) / ΠBM = δπdα / (16(1 – δ)) + O(α³) .

By (11), (A.99), (A.103), and (A.104), we obtain

(W* - WBM) / WBM = 5δπdα / (48(1-δ)) + O(α³) .

By (A.113) and (A.114), the result follows.

Proof of Proposition 7: Plugging (A.103) and (A.103) into SL* under low α region, we obtain

SL* = 3πuα/8 + 5πuα²/32(1 – δ) + O(α³) ,

From (A.115) and (A.111), it then follows that

(SL* - SLBM) / SLBM = (3 + 2δ)πuα / (12(1 – δ)) + O(α²) ,

which is negative when α is small. Next, substituting (A.103) and (A.103) into W* and Π* under low α region, and subtracting Π* from W*, we obtain

CS* = 1/8 + πuα/8 + 3πuα²/128(1 – δ) + O(α³) ,

Then, using (A.117) and (A.112), we have

(CS* - CSBM) = 3δπdα² / (128(1-δ)) + O(α³) ,

which is positive when α is small, which completes the proof.

Proof of Proposition 8: Under low security-loss environment, i.e., under a sufficiently small α, using (A.105), we obtain the profits as

Π(eu, ed, α) = 1/2 * πuα(1 – eu)α² / (8(1 – δ)) - Cu(eu) - Cd(ed) + πuα(1 – eu)(4πuα(1 – eu)πdα(1 – ed)(2δ – 1) – 4πuα(1 – ed)² + 3πuα(1 – eu)²)α³ / (128(1 – δ)²) + O(α⁴).

By taking a derivative of (A.119) with respect to eu, we obtain the first-order condition with respect to eu as follows:

dΠ / deu = πuα / 8 * (1 – eu)α² / (1 – δ) - Cu'(eu) + πuα(1 – eu)(9(1 – eu)²πdα + 8(2δ – 1)(1 – ed)πdα – 4(1 – ed)²πdα)α³ / (128(1 – δ)²) + O(α³) = 0.

Similarly, by taking a derivative of (A.119) with respect to ed, we obtain the first-order condition with respect to ed as follows:

dΠ / ded = πdαπuα(1 – eu)(1 – ed)(2δ – 1) / (32(1 – δ)²) - Cd'(ed) + O(α²) = 0.

From (A.121), under small α, if (1 – eu)πuα(2δ – 1) – 2πdα(1 – ed) < 0, then Π2 is negative, and hence ed = 0, in which case ed is a constant with respect to α. Next, we focus on the region in which (1 – eu)πuα(2δ – 1) – 2πdα(1 – ed) ≥ 0. Let Π11 ≡ ∂²Π/∂eu², Π22 ≡ ∂²Π/∂ed², and Π12 ≡ ∂²Π/∂eued. Then, using C″ > τ and C″ > τ, we obtain that Π11 < 0 and Π22 < 0 under small α. Furthermore, we also have

Π12 = -πdαπuα(πdα(1 – ed) – (2δ – 1)πuα(1 – eu))α³ / (16(1 – δ)²) + O(α⁴).

Using Π12 in (A.122) together with Π11 and Π22, and the condition C″ > τ and C″ > τ, we obtain that the highest order term of α in Π11Π22 – Π12² > 0 under small α is a constant τ² which is positive. Consequently, the second order condition is satisfied, and the unique pair of optimizer (e*u, e*d) exists. Let Π13 ≡ ∂²Π/∂euedα, Π23 ≡ ∂²Π/∂edα. By taking a derivative of (A.120) and (A.121) with respect to α, we obtain

de*u / dα = (Π12Π23 - Π22Π13) / (Π11Π22 – Π12²)
and
de*d / dα = (Π12Π13 - Π11Π23) / (Π11Π22 – Π12²)

First, for the numerator of de*u/dα, the highest order term of α under low security-loss environment is a constant term greater than τπuα/8, which is positive. Moreover the denominator of de*u/dα is positive, by using a strict convexity of Cu and Cd. As a result, de*u/dα is positive, i.e., e*u(α) is increasing in α. Second, for the numerator of de*d/dα, the highest order term of α under low security-loss environment is the second order term and greater than

-3τ(1 – eu)πuαπdα((1 – ed)πdα(2δ – 1) – 2πdα(1 – eu)) / (32(1 – δ)²) ,

which is positive when ed > 0 from (A.121). Similarly, as a result, it then follows that de*d/dα is positive, i.e., e*d(α) is increasing in α.

For the high security-loss environment, from Proposition 1, SaaS can be either in the middle tier or in the low tier in equilibrium. First, if SaaS goes into the middle tier in equilibrium, the firm's profit (except the investment costs) is given in (A.77). Following the steps for the low security-loss environment, we obtain first order conditions as follows:

dΠ / deu = cpδ(1 – cpδ(1 – eu)) / (8cp) - Cu'(eu) + cpδ(1 – cpδ(1 – eu)) / (4α) * ( (1 + cpδ(1 – eu))³πuα ) / (8cp) + O(1/α²) = 0.

and

dΠ / ded = cpδ(1 – cpδ(1 – ed)) / (4α) - Cd'(ed) + O(1/α²) = 0.

under large α. Moreover, from the condition τ > 1/2, it follows that Π11 ≡ ∂²Π/∂eu² <-τ+cp/2 < 0 and Π22 ≡ ∂²Π/∂ed² < −τ < 0 for large α. In addition, we obtain

Π12 = cpδ / (4α) * (1 – ed) / (πdα) + O(1/α²) .

Then, it follows that Π11Π22 – Π12² > 0 for large α, which then implies that the second order condition is satisfied, and hence there exists the unique maximizer (e*u, e*d). Next, in (A.124), the denominator of de*u/dα is positive from the second order condition. Furthermore, the numerator of de*u/dα in (A.124) has the highest order term, which is greater than

τ / (8cpδ(1 – cpδ(1 – eu))³ / (1 + cpδ(1 – eu))³πuα) + πuα / (8cp) * (1 – eu) / (πuα)

Note that A is finite and negative, and C is finite and positive in equilibrium; as a result, there exists τ such that for all B > τ, (A.129) is positive. Consequently, under this condition, de*u/dα is positive for large α, i.e., e*u increases in α. Similarly, the numerator of de*d/dα in (A.124) has the highest order term, which is greater than

cpδ(2τ - cpδ)(1-cpδ) / (8πdα(1 – cpδ)²) ,

and it is negative for large α since τ > 1/2. Hence, e*d increases in α. Next, we show that SaaS goes into the middle tier in equilibrium. From Proposition 1, we need to show that cpδ(1 – eu) ≥ 1/3 and δ > 2(1-cpδ)/(1+cpδ). First, if SaaS goes to the middle tier, e*u satisfies (A.126), which can be simplified to

cpδ(1 – cpδ(1 – eu)) - Cu'(eu) = 0

Note that at eu = 1 - cpδ/(2+δ), under large α, the left hand side of (A.131) can be written as

cpδ / (2+δ) * (1 - cpδ/(2+δ)) - Cu'(1 - cpδ/(2+δ)) + O(1/α)

by C″ > τ ≥ 1/2. Using δ ≥ δ, we obtain that (A.132) is negative under large α, which implies that the left hand side of (A.131) at eu = 1 - cpδ/(2+δ) is negative. Hence, e*u < 1 – cpδ/(2+δ), which then implies δ > 2(1-cpδ)/(1+cpδ). In addition, cpδ ≥ 1/2 guarantees that â ≥ 1 and cpδ(1-cpδ) ≥ 1/3.
Moreover, suppose that SaaS goes to the low tier in equilibrium, in which case the profit (except the investment costs) is given in (A.80). Following the same steps, under the conditions presented in the proposition, it follows that cpδ(1 – δ) ≥ 1/3 and δ > 2(1-cpδ)/(1+cpδ) are still satisfied, i.e., there is no interior maximizer of investments (e*u, e*d) in this case; as a result, the interior optimizer found in the previous case of SaaS in the middle tier is the global optimizer, which completes the proof.

Proof of Proposition 9: From the proof of Proposition 8, under a high security-loss environment, when 1/2 < cpδ, 1/2 < τ, and δ > δ, SaaS goes to the middle tier in equilibrium. Furthermore, e*u satisfies (A.126) and e*d satisfies (A.127). Comparing these two first order conditions, we obtain that e*u > e*d under a sufficiently large α, which completes the proof.
