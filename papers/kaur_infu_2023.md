# Artificial Intelligence for Cybersecurity: Literature Review and Future Research Directions

**Authors:** Ramanpreet Kaur*, Dušan Gabrijelčič, Tomaž Klobučar  
**Affiliation:** Laboratory for Open Systems and Networks, Jožef Stefan Institute, Ljubljana, Slovenia

**Published in:** Information Fusion 97 (2023) 101804  
**Available online:** 7 April 2023  
**License:** CC BY-NC-ND 4.0

---

## Abstract

Artificial intelligence (AI) is a powerful technology that helps cybersecurity teams automate repetitive tasks, accelerate threat detection and response, and improve the accuracy of their actions to strengthen the security posture against various security issues and cyberattacks. This article presents a systematic literature review and a detailed analysis of AI use cases for cybersecurity provisioning. The review resulted in 2395 studies, of which 236 were identified as primary. This article classifies the identified AI use cases based on a NIST cybersecurity framework using a thematic analysis approach. This classification framework will provide readers with a comprehensive overview of the potential of AI to improve cybersecurity in different contexts. The review also identifies future research opportunities in emerging cybersecurity application areas, advanced AI methods, data representation, and the development of new infrastructures for the successful adoption of AI-based cybersecurity in today's era of digital transformation and polycrisis.

**Keywords:** Detection, Protection, Response, Recovery, Identify, Learning, Cyberattacks, Taxonomy

---

## 1. Introduction

The term cybersecurity refers to a set of technologies, processes and practices to protect and defend networks, devices, software and data from attack, damage or unauthorized access [1]. Cybersecurity is becoming complex because of the exponential growth of interconnected devices, systems and networks. This is exacerbated by advances in the digital economy and infrastructure, leading to a significant growth of cyberattacks with serious consequences. In addition, researchers report the continued evolution of nation-state-affiliated and criminal adversaries, as well as the increasing sophistication of cyberattacks, which are finding new and invasive ways to target even the savviest of targets [2]. This evolution is driving an increase in the number, scale and impact of cyberattacks, and necessitating the implementation of intelligence-driven cybersecurity to provide a dynamic defence against evolving cyberattacks and to manage big data. Advisory organizations, such as the National Institute of Standards and Technologies (NIST), are also encouraging the use of more proactive and adaptive approaches by shifting towards real-time assessments, continuous monitoring and data-driven analysis to identify, protect against, detect, respond to, and catalogue cyberattacks to prevent future security incidents [3].

AI is an intriguing tool that can provide analytics and intelligence to protect against ever-evolving cyberattacks by swiftly analysing millions of events and tracking a wide variety of cyber threats to anticipate and act in advance of the problem. For this reason, AI is increasingly being integrated into the cybersecurity fabric and used in a variety of use cases to automate security tasks or support the work of human security teams. The flourishing field of cybersecurity and the growing enthusiasm of researchers from both AI and cybersecurity have resulted in numerous studies to solve problems related to the identification, protection, detection, response and recovery from cyberattacks.

Several reviews on cybersecurity and AI applications were published in recent years [4–7]. However, to the best of our knowledge, there is no comprehensive review that covers state-of-the-art research to explain cybersecurity activities covered by AI techniques and the details of how they are applied. Therefore, our objective was to provide a systematic review, a comprehensive view of AI use cases in cybersecurity, and a discussion of the research challenges related to the adaptation and use of AI for cybersecurity to serve as a reference for future researchers and practitioners. Table 1 shows a comparison of the study with review articles from recent years.

We performed a systematic literature review (SLR) on the use of AI for the provision of cybersecurity, with a particular focus on practical applications within five different cybersecurity functions (Identify, Protect, Detect, Respond and Recover) defined by the NIST cybersecurity framework [3]. The specific research questions addressed by this SLR are:

- **RQ1:** What would be the taxonomical representation of the application of AI for the provision of cybersecurity?
- **RQ2:** What are the specific use cases of AI for cybersecurity?
- **RQ3:** What are the current research trends associated with AI for cybersecurity?
- **RQ4:** What are the trending topics and future research directions for the adoption of AI for cybersecurity?

To answer these research questions and to provide a valuable output for the research community, 236 articles were examined prior to February 2022. Then, the selected studies were further analysed to specify the cybersecurity applications where AI was used, the selected AI domain, and the resulting impact. The SLR led to the following:

- A taxonomy of AI for cybersecurity that provides the multi-level classification of the reviewed articles based on the cybersecurity functions, solution categories, and specific use cases.
- Specific use cases of AI for cybersecurity to reveal the potential areas to harness the capabilities of AI.
- A descriptive analysis of the literature to explore the research trends of AI for cybersecurity.
- A critical analysis of the existing literature, identifying research gaps, to stimulate future research in the field.

The rest of the article is structured as follows. Section 2 discusses the relevant background to provide an introduction and conceptualization of cybersecurity and AI topics along with an explanation of the classification paradigms used in the literature related to AI for cybersecurity. Section 3 describes the research methodology adopted to conduct the SLR. Section 4 discusses the data extraction process to feed the descriptive analysis and state-of-the-art research presented in Section 5. Section 6 provides a descriptive analysis of the synthesized literature review. Section 7 identifies various research gaps that new studies can target, while Section 8 points out the limitations of our study. Finally, Section 9 presents the main conclusions and the research implications of this SLR.

### Table 1: Comparison of this review with existing studies

| References | Taxonomy | Use case identification | Classification of defence solution based on the Function | AI domain | SLR | Coverage | Research gaps | Purpose |
|------------|----------|------------------------|-------------------------------------------------------|-----------|-----|----------|---------------|----------|
| Wiafe et al. [4] | No | No | No | Yes | Yes | IEEE & ACM digital library | No | Provides an overview of existing research on AI for cybersecurity |
| Zhang et al. [5] | No | No | No | No | Yes | Google Scholar, SpringerLink, ScienceDirect, IEEE & ACM digital library | No | Provides a review constrained to the application of AI in the areas of user authentication, dangerous behaviour monitoring, network situation awareness, & identification of abnormal traffic |
| Torres et al. [6] | No | No | No | No | No | Nil | No | Reviews the application of machine learning techniques in spam, malware, and phishing detection |
| Truong et al. [7] | No | No | No | No | No | Nil | No | Reviews the application of AI techniques in intrusion, malware, APT and phishing detection |
| Proposed Study | Yes | Yes | Yes | Yes | Yes | Scopus Database | Yes | Explores research from 2010 to February 2022 related to AI applications for cybersecurity from a descriptive point of view, and a detailed state-of-the-art analysis |

---

## 2. Background

This section is dedicated to analysing the background information concerning the key concepts of this review, including the operational definition of cybersecurity using the NIST cybersecurity framework [3] and the AI taxonomy proposed by AI Watch [8] to clarify the concept of different applications of AI for cybersecurity.

### 2.1. Cybersecurity

Cybersecurity puts policies, procedures and technical mechanisms in place to protect, detect, correct and defend against damage, unauthorized use or modification, or exploitation of information and communication systems and the information they contain. The rapid pace of technological change and innovation, along with the rapidly evolving nature of cyber threats, further complicates the situation. In response to this unprecedented challenge, AI-based cybersecurity tools have emerged to help security teams efficiently mitigate risks and improve security. Given the heterogeneity of AI and cybersecurity, a uniformly accepted and consolidated taxonomy is needed to examine the literature on applying AI for cybersecurity. This structured taxonomy will help researchers and practitioners come to a common understanding of the technical procedures and services that need to be improved using AI for the implementation of effective cybersecurity.

For this purpose, a well-known cybersecurity framework proposed by NIST was used to understand the solution categories needed to protect, detect, react and defend against cyberattacks [3]. The NIST cybersecurity framework's core describes the practices to improve the cybersecurity of any organization. The framework's core has four elements: Functions, Categories, Subcategories and Informative references. The first two levels of the NIST framework, which consist of 5 cybersecurity functions and 23 solution categories, were used to classify the identified AI use cases. The functions provide a comprehensive view of the lifecycle for managing cybersecurity over time. The solution categories listed under each function offer a good starting point to identify the AI use cases to improve the cybersecurity. The main purpose of selecting these two levels is to provide a clear and intuitive categorization to classify the existing AI for cybersecurity literature into the appropriate solution category. The proposed taxonomy introduces a third level consistent with the first two levels by specifying AI-based use cases corresponding to each level of the cybersecurity framework, as shown in Fig. 1. A detailed description of the proposed taxonomy with a state-of-the-art review of AI for cybersecurity is provided in Section 5.

This taxonomy forms the basis for our SLR, by providing a description of the related subfields to cover the main aspects and fundamental keywords in the definition of cybersecurity solution categories. A detailed description of the keyword selection can be found in Section 3.

### 2.2. Artificial Intelligence

Several definitions of AI systems can be found that relate to (a) the fields in which they are used and (b) the stages of an AI system's lifecycle, such as research, design, development, deployment and use. Since the focus of this paper is on AI applications for cybersecurity, a prevailing, but simplified, definition of AI is adopted: "systems that exhibit intelligent behaviour by analysing their environment and with some degree of autonomy take actions to achieve specific goals" [9]. In practical terms, AI refers to a number of different technologies and applications that are used in a variety of ways. AI use cases in cybersecurity describe which environmental situations are desirable and undesirable, and assign actions to sequences.

For this SLR, the AI taxonomy proposed by Samoili et al. [8], which defines the core and transversal AI domains and subdomains, is used. The core AI domains, i.e., reasoning, planning, learning, communications and perception, were found to be useful as they encompass the main scientific areas of AI. Reasoning deals with knowledge representation and different ways of reasoning, while planning also covers searching and optimisation. Learning includes machine learning; communication is related to natural language processing; and perception is about computer vision and audio processing [8]. The approaches and technologies that make up these AI domains include, but are not limited to, fuzzy logic, case-based reasoning, genetic algorithm, Bayesian optimization, evolutionary algorithm, planning graph, artificial neural network, deep learning, support vector machine, natural language processing, text mining, sentiment analysis, image processing, sensor networks, object recognition and speech processing.

AI is a large, multidisciplinary research area, with a large body of literature addressing its applications and consequences from a variety of perspectives, e.g., technical, operational, practical and philosophical. This study focuses on the literature's thread that discusses the implications of the aforementioned methods and AI applications in cybersecurity scenarios. It analyses in detail how AI methods can be used for the identification, protection, detection, response and recovery in the domain of cybersecurity.

---

## 3. Research Methodology

The SLR aims to identify, evaluate and interpret all the available research in the area of interest to identify potential research gaps and highlight the frontiers of knowledge. It provides a high-quality, transparent and replicable review to summarize the large number of research studies. This study follows an SLR methodology for the following reasons: (i) AI for cybersecurity is a diverse field with a large quantity of literature; (ii) this study aims to answer specific research questions; (iii) the rigour and replicability it provides leads to an unbiased scientific study. The procedure for the SLR is described in detail below.

### 3.1. Selection of Bibliometric Database

Scopus and Web of Science (WoS) are the two most popular bibliometric databases. The Scopus database was chosen for this study because its coverage is almost 60% larger than that of the WoS [10]. In addition, Scopus offers better data management due to its wider coverage, advanced search filters and data analysis grids.

### 3.2. Search Strategy

Between November 2021 and February 2022, a comprehensive search for terms related to AI and cybersecurity was conducted for the purpose of a thorough literature review of the impact of AI on cybersecurity. The search was performed using the well-specified search terms for the AI and cybersecurity fields, as shown in Table 2. The keywords of the AI and cybersecurity fields were combined using the logical AND operator. The logical OR operator within the different keywords was used to find studies that are related to any of the terms in each field. Specifically, the AI keywords correspond to the AI taxonomy proposed by AI Watch [8], and the cybersecurity keywords were taken from the NIST cybersecurity framework [3].

### Table 2: Search string

| AI Keywords | Cybersecurity Keywords |
|-------------|------------------------|
| (("reasoning" OR "optimization" OR "machine learning" OR "artificial intelligence" OR "Natural language processing" OR "text mining" OR "classification" OR "feature extraction" OR "data mining" OR "sentiment analysis" OR "computer vision" OR "recognition" OR "genetic" OR "filtering" OR "GAN" OR "deep learning" OR "reinforcement learning" OR "data driven" OR "topic modelling") | ("cybersecurity") AND (("asset management" OR "inventory" OR "configuration" OR "security control validation" OR "assessment" OR "asset" OR "security control testing" OR "security posture" OR "business impact" OR "governance" OR "risk management" OR "team" OR "risk indicators" OR "risk assessment" OR "automated vulnerability" OR "vulnerability" OR "fuzzing" OR "penetration" OR "vulnerability severity" OR "vulnerability management" OR "threat hunting" OR "automated penetration" OR "attack graph" OR ("risk" AND "investment") OR "risk quantification" OR ("risk" AND "supply chain") OR "role mining" OR "role maintenance" OR "Multi-Factor authentication" OR "authentication" OR "identity" OR ("contextual" AND "authentication") OR "access control" OR "unauthorized access" OR "VPN" OR ("attribute based access") OR "Role based access" OR "segregation" OR "isolation" OR "isolate" OR "network segmentation" OR "data loss" OR "data leakage" OR "SQL injection attack" OR "APT" OR "email" OR "malicious domain" OR ("integrity" AND "files") OR ("integrity" AND ("monitoring" OR "auditing")) OR ("automated" AND "configuration") OR "fake news" OR "backup" OR (("backup") AND ("data" OR "code")) OR "plan" OR (("business continuity" OR "disaster Recovery" OR "incident response") AND ("automated")) OR "risk scoring" OR "risk prioritization" OR "vulnerability exploitation" OR (("Risk") AND ("remediation")) OR (("log" OR "audit") AND ("analysis")) OR "SIEM" OR "VPN" OR "firewall" OR "IPS" OR "antivirus" OR "antimalware" OR "immune system" OR ((("anomaly") OR ("event") OR ("intrusion") OR ("fraud")) AND ("detection") OR (("event correlation") OR ("security intelligence") OR ("event analysis") OR ("correlation") OR ("SIEM") OR ("SOC") OR ("monitoring") OR ("behavior Based") OR ("social network") OR ("threat intelligence")) OR ("dark web") OR ("chatter noise") OR ("translate") OR ("topic modelling") OR ("sentiment analysis") OR ("cyber trap") OR ("threat intelligence") OR ("darknet") OR ("deepnet") OR ("social network") OR ("sentiment") OR ("honeypot")) OR (("incident") AND (("detection") OR ("response") OR ("playbook") OR ("case based") OR ("case") OR ("identification") OR ("assessment") OR ("classification") OR ("categorisation") OR ("categorising"))) OR (("cybersecurity") AND ("triage")) OR (("forensic") AND (("intelligent") OR ("incident")) OR "isolation" OR "remediation" OR "risk quantification" OR "recommender system" OR (("incident") AND (("analysis") OR ("report") OR ("document") OR ("information"))) OR (("recovery") AND (("planning") OR ("dynamic")) OR ("safe")) OR "recovery") |

### 3.3. Inclusion and Exclusion Criteria

Following the search stage, the studies identified were screened to eliminate irrelevant work. To find the pertinent papers that address the research questions, the studies gathered in the earlier stage were subject to inclusion and exclusion criteria. A significant, yet manageable, selection of studies must be ensured at this point. The search conducted was not limited to a specific period and also considered early publications to avoid overlooking any important studies. The inclusion criteria were as follows:

- The article is written in English.
- The article is a full research paper (i.e., not a presentation or supplement to a poster).
- The article should make it apparent that AI is its primary emphasis or include AI as a large part of the methodology. For example, publications that explicitly include machine learning as a core component of their methodology/research.
- One or more of the research questions posed in this research are directly answered by the article.
- For studies that have appeared in multiple journals or conferences, the most recent version is considered.

The following publications were excluded from further review:

- The studies that are not written in English;
- The studies that provide a review or survey of AI in different cybersecurity domains;
- The articles that represent the same work by authors in different conferences or journals were also filtered to remove duplicates;
- The articles that provide a comparative analysis of different AI models or existing techniques for cybersecurity tasks;
- The articles that improve the security of AI techniques to make them attack resistant;
- The papers providing only recommendations, guidelines or principles for cybersecurity (non-scientific);
- Editorials, books, chapters and summaries of workshops and symposiums;
- The studies that do not provide sufficient information;
- The studies that have fewer than 5 pages;
- The studies where a full text could not be found.

### 3.4. Selection of Primary Studies

Fig. 2 shows in detail the selection process for the study. After the initial step of identifying and applying a search term, the inclusion and exclusion criteria were applied to refine the 2395 studies retrieved from the Scopus database. Based on the removal of non-English papers, posters, reviews, surveys, non-scientific publications, editorials, books, chapters, summaries of workshops and symposia, duplicates, guideline documents, and comparative studies, 366 articles were removed, leaving 2029. These 2029 studies were analysed based on the title and abstract. The title and abstract provided a clear indication of whether the study was outside the focus of the review and could therefore be excluded. If the title or abstract did not clearly indicate the application domain or contribution of the study, it was included in the review for subsequent steps where full text of the article was examined. Based on the title and abstract analysis, the 2029 studies were further narrowed down to 638. After a thorough examination of the full articles, 402 additional studies were eliminated. As a result, a total of 236 primary studies served as the basis for this SLR. The next sections present the findings and analysis of these 236 primary studies.

---

## 4. Data Extraction

After the selection of the primary studies, data extraction began to feed the state-of-the-art and descriptive analysis phase. The main goal of data extraction is to break down each study into its constituent parts and describe the overall relationships and connections. The data extraction parameters (explained in Table 3) collect the qualitative and contextual data from the primary studies selected for the SLR. The qualitative data are collected to write a short summary of each primary study to present the contribution along with the demographic information. The contextual data include details about the cybersecurity function, solution category, use cases, and core AI domain, to have a clear understanding of the existing literature. These qualitative and contextual data are further examined to identify the relationships between the different studies.

### Table 3: Data extracted from each primary study

| Data Type | Data Item | Description |
|-----------|-----------|-------------|
| Qualitative Data | Title | Title of the primary study |
| | Author | Author of the study |
| | Year Published | Publication year of study |
| | Article Type | Publication type, i.e., conference, journal |
| | Source | Journal/Conference name that published the study |
| | Geographical Region | Geographic region of the authors of the primary study |
| | Summary | A summary of the paper, with major contribution. |
| Contextual Data | Cybersecurity Function | Type of cybersecurity activity in primary study. NIST taxonomy defines cybersecurity activities as 5 functions: Identify, Protect, Detect, Respond, Recover. |
| | Solution Category | Identification of the main solution category in which primary study falls. The NIST taxonomy provides a subdivision of each cybersecurity function into groups of cybersecurity solution categories, e.g., the detection function is divided into 3 categories: anomalies and events, security continuous monitoring and detection processes. |
| | Specific Use Case | Specific cybersecurity use case of primary study for AI application to match the function and solution category. |
| | Core AI Domain | Core AI domain of the AI technique used by the primary study as defined by the AI Watch [7]. |

---

## 5. State of the Art

To identify the studies that evaluate the application of AI for cybersecurity, a taxonomy is proposed to classify the studies that address the first two research questions (RQ1 and RQ2). The first two levels of the taxonomy are adopted from the NIST cybersecurity framework. The first level organizes the cybersecurity literature into five core functions: identify, protect, detect, respond and recover. These five cybersecurity functions cover the use of AI tasks from the prevention of the security attack to the more complex mechanism of actively looking for new threats and counterattack. The functions cope with different aspects of the cybersecurity attack lifecycle for an effective defence. The second level of taxonomy uses the NIST framework's categories to expand the core functions into different cybersecurity solutions with closely tied programmatic needs and particular activities. The last level of the taxonomy presents the AI use cases associated with the upper level of taxonomy and link the SLR with each identified use case. Fig. 3 summarizes the proposed taxonomy and presents the logical progression of cybersecurity functions along with a detailed description of the different categories of cybersecurity solutions implemented using the AI technologies.

### 5.1. Identify

The identify function provides the foundation for the other cybersecurity functions by pinpointing the critical functions and risks associated with systems, people, assets and data. This helps develop an understanding of the current state of the cybersecurity, identify gaps, and develop an appropriate risk management strategy to achieve the desired security based on the organization's own needs, risks and budget. Table 4 summarizes the main contribution of each primary study in the identify function. The various categories of cybersecurity solutions in this function are detailed below.

#### 5.1.1. Asset Management

Asset management is the process of identifying and keeping track of the information, people, equipment, systems and buildings that help an organization accomplish its goals and are proportionate to the asset's relative importance to those goals and risk strategies. It includes the discovering, inventorying, managing and tracking of assets to protect them. Cybersecurity asset management is becoming increasingly complex as organizations have more platforms than ever before: from operational technology systems and Internet of Things (IoT) to on-premises and cloud-based services. This proliferation of new asset types and the ability to work remotely have resulted in highly distributed assets that are difficult to manage and inventory.

An AI-based asset management system can solve many of these challenges by feeding new levels of intelligence to the human team across the following use cases.

##### 5.1.1.1. Asset Inventory Management

Asset discovery and management are critical to ensure complete visibility and control over all assets in an extended network. AI can help with the continuous and automatic discovery of all devices, applications and users, as well as their classification and criticality for operations. With an accurate and up-to-date inventory, assets can be tracked and analysed for a risk assessment against known attack vectors, and compliance monitors can detect rogue assets and unauthorized use.

Researchers have developed different approaches to asset classification using machine learning algorithms. Promyslov et al. [11] used a k-means clustering to classify the assets according to their cybersecurity requirements based on their safety, functionality and integrity in a nuclear power plant. Millar et al. [12] proposed a random forest-based machine learning classifier for operating system classification and identification of the vulnerable devices on the network. Several studies [13–15] focus on identifying and classifying IoT devices based on their network-traffic characteristics. Aksoy et al. [13] and Sivanathan et al. [14] worked for single-device identification and classification using multiple and multi-stage machine learning methods, respectively, and are only suitable for a small IoT network. Cvitić et al. [15] proposed a solution to the classification problem in a rapidly evolving, heterogeneous and dynamic environment by using a supervised machine learning method capable of assigning IoT devices to predefined classes based on the values of their traffic flows.

Researchers are also working on the identification and blocking of malware infected assets [16], the determination of asset criticality [17], and the risk assessment of individual assets [18] to manage and ensure their security.

##### 5.1.1.2. Automated Configuration Management

Configuration management is a governance process for defining and maintaining the desired state of a system and providing timely alerts for any misconfiguration. The automated configuration management system will consistently define the system settings and maintain the system accordingly by only allowing changes in a controlled and authorized environment.

The customization of the system's configuration to ensure the required level of performance and security is important to reduce human error due to manual or sub-optimal configuration settings. Researchers [19,20] are working on dynamic configuration systems for online file sharing systems and distributed cloud storage based on system characteristics and operating environments using multi-objective reinforcement learning and genetic algorithms, respectively. Sharifi et al. [21] and Bringhenti et al. [22] proposed a fully automated framework for the customization of security controls by observing the user's behaviour and by refining high-level security requirements expressed in a human-friendly language, respectively.

Automated configuration assessment provides the compliance team with the ability to continuously review and test the configuration to identify the vulnerable configuration in time to reduce or avoid cybersecurity incidents. Varela-vaca [23,24] proposed a method based on software product line techniques to automatically analyse the vulnerable configurations of the system. Liu et al. [25], on the other hand, demonstrated the use of a random forest model to predict cybersecurity incidents based on the misconfiguration of the DNS and BGP protocols along with the externally visible malicious activities originating from the network.

##### 5.1.1.3. Automated Security Control Validation

The automation of security control validation will provide the real-time monitoring of security in a changing environment and threat landscape. Researchers are working on the implementation of AI techniques for a definitive assessment of the overall security of the system using a network's telescope data [26], a building's cybersecurity framework [27], or by correlating the threat, vulnerabilities and security measures [28].

#### 5.1.2. Business Environment

The business environment category is defined to identify the critical processes and applications that ensure business continuity in adverse scenarios. This information is critical to business sustainability and serves as the basis for developing effective response and recovery strategies. AI technology can be used to automate this process via the following use case.

##### 5.1.2.1. Automated Business Impact Analysis

Business impact analysis is the most important technique to determine critical functions and applications in the business environment by evaluating the impact of cybersecurity incidents on the business. AI techniques can be used to automate the business impact analysis by evaluating the economic risks based on a known attack vector or by calculating the threat feasibility along with the probability of high-impact security events on critical business areas. Researchers are measuring the economic risk of cybersecurity in different businesses using the modelling of different known attack profiles [29], rare-event simulation [30], or by linking the business objective to the attacker's capabilities to guide a scenario analysis [31] to determine its impact on business assets.

#### 5.1.3. Governance

Governance involves the policies, procedures and processes for understanding the environmental and operational requirements, and monitoring the regulatory requirements of the organization. This helps to identify an organization's responsibilities and provides information about cyber risks to the management. AI can be used for policy enforcement or automating the retrieval of key risk indicators. While there is some research on policy enforcement, no research articles on measuring risk indicators in real time were found in this study. Therefore, it is a temping future research direction to develop an early-warning system to indicate risk development over time due to policy violations, red flags or other symptoms. The automatic retrieval of key risk indicators, such as the mean time between failures, the presence of unpatched systems, risk appetite or the number of attempted breaches, and converting them into knowledge, will be beneficial to prevent a cybersecurity breach by rapidly remediating the risk.

##### 5.1.3.1. Automated Policy Enforcement

Policy enforcement is crucial for organizations to ensure their compliance with the regulations and appropriate risk management. AI is being used in automated policy enforcement in traditional non-SDN networks by using a controller and policy proxies [32]. The controller is a centralized management server used to manage software defined middleboxes for traditional routers and a policy proxy that will identify the traffic that is subject to polices and assists it in policy enforcement.

#### 5.1.4. Risk Assessment

Risk assessment is the process of identifying, estimating and prioritizing cybersecurity risks associated with operations, operational assets and individuals currently or in the near future. It requires a careful analysis of threat, vulnerability and attack information to determine the extent to which cybersecurity events could adversely impact on the organization and the likelihood that such events will occur. The manual risk assessment process is complex, costly and time consuming due to the large number of risk factors, and it requires active human involvement at every stage. The AI-based risk assessment process addresses these challenges by supporting the risk management team in the following use cases.

##### 5.1.4.1. Automated Vulnerability Identification & Assessment

An automated vulnerability assessment is the process of systematically reviewing security weaknesses in a system using automated tools for vulnerability identification, classification, exploration and prioritization These automated tools rely on vulnerability repositories, vendor vulnerability announcements, asset management systems, and threat intelligence feeds to identify, classify and assess the severity, and make recommendations for the remediation.

**Automated vulnerability detection:** It is an important step to identify the vulnerabilities of applications, servers or other systems and assets of an organization. Researchers have worked on the software vulnerability detection by checking the source code using deep learning and transfer learning [33–35]. These studies employ text-mining techniques to feed the machine learning based vulnerability detection models in unison with a recommendation system to help programmers to write secure code.

Researchers have also worked on detecting the emerging vulnerabilities of software [36] and cybernetic infrastructure [37] using vulnerability repositories or social networks, respectively. Saha et al. [38] proposed a new scheme for the identification of vulnerabilities across the system and network levels by modelling the behaviour of cyber-physical systems (CPS)/IoT under attack at the system and network levels and then use machine learning to discover any potential attack space.

Researchers use AI-based fuzzing to discover vulnerabilities in software and hardware interfaces and applications. This is done by injecting erroneous, unexpected or randomly generated data into a program or interface and then monitoring for events like crashes, failed code assertions, undocumented jumps or debug routines, and possible memory leaks. AI techniques are leveraged to develop an automated system for identifying potential attack options, input generation, the generation of probable test cases and analysing crashes, as shown in Fig. 4. Researchers [39,40] used reasoning and natural language processing for seed generation techniques to increase the code coverage with more unique execution paths as one of the basic steps of the smart fuzzing system. Test case generation is one of the most widely studied fields of AI-based fuzzing for web browsers [41], compilers [42,43], cyber-physical systems (CPS) [44], software libraries [45] and simple computer programs [46].

Automated penetration testing is an efficient and intelligent attempt to penetrate an attack surface by exploiting known or zero-day vulnerabilities to identify what the attacker can gain from current environments. Researchers are working on devising autonomous penetration testing using reinforcement learning for large networks [47,48] and microgrid control algorithms [49].

**Automated vulnerability classification:** Vulnerability classification is an important step that facilitates a deeper understanding of security related information to accelerate the vulnerability assessment. Researchers are working on automatic vulnerability classification systems and for labelling vulnerability descriptions in vulnerability reports. Russo et al. [50] proposed an approach to summarize the daily posted vulnerabilities and categorize them according to the defined taxonomy model for the industry. Aota et al. [51] addressed the use of text mining to classify vulnerabilities using the description provided in the Common Vulnerabilities and Exposures (CVE) list. Vanamala et al. [52] also categorize the CVE entries to the Open Web application Security Project (OWASP) top-10 risks.

**Vulnerability exploration:** An important step in vulnerability assessment is to identify the potential attack vectors that can exploit the vulnerabilities to effectively evaluate and manage them. For this purpose, some researchers use the dataset from the MITRE corporation [53,54], while others use the CVSS provided by the Forum of incident response and security teams [55]. Bakirtzis et al. [53] and Kuppa et al. [54] used a model-driven process to automatically map adversarial tactics, techniques and common knowledge to the given system model. In contrast, Chatterjee & Thekdi used a probabilistic model to evaluate and manage the system vulnerabilities by rapidly adapting to the changing network and attack characteristics [55].

**Vulnerability assessment and prioritization:** The main objective of this step is to prioritize vulnerabilities and to provide an assessment report based on its severity and the vulnerability exposure of the systems. AI techniques are used to assign a severity score to each vulnerability based on the system, data and business at risk, along with the ease, severity and potential damage of a resulting attack. Jiang and Atif [56] worked on the automatic assessment and reconciliation of the vulnerability severity from conflicting vulnerability reports using the machine learning pipeline based on the vulnerability severity and threat profile metrics. Samtani et al. assessed the vulnerabilities of the SCADA devices from the Shodan dataset and classified them into four main risk levels: critical, high, medium and low [57]. Brown et al. calculate the vulnerability and exploit risk scores for every IoT device in the attack graph created using the network topology specified by the network administrator [58].

##### 5.1.4.2. Automated Threat Hunting

Automated threat hunting is a proactive security search across networks, endpoints and datasets to detect potentially malicious, suspicious or risky activities within an organization. It identifies and categorizes prospective threats in advance using fresh threat intelligence on data that has already been gathered. Threat hunting is a relatively new application area that is very important for early detection. However, existing approaches still work on anomaly-based threat detection and overlook the rich external knowledge about threats provided by open-source cyber threat intelligence (OSCTI) [59].

##### 5.1.4.3. Attack Path Modelling

Attack path modelling is a proactive risk reducing approach that supports security teams by mapping the vulnerable routes in the network to assess risk, identify vulnerabilities, and take counter measures to protect key assets. Researchers have used AI techniques for path modelling using intrusion alerts [60] or vulnerability descriptions [61,62]. Some researchers used all cyber data, including alerts, vulnerabilities, logs and network traffic to simulate attacker/defender activities and take preventive action in real time [63, 64].

##### 5.1.4.4. Automated Risk Analysis and Impact Assessment

Automated risk analysis and impact assessment strengthen the risk management team by intelligently using the risk data available internally and externally to assess risk and related metrics in real time. AI is a catalyst to accelerate an advancement in risk management by automating the calculation of risk score [65,66], the inference of the probability of a security incident [67], the identification of key vulnerability risk indicators [68,69] and risk assessment and decision analysis [70–72] using log data and threat intelligence within and outside the organization.

##### 5.1.4.5. Predictive Intelligence

Predictive intelligence is intelligence that is actionable and relevant in a given context and can be used to anticipate attacks. Intrusion prediction tools are helpful in providing an active defence against future attacks by predicting the type, intensity and target of an intrusion in advance. Researchers are using deep-learning [73–76] approaches to forecast the alerts from malicious sources [73] or on a given target [74–76] using the sequence of previous alerts [73], historic spam e-mail [74], and network traffic [75,76] data.

Malware prediction involves methods to predict and block the malicious files before they execute their payload completely, to prevent malware attacks rather than remedy them. In this direction, Rhode et al. developed a malware prediction model based on a recurrent neural networks (RNNs) model to predict malicious behaviour using machine activity data [77].

Attack prediction is deemed to have excellent potential for proactively advancing cyber resilience. Researchers present attack prediction schemes by utilizing different types of data retrieved from news sites and websites [78], dark web forums [79], national vulnerability databases [79], incident reports [79], and common vulnerabilities and exposure databases [80].

#### 5.1.5. Risk Management Strategy

A risk management strategy assists the operational risk decisions by establishing the priorities, risk tolerance and constraints. It needs to ensure that the acceptable risk levels are established and documented along with the reasonable resolution times and investment. AI has the potential to transform this category by automating the following activities.

##### 5.1.5.1. Decision Support for Risk Planning

Cybersecurity risk planning involves the implementation of a desired portfolio of countermeasures within a predetermined budget. Formal decision support systems [81–83] and attack graph modelling [84] can help security planners make economic comparisons with the cost of countermeasures and available risk budgets.

The decision-making problem in cybersecurity risk planning is important due to the sensitivity of the risk plan to the decision maker's attitude towards risk and its interplay with the budget available. Thus, the implementation of a decision support system for estimating an uncertain risk faced by an organization under cyberattack, factoring uncertain threat rates, countermeasure costs, and impacts on its assets is very important. In this direction, Rees et al. [81] used a genetic algorithm to find the best combination of countermeasures to block or mitigate security attacks, allowing the user to determine the preferred trade-off between the investment cost and the resulting risk. Paul & Wang [82] and Paul & Zhang [83] have used robust optimisation to investigate the optimal balance between the prevention, detection and containment safeguards to deal with cybersecurity uncertainty. Zheng et al. [84] used the attack graph model for the identification of a portfolio of security controls to reduce risk. Their model is utilized to choose the best possible set of controls to ensure that the overall cost does not go above the organizational budget.

#### 5.1.6. Supply Chain Risk Management

Supply chain risk management supports risk decisions specifically related to identifying, assessing and managing supply chain risks. The effective management of cybersecurity risks in a supply chain requires a comprehensive view of the threats and vulnerabilities, cost-effective supply chain risk planning strategies, and an assessment of the cyber resilience of the supply chain. Researchers are actively using AI techniques to automate threat analysis and prediction [85], optimal cybersecurity investment [86–88], and an assessment of the cyber resilience [89] of the supply chain.

##### 5.1.6.1. Cyber Supply Chain Security

Cyber supply chain security requires a secure integrated network between the incoming and outgoing chain's subsystems. Therefore, it is essential to understand and predict threats using both internal and threat intelligence resources to limit the disruption of the business. Yeboah-ofori et al. integrated cyber threat intelligence data and used machine learning techniques to predict cyberattack patterns on cyber supply chain systems [85].

Optimizing cybersecurity investments is an important area in the Industry 4.0 supply chain cybersecurity to quickly detect, mitigate and balance the impact of security breaches with the available budget. In this direction, Sawik [86–88] proposed different models to determine an optimal cybersecurity investment with a limited budget and a portfolio of security controls to balance the cybersecurity in the supply chain.

An assessment of the cyber resilience of a supply chain is a crucial task to make the supply chain safe from cyber intrusions and to secure a competitive business advantage. In 2021, Rahman et al. [89] proposed an integrated and comprehensive approach based on Dempster-Shafer (D-S) theory as a methodology for building a framework for evaluating the cyber resilience of an additive manufacturing supply chain.

### 5.2. Protect

The protect function helps plan and implement appropriate controls to limit or contain the impact of a potential cybersecurity event. This includes a number of technical and procedural controls to proactively protect against internal and external cyber threats. AI can improve the resilience of the system by authenticating users, devices and other assets, monitoring the user behaviour, automated access control, adaptive training, data leakage prevention & integrity monitoring, automated information protection and processes and provision of protective solutions to proactively secure the system. A summary of each primary study focusing on the protect function is provided in Table 5. Solution categories along with a detailed overview of the AI use cases in each category are presented below.

#### 5.2.1. Identity Management, Authentication and Access Control

Identity management, authentication and access control is responsible for limiting the access to assets and associated facilities to authorized users, processes or devices, and to authorized activities. AI can be used for the management and protection of physical and remote access using intelligent user authentication, intelligent device authentication, automated access control using authorizations, and access permissions to prevent unauthorized access and its consequences.

##### 5.2.1.1. AI-supported User Authentication

AI can improve user authentication with physical biometrics [90], behavioural biometrics [91–94], or multi-factor authentication [95,96] instead of easily compromisable usernames, passwords and even one-time text tokens.

Physical biometrics refers to the innate physical characteristics of users that can be used for identification such as fingerprints, iris and bio-signals. In 2020, Siam et al. presented a PPG (photoplethysmography) based biometric human authentication system using deep learning [90].

In contrast, behavioural biometrics are related to the uniquely identifiable and measurable patterns in human activities that can provide continuous and user-friendly security. There are several behavioural biometrics, including usage behaviour [91–93] and gait [94]. The use of behaviour patterns related to a user's interaction with its own device is the main basis of the continuous authentication systems. In this direction, Valero et al. suggested using mobile functions and usage data, e.g., accelerometer, gyroscope, magnetometer, and statistics from interactions with different applications, to determine whether the current user is the same as the one previously authenticated [91]. In 2019, Sánchez et al. designed and implemented a continuous authentication mechanism based on the behavioural profiles of users according to their interaction with different office devices for smart offices using a cloud computing paradigm and a random forest (RF) algorithm [92]. In addition, these solutions are gradually being used in federated identity management solutions, which further increases interest in them [93].

Gait authentication is a non-intrusive, transparent and continuous method of authentication in mobile devices that captures the information needed to verify the authenticity of the user as the person walks. In 2022, Alobaidi et al. [94] investigated the feasibility of gait authentication in the uncontrolled real world by using time and frequency-domain feature extraction of each gait cycle.

Multi-factor authentication is a layered approach to secure data and applications that require a combination of two or more credentials to verify the identity or login of users. Researchers [95,96] used the keystroke dynamics as a second layer of security for web-user authentication and device authentication.

##### 5.2.1.2. AI-supported Device Authentication

Intelligent device authentication is the process of authenticating devices based on their credentials or behaviour in the network to ensure the security of machine-to-machine communication. Researchers are actively working in the field of sensor identification and authentication to ensure the security of cyber-physical systems or the automotive sector. Channel [97] and sensor [98,99] imperfections are used to find the transient and steady-state parameters as an input to the machine learning model for sensor identification.

##### 5.2.1.3. Automated Access Control

Automated access control restricts system access to authorized users based on situations or their roles and regulations within an organization. Researchers are actively using AI techniques for maintenance of the access control state [100], role mining [101] and situation-aware decision making [102,103] to prevent unauthorized access and its consequences.

Role based access control (RBAC) grants access to different users based on their roles in the organization. Benedetti and Mori have proposed the use of AI techniques to update and maintain the access control state when exceptions or violations are reported [100]. They mainly work on providing an optimized plan of actions to reconfigure the RBAC state to facilitate the maintenance process. Abolfathi et al. proposed a scalable and optimal role mining approach to extract user-role and role-permission relations from existing access control lists [101].

Attribute-based access control takes into account various preconfigured attributes of characteristics that can be related to the user, environment and accessed resource. Chukkapalli et al. [102] and Leander et al. [103] tested the performance of situation-aware decision making for attribute-based access control in smart fisheries and smart manufacturing systems, respectively.

#### 5.2.2. Awareness and Training

This solution category involves the cybersecurity awareness and training provided to personnel and partners to carry out their information security duties and responsibilities in compliance with policies and procedures. AI methods can be used for adaptive and personalized cybersecurity training, awareness or recommendations through the automatic selection of content using natural language processing algorithms [104,105] or by providing a machine learning-enabled intelligent coach for solution-guiding hints [106].

##### 5.2.2.1. Adaptive Security Awareness & Training

Adaptive training and awareness are important to overcome the challenges of outdated training content, the selection of training material, and the selection of an acceptable training approach. Tan et al. [104] created an adaptive web-based learning system that receives up-to-date training content from DBpedia and provides automated content selection based on a learner's prior knowledge of information security. Nembhard et al. [105] and Gasiba et al. [106], on the other hand, help programmers by topic modelling or by using serious games techniques to recommend or raise awareness of secure coding practices.

#### 5.2.3. Data Security

Data security governs information management in line with the risk strategy for protecting sensitive information. This includes protecting data at rest and in transit, as well as managing the lifecycle of the assets that hold the information, including its decommissioning or disposal. Researchers are actively using AI techniques for data leakage prevention, intelligent e-mail protection, malicious domain blocking and reporting, and agent-based integrity monitoring to ensure data confidentiality, integrity and availability.

##### 5.2.3.1. Data Leakage Prevention

Data leakage prevention deals with the detection and protection of data breaches, exfiltration or the unwanted destruction of data. AI techniques are used for monitoring data access, data movement and user activity [107–109], automated data sensitivity detection [110,111], and advanced persistent threat (APT) detection [112–114] to prevent data leakage.

The identification of the authorized individuals and how they use sensitive information provide accurate insights for data leakage prevention by observing their concerning behaviours or activities. Researchers [107–109] are actively using AI techniques to monitor user activity to identify their anomalous behaviour in terms of a spike in activities or unusual activities by correlating the data received from multiple sources. In this direction, researchers are using an insider threat test dataset provided by CERT to provide insights for data leakage prevention using different temporal representations of user activity [107] or by daily activity summaries, e-mail contents and email network [108]. In contrast, Al-shehari and Alsowail [109] proposed a model that is only applicable for the identification of data leakage events during the sensitive period before an employee leaves an organization.

Automated data sensitivity detection is a method of identifying and classifying data by analysing, labelling and organizing the data into relevant categories (confidential, private and public) based on shared characteristics. It can empower the data leakage prevention techniques with the ability to monitor users' actions towards only particular relevant portions of sensitive data, rather than tracking all the data at all times. Alzhrani et al. [110] proposed an automated classification technique enabled by security similarity (ACESS) for mitigating the threat of sensitive data leakage from insiders. In 2021, Guo et al. [111] pointed out that sensitive information often resides in unstructured data, making unintentional data leakage easier. Therefore, they proposed a content and context-based sensitive information identification method using BiLSTM and an attention mechanism.

Advanced persistent threats (APTs) are a type of targeted cyberattack that lasts for a long time and is unnoticed by the target network's defences. The main purpose of this type of attack is to steal data rather than cause any damage. Researchers are working on the efficient capture of telemetry from endpoints, networks and clouds to integrate and analyse this diverse telemetry to uncover anomalies, indicators of compromise (IoCs) and other behaviour of interest [112,113].

##### 5.2.3.2. Intelligent E-mail Protection

Intelligent e-mail protection is a class of software solutions to prevent sophisticated e-mail focused cyberattacks. Traditionally, a spam e-mail was used as a tactic for hawking goods and services by sending unsolicited e-mails to bulk lists. Today, however, it is actively being used to spread malware, steal authentication credentials, or commit financial frauds. AI techniques are being used for automated protection against malicious spam e-mails.

Researchers are using supervised classification [114] and deep-learning based [115] techniques to identify spam in real time using dynamic incoming e-mail data, including general, view, subject, attachment, and content-related features. However, Gualberto et al. [116] and Nguyen et al. [117] confined their research efforts to phishing e-mail detection by analysing the content of e-mails.

##### 5.2.3.3. Malicious Domain Blocking & Reporting

Malicious domain blocking and reporting provides the next level of security for e-mail protection by catching any malicious network traffic resulting from opening the spam e-mail or attachment. Researchers use AI to identify suspicious websites for each DNS lookup and block access to malicious websites associated with malware, phishing, ransomware and other cyber threats.

The detection of malicious websites works by training machine learning algorithms with a rich collection of malicious and non-malicious website features. These features can be divided into four main categories: website design features [118], domain-based features [119–121], URL-based features [122,123], and hybrid features [124, 125].

In 2021, Cohen et al. [118] presented a new website categorization method to identify malware or crack websites based on the automated scraping and processing of thousands of visual and non-visual design features. Domain name-based features are very popular for the detection of malicious websites in the research domain. Researchers are using supervised machine learning models [119] and deep-learning [120,121] techniques to detect malicious domain names using classical domain-name features. Features extracted from the URL strings, including linguistic, lexical, contextual and statistical information are used to determine the malicious websites. Indrasiri et al. [122] and Vinayakumar et al. [123] provide the detection and analysis of malicious websites by using URL-based features as an input to the ensemble machine learning and deep-learning models, respectively.

Some researchers are also using hybrid features for malicious website identification to comprehend botnet detection [124] or phishing website detection [125]. These techniques use a combination of features related to domain name structure and DNS response such as resolution source, daily resolution amount, etc.

#### 5.2.4. Information Protection, Processes and Procedures

This area deals with the protection of information sources and assets consistent with the defined security policies, processes and procedures. It includes the protection of information, and the establishment, management and implementation of response, recovery and vulnerability management plans. Researchers are working on the application of AI techniques for AI-powered backup, and an AI-enhanced vulnerability management plan to maintain the processes and procedures to manage information protection.

##### 5.2.4.1. AI-powered Backup

AI-powered backup solutions are emerging to back up critical data and software components according to priorities and requirements for ensuring efficient backup. AI techniques are being used for dynamic backup scheduling [126] and optimized backup scheduling [127].

Qin et al. [126] designed a dynamic backup system with intelligent scheduling algorithms to improve the stability and predictability of the backup environment. The proposed system schedules the backup efficiently by determining which backup starts first and which storage is assigned to that backup for improving the efficiency. In contrast, Van de Ven et al. [127] used a two-dimensional Markov chain to model data backups and study the optimization of backup scheduling. At each time slot, the proposed technique examines a probabilistic backup policy to initiate the backup, regardless of the backup size.

##### 5.2.4.2. AI-enhanced Vulnerability Management Plan

A vulnerability management plan is a framework designed to proactively reduce the exposure to risk that has the potential to disrupt and impact the system. With the rise in reported vulnerabilities in recent years, it is more important to align the vulnerability management plan with the system's requirements and critical success factor. Researchers are using AI techniques to determine context-based, vulnerability risk scores and vulnerability exploitation trends to protect the assets and information systems in real time.

Context-based vulnerability risk scoring will help the analyst to prioritize the risk in the context of particular assets or information systems and enable them to take protective action. Zeng et al. [128] proposed a new risk prioritization method to assess the vulnerability risk by integrating the attacker model to capture the attacker's preference for exploiting vulnerabilities. The risk score is defined by the criticality of exploitation and the likelihood of the exploitation using the logic-reasoning engine.

A vulnerability exploitation trend will help the analyst to prioritize patching and remediation by predicting the vulnerabilities that will most likely be exploited. Researchers are using novel AI techniques to predict the exploitability [129] and solve the class imbalance problem to improve the performance of machine learning algorithms [130]. Here, Yin et al. [129] focused on the problem of vulnerability exploitation prediction using transfer learning to help experts prioritize the application of a patch. Yin et al. [130] also proposed a novel sequential batch-learning technique, called real-time dynamic concept adaptive learning, to address the concept-deviation and dynamic class imbalance issues in exploitability prediction.

#### 5.2.5. Protective Technologies

Protective technologies provide the security and resilience of systems and assets. These technologies use particular tamper-evident features to identify and deter attempts to breach, change, penetrate and extract information from the organization's assets. AI can be used to provide protective solutions in the form of log analysis tools, intrusion prevention systems, anti-virus/anti-malware solutions and protection by deception.

##### 5.2.5.1. Log Analysis

Log analysis is the process of reviewing computer generated event logs to proactively identify bugs, security concerns or other risks. AI-powered log analysis tools can automate the routine and repeated tasks to efficiently handle large amounts of distributed log data.

Bai et al. [131] tested the performance of a variety of supervised machine learning approaches for detecting the evidence of malicious remote desktop protocol (RDP) sessions using windows RDP event logs. Afzaliseresht et al. [132], on the other hand, proposed a new approach for data presentation using a storytelling technique to generate a natural language report for recognizing cyber threat information according to the users' level of knowledge.

Researchers are also working on providing solutions to solve variety and interoperability issues in log management. De la Torre-Abaitua et al. [133] and Eljasik-Swoboda and Demuth [134] worked on addressing the variety issue using intelligent methods for extracting and processing textual data from different sources for the acceptable log feature representation with the aid of information retrieval approaches. Similarly, Sisiaridis and Markowitch [135] worked on the security analytics of the heterogenous log data derived from different network sensors by employing automated feature extraction and feature selection techniques.

##### 5.2.5.2. Intrusion Prevention System

Intrusion prevention systems monitor the network traffic and then take an appropriate action to thwart the attack by reporting, blocking, dropping or resetting the connection. Researchers have proposed unsupervised isolation forest [136] and self-organizing incremental neural networks and SVM based intrusion prevention systems [137] for embedded systems in automotive electronics and IoT networks, respectively.

##### 5.2.5.3. Anti-virus/Anti-malware Solutions

AI-powered anti-virus/anti-malware solutions can analyse thousands of files and extract useful features to classify them as benign or malware. Researchers have created anti-virus programs for detecting malware using the features retrieved from the executables [138] or dynamic data analysis [139] as an input to artificial neural networks (ANNs) or recurrent neural network (RNN) models, respectively.

##### 5.2.5.4. Protection by Deception

Protection by deception is an advanced technique to protect critical documents after an attacker has penetrated the network. AI has been used to generate credible fake text documents to mislead cyberattacks. Karuna et al. [140] proposed the creation of decoy files to divert the adversary away from the real target when the adversary is already in the system. Their decoy text-creation approach uses a genetic algorithm that manipulates real document's comprehensibility to hard-to-comprehend, but believable fake documents.

### 5.3. Detect

The detect function enables the timely discovery of the cybersecurity events by developing and implementing appropriate activities to identify their occurrence. This function is crucial for the security as prompt detection will minimize the disruption. It includes activities for the timely detection of intrusions and anomalies along with the impact assessment, implementation of security continuous monitoring to verify the effectiveness of protective measures, and appropriate maintenance of detection processes to ensure the awareness of cyber events. AI can improve the detection speed by monitoring the internal and external information sources and swiftly correlating this information to detect the unusual activities to minimize the repercussions. Table 6 presents a summary of the main contribution of each research study to the detect function, along with the details of the solution category, AI use cases and the AI domain used. The solution categories along with a detailed review of the AI use cases are provided below.

#### 5.3.1. Anomalies and Events

The solutions in this area address the detection and classification of anomalous activities by establishing and managing baselines for operations and dataflows collected from multiple sources. These baselines are then used to detect and analyse events to understand attack targets and methods.

##### 5.3.1.1. Intrusion Detection System (IDS)

An IDS is a set of tools and techniques to monitor a system and network traffic to analyse the anomalous and suspicious activities, with the aim to detect possible intrusions targeting the system. In the state-of-the-art research, IDS was implemented from three perspectives: binary classification, multi-category classification or both. Binary classification assumes two labels: normal and attack. Multi-category classification, on the other hand, deals with the problem of classification into three or more classes. In the case of IDSs, the multi-category classification differentiates between different types of attacks and provides users with more information to deal with the attack. Benchmark datasets are needed for the effective development and evaluation of both binary and multi-category intrusion detection systems. Therefore, only those studies that used benchmark datasets to evaluate their approach are included in this review.

In this direction, researchers used the ADFA-WD and ADFA-WD: SAA datasets for system call-based IDS [141], Aegean Wi-Fi (AWID) wireless networks dataset [142,172,184], BGP RIPE dataset for routing information services [143], datasets provided by the Canadian Institute of Cybersecurity [151-153,178,180-184,192-194], CIFAR-10 dataset of images [147,148], CTU-13 dataset for various botnet scenarios [149, 150], Ethereum classic dataset depicting attacks on an open-source blockchain-based distributed computing framework with a smart contract [151], ICS Cyberattack gas-pipeline dataset [152,153,178,188, 189], KDD99 and NSL-KDD datasets of network traffic records [146,148, 154-160,168,176,177,179,180,182,184,186,187,190-192,194], Coburg intrusion detection datasets (CIDDS) of labelled flow-based datasets from anomaly detection [156], UNSW-NB15 dataset of raw traffic files for different types of attack [155,157,158,160-163,176,190,191], BOT-IoT dataset of normal and botnet traffic in an IoT network [157, 183], benchmark dataset of Hadoop logs for log-based anomaly detection [164], SEA dataset for behaviour logs of Unix users [165], Secure water-treatment dataset (SWaT) of network data gathered from different sensors and actuators in water-treatment plant [153,166,167,178], UGR'16 dataset of well-labelled traffic collected from tier-3 internet service provider [168], DARPA'99 dataset with an online and offline collection of real/synthetic samples in an experimental environment [169], UCM 2011 dataset with the real traffic traces [169], and TON_IoT dataset for new generations of Industry 4.0/IoT, Industrial internet of things (IIoT) [170].

Binary classification is the basic classification type and is the most studied in the literature for the intrusion detection problem. Most researchers worked on applying different machine learning classifiers [148-152,154-164,168-173,175-177] for misuse detection, but a few also worked on solving the hyperparameter optimization of classifiers [146], the class imbalance problem in datasets [158], and feature extraction from the dataset [159,160,167,171].

In multi-category classification, the dataset contains multiple disjoint classes and the data belonging to each class are given the same label. In the multi-category classification problem, there are several other classes of traffic besides normal, including denial of service (DoS), distributed denial of service (DDoS), remote-to-local or user-to-root attacks. Multi-category classification for intrusion detection also explores the application of different classifiers [173,174,178,179,180], feature extraction problem [172,175,181,183], hyperparameter tuning of classifiers [182], and handling the class imbalance problem in datasets [176, 177].

Some researchers have used both binary and multi-category classification in their approaches [191–201]. They have proposed different classifiers for the intrusion detection problem [184-186,188-190] and address the class imbalance [187], three-dimensional data visualization [191] and feature extraction [192–194] problems for the datasets.

#### 5.3.2. Security Continuous Monitoring

Security continuous monitoring is real-time monitoring of information systems and assets to gain a clear insight into their environment and detect security events. AI can be used to automate monitoring by providing security intelligence using a dynamic, heterogenous information network that will process the logs of data generated from the monitoring of physical environments, networks, service providers, users and systems containing sensitive information.

##### 5.3.2.1. Security Monitoring

Security monitoring is a process that involves the collection, analysis and presentation of data from a variety of sources, with the aim to develop a universal solution to reveal the perpetrator's modes of operation and intentions. In this direction, researchers are actively working on processing and correlating data from heterogeneous sources [195,196] and situational awareness [197–200] for understanding security information.

An important problem in this area is processing massive, dynamic and heterogenous security information from an evolving collection of sources and algorithms. Thus, AI techniques are being used for a detailed analysis to track the associated security events in a fine-grained and reliable way. Grammatikis et al. presented a security information and event management system specifically tailored for the smart grid to detect, normalize and correlate cyberattacks and anomalies against a range of smart-grid application layer protocols [195]. Similarly, Fausto et al. [196] focused on the integration of logs belonging to both the physical and cyber domains and correlated their data together to detect potential anomalies in critical infrastructures.

Situational awareness provides a holistic and specific view of large-scale networks to enable security analysts and researchers to identify, process and comprehend information in real time. For this, Kodituwakku et al. [197] introduced a platform to process and visualize real-time, large-scale network data to not only monitor and study network flow data, but also to develop novel analytics. Similarly, Nikoloudakis et al. [198] presented an automated, situational awareness platform that uses real-time awareness features provided by the software-defined network (SDN) paradigm to perform a vulnerability assessment on network-enabled entities, their assignment to a connectivity appropriate slice and the continuous monitoring of the underlying infrastructure. Researchers [199,200] are actively working on maintaining holistic situational awareness (cyber and physical systems) in cyber-physical systems due to the tight integration of cyber and physical systems in mission-critical applications.

#### 5.3.3. Detection Processes

The detection processes involve activities to ensure the maintenance and readiness of detection procedures to reliably provide the threat intelligence and awareness of cybersecurity events. This involves activities to continuously improve and test the detection processes for efficient working. AI can be used to provide proactive vigilance on the internet using automated threat intelligence extraction from various web and internal resources. The resources include the dark web, threat intelligence sharing platforms and honeypots. The following use cases detail the use of AI techniques for the maintenance of detection processes.

##### 5.3.3.1. Dark Web Investigation

A dark web investigation is a process that monitors internet resources in the dark web related to cybercrime. This process continuously monitors criminal forums and the black market to detect illegal activities and take appropriate measures to minimize risk. Researchers perform a dark web investigation by making a sentiment analysis of textual data from dark web forums [201,202], threat intelligence using dark web data [203–205], and identification of key attackers, their assets and areas of expertise [206,207].

Automated analysis tools are needed to identify the potential threats by analysing the language and targets of hackers without manually monitoring the large volume of posts made on the dark web. Sentiment analysis is used to automate the mining of opinion, views and emotions from the text using natural language processing (NLP). In this direction, a bilingual lexical resource (BiSAL) for the sentiment analysis of English and Arabic texts related to cyber threats, radicalism and conflicts was reported by Al-Rowaily et al. [201]. Deb et al. [202] constructed a methodology for predicting malicious cyber events by exploiting the behaviour of malicious actors via a sentiment analysis of posts on hacker forums. These forums on both the surface web and dark web have some predictive power that can be used as signals outside the network to predict attacks using time-series models.

Proactive threat intelligence is identifying and addressing the security risks before an attack occurs by collecting information from hacker forums and marketplaces offering products and services focusing on malicious attacks. Ishikawa et al. [203] presented a machine learning scheme to track attack activities and the evolution of infected devices using a dark web traffic analysis. Their analysis is based on the exploration of the underlying correlation between targeted network services, as indicated by the destination port numbers of scanning packets. In contrast, Pantelis et al. [204] and Schafer et al. [205] worked on devising specialized information retrieval techniques for the dark web to support cyber threat textual mining and business intelligence.

Exploring the discussion on dark web forums is an important problem for extracting key ideas to uncover popular topics, emerging threats, and key actors in the attacker community for the benefit of cybersecurity professionals. Researchers [206,207] have used topic modelling to extract topics, track the evolution of topics, and identify key hackers with their speciality topics and uncover their role in the underground market.

##### 5.3.3.2. Automated Assessment of Different Threat Intelligence Sources

An automated assessment of different threat intelligence sources will help extract useful information from various sources, such as vulnerability databases, twitter, news sites, incident reports, and research articles to take timely actions to ensure the overall security of the system. This involves processing evidence-based knowledge from multiple sources about threats and actors to improve security and the decision-making process. The researchers are working to solve the problem of the quantity and heterogeneity of cyber threat intelligence sources and their formats to provide actionable intelligence.

Security professionals face a basic challenge when analysing cybersecurity reports, as immeasurable amounts of cyber information are produced daily, necessitating automated information extraction technologies to facilitate data retrieval and query. In this direction, researchers [208,209] have presented innovative methods for extracting the information from cyber threat intelligence reports using named-entity recognition to help security analysts gain accurate threat information as quickly as possible.

Timely and relevant information extraction from open-source intelligence (OSINT) published daily by users, security organizations and researchers is critical for maintaining a high level of security. Twitter is an important