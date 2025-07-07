# Moving from a 'human-as-problem' to a 'human-as-solution' cybersecurity mindset

**Authors:** Verena Zimmermann<sup>a</sup>, Karen Renaud<sup>*,b</sup>

*<sup>a</sup> TU Darmstadt, Darmstadt, Germany*  
*<sup>b</sup> Abertay University, Dundee, UK & University of South Africa, Pretoria, South Africa*

---

## Article Info

**Keywords:**
- Cybersecurity
- Human's Role
- Problematization
- Socio-technical System

---

## Abstract

Cybersecurity has gained prominence, with a number of widely publicised security incidents, hacking attacks and data breaches reaching the news over the last few years. The escalation in the numbers of cyber incidents shows no sign of abating, and it seems appropriate to take a look at the way cybersecurity is conceptualised and to consider whether there is a need for a mindset change.

To consider this question, we applied a "problematization" approach to assess current conceptualisations of the cybersecurity problem by government, industry and hackers. Our analysis revealed that individual human actors, in a variety of roles, are generally considered to be "a problem". We also discovered that deployed solutions primarily focus on preventing adverse events by building resistance: i.e. implementing new security layers and policies that control humans and constrain their problematic behaviours. In essence, this treats all humans in the system as if they might well be malicious actors, and the solutions are designed to prevent their ill-advised behaviours.

Given the continuing incidences of data breaches and successful hacks, it seems wise to rethink the status quo approach, which we refer to as "Cybersecurity, Currently". In particular, we suggest that there is a need to reconsider the core assumptions and characterisations of the well-intentioned human's role in the cybersecurity socio-technical system. Treating everyone as a problem does not seem to work, given the current cyber security landscape.

Benefiting from research in other fields, we propose a new mindset i.e. "Cybersecurity, Differently". This approach rests on recognition of the fact that the problem is actually the high complexity, interconnectedness and emergent qualities of socio-technical systems. The "differently" mindset acknowledges the well-intentioned human's ability to be an important contributor to organisational cybersecurity, as well as their potential to be "part of the solution" rather than "the problem". In essence, this new approach initially treats all humans in the system as if they are well-intentioned. The focus is on enhancing factors that contribute to positive outcomes and resilience. We conclude by proposing a set of key principles and, with the help of a prototypical fictional organisation, consider how this mindset could enhance and improve cybersecurity across the socio-technical system.

---

## 1. Introduction

Security incidents that endanger the confidentiality, integrity and availability of information abound, and are currently at an all-time high (Kroll.com, 2018). For example, IBM X-Force (Alvarez et al., 2017) tracked over 600 million leaked documents in 2015 and more than four billion in 2016. Other recently-reported breaches include Yahoo (Weise, 2016), LinkedIn (Schuman, 2016), Last.fm (Mannes, 2016), Equifax (Yurieff, 2017) and Marriott (Forbes, 2018). In October 2016, the Mirai botnet caused Internet-wide disruptions of major sites such as Etsy and Twitter (Antonakakis et al., 2017). Such events cost organisations and countries a great deal of money (Ponemon Institute, 2017; Rodionova, 2017), threaten critical infrastructures (ICS-CERT, 2016) and disrupt individuals' lives (Fae, 2018). Many organisations are trying to find better ways to prevent incidents and halt the seemingly unhindered success rates of hackers (McAlpine, 2018). As the whole world grapples with these issues (Sobers, 2018), and cyber incidents continue to occur, there is a need to examine and question our existing mindset in terms of how we respond to this situation. Constructing a meta-view of cybersecurity and questioning the underlying assumptions might help generate new and helpful insights which can lead us down more effective paths, in terms of improved cybersecurity.

The aim of this research is to uncover characterisations of "the problem" in the cybersecurity arena. By so doing we want to reveal the underlying assumptions of this characterisation and to derive new reference points for improving cybersecurity. Our approach was governed by the research questions depicted in Fig. 1, applying an interrogation technique called "problematizing" (Bacchi, 2012). References to applicable sections and figures are contained within the diagram.

The problematization approach, detailed by Bacchi (2009), is a way of questioning unstated and widely-accepted assumptions about a given field. It helps us to reconsider the veracity of existing characterisations of what is viewed as the underlying "problem". It is important to do this, because solutions are developed based on this conceptualisation of the problem space. Bacchi cites Foucault (1991), who explains that problematization is concerned with how people govern themselves. He argues that we can strive to reveal truth about such governance by looking at general practice in an area. We can interrogate the area to find out what is said and what is done to reveal unstated yet commonly-held beliefs.

To illustrate the potential of this approach, consider knife crime. Shackle reported, in 2005 (Shackle, 2018), that the WHO considered Glasgow to be the murder capital of Europe, with more than 1000 people being treated every year for serious facial trauma as a consequence. Solutions, up to that point, had focused on using the criminal justice system and active policing to address the issue (BBC, 2005). Leyland and Dundas (2010) pointed towards deprivation and inequalities to explain this phenomenon. Karen McCluskey from Strathclyde Police was the first to suggest that the problem was actually not a criminal issue, but rather a public health issue (Bulman, 2018). Health issues are treated by curing them, not policing them, and the solutions McCluskey proposed aligned with the public health perspective. This new approach has paid off, dramatically reducing knife crime in Glasgow and across Scotland over the last decade (O'Hare, 2018; The Economist, 2018). Re-problematizing changed perspectives about what the problem really was, and encouraged deployment of solutions that aligned with the new conceptualisation that led to a welcome reduction in knife crime.

In a field that is as complex and dynamic as cybersecurity, it is crucial for us to uncover and question what is viewed as the "problem" and not uncritically to accept existing wisdom in this respect.

Socio-technical systems, which is essentially what cyber systems are, are made up of multiple interconnected components, including human actors, technology and processes (Fig. 2). On the component level, additional factors such as governance practices, organisational hierarchies and interactions between components come into play. All of these are further impacted by, and interact with, the outer environment and legislative constraints, and the result of such complexity is that it is almost impossible to predict outcomes with any degree of certainty. System outcomes are thus emergent.

Our problematization process revealed an assumption that the individual human actor is generally considered to be "the problem" in the wider socio-technical cybersecurity system (Section 2). In Sections 2.5 and 3, we question this problem conceptualisation and review insights from the area of usable security and other disciplines, such as safety and management, that have brought about positive changes. Combining and adapting these interdisciplinary insights, we formulate new reference points and propose a different cybersecurity mindset, 'Cybersecurity, Differently' in Section 4. The approach is different from current efforts in that the human actors and their needs and limitations are not only considered in the system design, but the human is actually viewed as a solution rather than a problem. We describe examples and reflect on the challenges of achieving such a shift of mindset in security in Sections 5 and 6, and conclude in Section 7.

---

## 2. Problematization of cybersecurity

This section details our problematization process, which poses five of Bacchi's six questions (Bacchi, 2009), as depicted in Fig. 1.

### 2.1. Question 1: what is the problem?

We examined the cybersecurity-related public announcements and publications of government and industry. We also consider what hackers themselves have said about the problems they exploit. Details about how we extracted the government-, industry- and hacker-identified problems are provided in Appendix A.

#### 2.1.1. Government-identified problems (Section A.1)

Many governments have published cybersecurity strategy policies, essentially encoding what government says and what they plan to do. Those in government who develop and write these policies do so based on their implicit understanding of the "problem" that the policy is formulated to address, whether or not their conceptualisation is explicitly stated or not.

Luiijf et al. (2013) compared nineteen national cybersecurity strategies in 2013. In contrast to our approach, their analysis relied on the assumption of a common global set of threats and focused on differences in the aims and strategies formulated by governments to deal with these threats.

To contemplate governments' problematizations of cybersecurity, we had first to decide which countries' policies to analyse. A number of organisations publish Global Cybersecurity Index lists¹, but they differ in terms of what the index is based on, and countries appear in different positions on the lists.

We decided to focus on the cybersecurity policies published by the Five Eyes countries: Australia, Canada, the UK, the USA and New Zealand. This can be considered to be the world's most complete and comprehensive intelligence alliance (Tossini, 2017).

#### 2.1.2. Industry-identified problems (Section A.2)

We examined the complete security reports from the top five cybersecurity companies as ranked by eSecurity Planet². Because most reports are released annually, we analysed the most recent freely available version. The companies' whose reports we analysed included: Cisco, Symantec, Palo Alto Networks, Check Point and Microsoft.

#### 2.1.3. Hacker-identified problems (Section A.3)

How do hackers compromise systems? These are the "problems" that they exploit in order to breach system security. A few examples give us a sense of what they do and say. These were also analysed to isolate the problems revealed by their statements.

#### 2.1.4. Summary: outcome of the problematization process

The derived problems (P1 to P18) are shown in Tables 1 and 2, and depicted in Fig. 3 within the socio-technical system.

The identified problems: lack of cyber knowledge, awareness and skills (P1), lack of accountability (P2), lack of policies and compliance (P3), lack of reporting (P18) as well as malicious activities by employees inside the organisation (P6) or cyber criminals outside the organisation (P7) concern the human actors, and their behaviours, on an individual level. Entities not wanting to take or share responsibility (P5) and shortcomings in following security best practices (P4) are located at the intersection of people, organisational processes and technology.

P7 and P8 concern activities of cyber criminals and software vulnerabilities, and are located at the intersection of people and technology, as software vulnerabilities are presumably caused, overlooked or not patched by software developers interacting with technology, and exploited by the cyber criminals. Thus, these problems again implicitly concern the human actor.

Some of the problems on an individual level are echoed on a societal or governmental level, e.g. a lack of individual cyber knowledge is mirrored by a general scarcity of cyber security professionals (P9), a lack of targeted research (P16) and a lack of local innovation (P11). Individual criminal activities are reflected in hostile nations' activities (P15) and challenges in detecting and prosecuting criminals (P10). In terms of the prevention and handling of cybersecurity incidents on a governmental level: a lack of leadership (P14), a lack of communication and collaboration (P12), a lack of trusted advice (P17) and problems in people reporting (P18) and appropriately responding to incidents (P13) are identified. The governance bubble influences and interacts with the core socio-technical system.

The challenges of detecting criminal activities (P10) and responding to incidents (P13) are located at the intersection between governance and technology. In organisations, the initial detection and handling of abnormal or malicious activities depends largely on technological measures such as firewalls or intrusion detection systems that warn human operators and forward information for further processing.

To conclude, almost all of the identified issues in cybersecurity concern human actors in their various roles in some way, e.g. as software developers who create and maintain security-related technology, policy makers who introduce laws and standards, as well as employees and end users that make use of security-related technology while targeting other work-related or private goals. In the following, we will use the term "human actor" to acknowledge the variety of knowledge levels and roles of people in general, as compared to focusing solely on one particular role.

The problems at the governmental level are mainly concerned with preventing, controlling or responding to the problems at the individual level, such as lack of knowledge, skills and awareness, but also malicious behaviours. Even the problems that can be attributed to technology or processes are indirectly related to human behaviours. Human actors are using outdated technology, overlooking software vulnerabilities, falling for phishes, not following security policies and not sharing responsibility. The conclusion is that the human actor is viewed as the primary security risk and thus a "problem" to be dealt with.

### 2.1.5. Related research into the human in the cybersecurity area

Because the focus of this research is on the role of the human actor in the socio-technical system, we provide a brief overview of human-centred research in the cybersecurity area. Research focusing on technical aspects is not reviewed.

A study carried out in 2017 analysed a decade's publications in major human-centred security conferences, in terms of whether they focused on the individual, on social aspects of human-centred security, or on their greater role in the socio-technical system (Renaud and Flowerday, 2017). The researchers discovered that the majority of papers focused on the individual, with a very small number focusing on social aspects or on the bigger picture. The primary focus was the human-computer interaction layer in Fig. 2 i.e. the individual human actor's role in cybersecurity.

That being the focus, what aspects do academics study? Wood and Banks considered human error to be the most frequent cause of adverse incidents and "a serious threat to the viability of computer-based systems, and thereby to the industrialised world at large" (Wood and Banks Jr, 1993, p.51). Some say that the average computer user simply lacks knowledge and awareness of cybersecurity issues and of the secure behaviours they ought to be carrying out (Kraemer and Carayon, 2007; Kritzinger and von Solms, 2010). Other researchers argue that a lack of knowledge is not the primary problem, but rather that users do not care about possible consequences, that they are unmotivated to take responsibility (Thomson and Van Niekerk, 2012), or merely lazy. Herley (2009) points out that the word "lazy" has traditionally been used to explain insecure end-user behaviours, although he disagrees with this characterisation.

Insecure behaviours, errors and the deployment of coping mechanisms have also been attributed to a mismatch between system design and human perception and cognition (Chiasson and Van Oorschot, 2015; Herley and Van Oorschot, 2012; Posey et al., 2014; Renaud et al., 2014; Sasse et al., 2001; Wood and Banks Jr, 1993). Researchers in the relatively young field of usable security have focused on improving usability and coming up with solutions to design issues (Adams and Sasse, 1999; Balfanz et al., 2004).

In their seminal paper Whitten and Tygar (1999), for example, identified usability issues as a primary reason for users not being able to encrypt emails. Disappointingly, more recent studies on encryption found that despite a great deal of research in the interim, people are still struggling to encrypt emails (Ruoti et al., 2016; 2013).

### 2.2. Question 2: what effects are produced by this representation?

Having identified the humans within the socio-technical system as a "problem to control", it is understandable that matching solutions to deal with the human would be deployed. Governments strategise, enact legislation and provide resources to drive change. On an operational level, the actions of organisations to address the "human as problem" include:

**Exclude:** Industry experts suggest excluding the human from the system as much as possible, suggesting automating of security processes or making them invisible. Cisco suggests that "automation and intelligent tools [...] can help overcome skills and resource gaps." [p.10] (Cisco, 2018). A Verizon report puts it even more directly by stating: "Automate anything you can as this reduces the human error associated with many breaches we see" [p.36] (Widup et al., 2018). Some academics agree with this sentiment (Vidyaraman et al., 2008).

**Educate & Train:** Standards bodies, such as NIST (National Institute of Standards and Technology, 2014), academic researchers (McIlwraith, 2016; Øien et al., 2010) and industry (Alvarez et al., 2017; Check Point Software Technologies Ltd, 2018; Cisco, 2018; Hatekar et al., 2018; Symantec Corporation, 2018; Widup et al., 2018), highlight the necessity of training, manuals and security awareness campaigns. Consequently, many drives exist to increase security knowledge and awareness (Bulgurcu et al., 2010; Siponen, 2000). Other approaches focus on making people care e.g. by inducing fear of negative consequences (Vance et al., 2013) or goal-setting (Thomson and Van Niekerk, 2012).

**Use Policies to Control & Constrain:** Organisations implement a number of measures to control and prevent the insecure actions of human actors (Daugherty, 2016; Rayome, 2017). The most widespread of these is the formulation and enforcement of security policies (Bauer et al., 2017; Kritzinger and von Solms, 2010; Siponen et al., 2010; Sobel et al., 2007). The aim is to ensure that the human actor behaves securely, as instructed by the policies (Alvarez et al., 2017; Cisco, 2018; Palo Alto Networks Inc., 2018; Peltier, 2016; Widup et al., 2018).

**Conduct Root Cause Analyses:** In many cases, in the aftermath of a new breach, a root cause analysis is carried out (Andersen and Fagerhaug, 2006; Bagian et al., 2002; Blickstein et al., 2011). There is often a great deal of hindsight-enabled finger-pointing (Carman, 2015; CIO Staff, 2006a; Ismail, 2017; Keane, 2015; Shinder, 2016). If there is sufficient public outrage, it is likely that someone will have to be held accountable and punished (BBC, 2016), before the media moves on to another story (Horowitz and Wiener-Bronner, 2017; Isaac et al., 2017; Reuters, 2016; Russell, 2017). The breached companies themselves sometimes terminate a single employee's employment, or at least pressure them to resign (CIO Staff, 2006b; Donnelly, 2015; Reuters, 2017; Swisher, 2017), perhaps to show how serious they are about rooting out the negligent person behind the breach. Often, the response to adverse events is to re-train all employees, or to create more policies and processes to regulate human behaviours (Arthur, 2018; Renaud, 2014).

In conclusion, the "human-as-problem" mindset manifests in measures that exclude the human or constrain human behaviour by requiring compliance with security policies. Efforts to increase awareness and knowledge are redoubled.

### 2.3. Question 3: what assumptions have been made?

To derive the assumptions behind the conceptualisations, we examine the identified problems and proposed solutions.

First, the outcome of our problem conceptualisation (Fig. 3) indicates that the human in the system is the cause of cybersecurity errors and adverse events. We shall refer to this as "Human as Problem".

Second, the review in Section 2.2 shows that the "human as problem" should be dealt with by: (1) excluding the human from the system (Cisco, 2018; Widup et al., 2018), (2) educating and training where exclusion is infeasible (Alvarez et al., 2017; Check Point Software Technologies Ltd, 2018; Cisco, 2018; Hatekar et al., 2018; Symantec Corporation, 2018; Widup et al., 2018), and (3) requiring compliance with security policies (Alvarez et al., 2017; Cisco, 2018; Palo Alto Networks Inc., 2018; Siponen et al., 2014; Widup et al., 2018).

The underlying assumption is that adverse cyber events can be prevented by controlling and constraining the human actor's behaviour. We shall refer to this as "Exclude, Train, Constrain & Control".

Third, the use of the aforementioned policy-based controls relies on the assumption that it is indeed possible to encapsulate all desirable security actions within policies and organisational processes. We shall refer to this as "Policy Adequacy".

Fourth, building on the previous assumptions, it is concluded that the focus of cyber defence should be on preventing errors and adverse security events (Liginlal et al., 2009; Wood and Banks Jr, 1993). This reveals an assumption that the absence of errors denotes the presence of security. We will refer to this as "Prevent Errors"

Fifth, when an adverse cyber event occurs, a "root cause" analysis should be carried out (Ponemon Institute, 2017; Smith, 2003) (Section 2.2). The underlying assumption is that a socio-technical system can be thought of as the sum of its parts and that incidents can be traced back to a single system component. "Fixing" this component should then prevent recurrences. We shall refer to this as "System Decomposability".

Sixth, the next step, after the root cause analysis, should be to patch vulnerabilities, update or lock down devices or apply more automation and technology (Palo Alto Networks Inc., 2018; Symantec Corporation, 2018; Widup et al., 2018), in addition to tightening up security policies and measures to constrain employee behaviours (Arthur, 2018; Renaud, 2014). The assumption is essentially that security-by-resistance is the right way to go. We shall refer to this as "Resistance Stance".

The different assumptions are depicted in Fig. 4. These are essentially inter-dependent, and co-reliant.

Fig. 5 depicts the current 'Cybersecurity, Currently' mindset, based on our interpretation of the assumptions underlying identified problems. This figure depicts the three main socio-technical system components: people at the centre, using technology to carry out organisational functions, with processes encoding organisational means and methods of so doing. In this diagram, the mindset is outside-inwards: the human's behaviour is considered problematic and the organisation acts to protect themselves from the consequences of their variable behaviours. Processes exist to impose control and are regularly reviewed in order to ensure that undesirable actions are curbed. Access to data and technology is severely constrained so as to prevent insecure actions.

### 2.4. Question 4: how has this representation come about?

A comprehensive discussion of this question is out of context for this paper. However, we do suggest an explanation for the core assumption about the human actor being the problem. When organisations initially started using computers, those responsible for computer security had two concerns: (1) physical security of the machines, which were usually housed in their own space, and (2) insiders accessing or destroying data, either deliberately or inadvertently. This led to an information security approach revolving around governance, risk and compliance (GRC) (Lipner, 2015) and consequent control mechanisms such as policies, standards, and doctrines (Bebchuk and Roe, 1999; Warner, 2012). This might have created a path that entrenched itself and informed all subsequent information security endeavours (Dobusch and Kapeller, 2013).

Anecdotally, the reasoning, currently, seems to be: (1) If a hacker exploits software vulnerabilities, that is the fault of the IT staff for not keeping the system patched and secure. (2) If someone falls for a phishing message, they did not pay enough attention. (3) If a breach occurs, it is possible that someone leaked their password or chose a weak one. In this way, every adverse event can be traced back to some human's failings or malicious behaviours and the human is perceived to be the one component that gets in the way of good security.

### 2.5. Question 5: how could this representation be questioned?

#### 2.5.1. First, human as problem

The assumption that the human constitutes a problem to control is deeply rooted. Consider the Sony hack. Sony became aware of the presence and activity of malware on their systems. Hackers stole personal information about employees, emails, executive salary details, and copies of unreleased Sony films (Siboni and Siman-Tov, 2014). Sony surmised that an IT administrator's password had been stolen, perhaps because he or she had been deceived by a phishing email. Arthur (2018) reports that, on the day after the Sony attack, the FBI held information sessions during which employees were lectured about password "best practice" and spotting phishing attacks. Yet these employees did not open the door to the hackers. The hackers gained access directly via Sony's website using an exploit called SQL injection (Bright, 2011) and accessed the database that held all the user names and passwords stored in the clear. So, despite the fact that employees' behaviours did not trigger the breach, the immediate remediation incorrectly focused on their password choices and phish detection abilities, confirming unthinking attribution of a negative outcome to some human actor.

In reality, cyber incidents have multiple interacting causatives, and while the individual can indeed contribute, that is not the whole story. Socio-technical systems are complex, highly interactive and unpredictable, and adverse events have multiple contributing factors.

Moreover, contrary to being the primary source of all problems, humans can actually be a vital player in defending against attacks (Hatekar et al., 2018). Labelling human actors as "the problem" does not acknowledge their ability to detect anomalies and halt attacks.

#### 2.5.2. Second, exclude, train, control & constrain

These remediations essentially remove responsibility from the human actor and do not permit them to be part of the solution. They are reduced to being rule followers; compliance becomes the mantra. Yet compliance only enhances security if the attackers do not innovate and change strategies, and only if the system is decomposable. Both of these assumptions, however, are unrealistic (Castelli et al., 2018; Cooper, 2017) (see Fig. 2).

#### 2.5.3. Third, policy adequacy

Policies implement an unexceptionalist approach (Hopkins, 2011), applying the laws of the physical world to cyberspace. Yet cyberspace is not physical space. What is required is an exceptionalist approach that deals with cyberspace problems in a way that is better aligned with its idiosyncratic configuration and complexity.

Moreover, Cooper (2017) points to a mismatch between defender (reactive) and hacker (proactive) strategies. Policies prevent individuals from countering innovative and evolving hacker tactics.

#### 2.5.4. Fourth, prevent errors

The idea that errors can be prevented conflicts with the realities of the actual socio-technical system. Simply because errors are not making their presence felt can not automatically be interpreted as a sign that all is well.

Let us reconsider the Sony Hack. Subsequent investigations revealed widespread insecurities. Machines were not updated, people could install software downloaded from the Web, and passwords were being stored in plain text (Bort, 2014). While the 2014 attack reached the media, this was not the first time Sony was hacked. In 2011, hackers had already breached their systems using SQL Injection (Martin, 2011). This shows that Sony had systemic issues in 2011, and they were still there in 2014. These systemic flaws included inadequate governance & maintenance, and poor software engineering, among others. The huge Marriott data breach of 2018, too, was not the first successful hack — it was merely the last in a string of breaches (Brewster, 2018). In both these cases, no one noticed anything out of the ordinary, and the organisations were lulled into a false sense of security. A strategy that focuses solely on preventing and detecting errors is unlikely to detect ongoing security issues.

#### 2.5.5. Fifth, system decomposability

The Global State of Information Security Survey 2018 refers to "an increasingly complex digital society" (Castelli et al., 2018). The rising cyber interdependence of infrastructure networks is also acknowledged by the World Economic Forum (2017) as: "greater interdependence among different infrastructure networks is increasing the scope for systemic failures – whether from cyberattacks, software glitches, natural disasters or other causes – to cascade across networks and affect society in unanticipated ways" [p.7].

Root cause analyses, as a commonly deployed technique, do not acknowledge the multiple interactions and complexities of socio-technical systems. Looking for and remediating a single "root" suggests that it is indeed possible to isolate a single cause when the reality is that a multiplicity of causes often come together in an unpredictable fashion, to trigger an adverse event. A PwC report (Castelli et al., 2018) acknowledges that "organisations must dig deeper to uncover risks" [p.10] that are inherent in today's socio-technical systems with emergent propensities.

#### 2.5.6. Sixth, resistance stance

Many efforts to avoid cyber incidents focus on hardening the system. This can include adding more constraining rules to the policies (Renaud, 2014).

The current successes of hacking attacks suggest that it is impossible entirely to avoid and resist cyber attacks, so we should rather turn our attention to more equally balancing resistance and efforts to build resilience (Paz et al., 2018). Such resilience denotes the ability to recover to pre-event levels of functioning after a disturbance (Gardi et al., 2009; Hollnagel et al., 2006).

#### 2.5.7. Summary

It becomes clear, when one examines Fig. 5, that the primary focus currently is on controlling the human actor, based on the assumption that their actions are problematic, and perhaps even malicious. This might be an effective strategy, except for the fact that the cyber arena is fluid and ever-changing. Hackers evolve their techniques and technology changes at an unprecedented rate (Cooper, 2017). Relying on policies to control human behaviour and thereby to prevent all errors does not acknowledge this reality. This situation is exacerbated by the fact that the usual response to adverse events is the enhancement of policies and reinforcement of compliance efforts. As the number of attacks escalate, it seems time to consider a different cybersecurity mindset.

---

## 3. Question 6: how can the problem be thought about differently?

We first provide an overview of insights gained from other disciplines that have taken a similar meta view of their practice, before returning to our cybersecurity theme:

### 3.1. Management

In the field of management, Hart (2013) outlines the impacts of the kind of situation that is depicted in Fig. 5. In particular, he explores the consequences when the focus is on controlling the human, and on ensuring that processes are followed to ensure best practice. He also speaks about reducing the human to a "rule follower", displacing responsibility from the human actor to the rules, and, beyond that, to the process formulator and policy writer (Pham et al., 2017).

Bourdieu (1998) argues that this kind of displacement of responsibility to the policy makers drives a wedge between those who make policies, and practitioners who actually carry out the work. This could lead to practitioners disowning the problem.

The way humans are being "controlled" in cybersecurity is creating a situation where the human becomes a problem, because they are disempowered and marginalised by the controlling mindset: what systems theory calls a 'reinforcing loop'. Permitting people to take responsibility allows them to maximise their agency in terms of behaving to secure the organisation's devices and information. Moreover, Spector (1986) finds that giving people control delivers high levels of job satisfaction and performance.

### 3.2. Military

In the military, Marquet (2013), who was the captain of a nuclear-powered submarine, came to the realisation that he was creating a culture of following instead of individual leadership. Morale was low and serious mistakes were being made. He radically changed the way he ran his ship, and discovered that giving his crew ownership and control over problems, at their own level of competence, transformed his ship from the worst to the best in the fleet. This outcome was achieved by switching from controlling to trusting his junior officers and empowering them to make the best decisions at their level of expertise. At the moment, this kind of trust is almost unheard of in cybersecurity practice.

### 3.3. Safety

This field delivers many valuable insights. Their beginnings were very similar to the way cybersecurity works today. In the 1930s (Heinrich, 1959) safety equated to the achievement of zero accidents, incidents and failures. An accident was viewed as an event that "invariably results from a completed sequence of factors — the last of these being the accident itself" (Heinrich, 1959, p.13). That is why this approach is often referred to as the "Domino Model" (Hollnagel, 2014, p.64). If an event, A, invariably led to an effect, B, the system could be considered to be bi-modal and easily decomposable. An accident analysis was conducted post-hoc with the help of accident reports and event trees. Heinrich concluded that 88% of accidents were directly caused by unsafe human acts (Heinrich, 1959, p.21), i.e. human error. This is similar to the current stance in cybersecurity where post-hoc analyses are carried out to identify single root causes, assuming that the underlying system is decomposable enough to support this.

Measures to prevent accidents in safety thus attempted either to find and eliminate causes (Heinrich, 1959, p.16), or to strengthen the barriers between the linear chain of events. Examples included technological automation, enforcing strict rules, mandating use of safety equipment, awareness posters and personnel adjustments, e.g., identifying and replacing the unreliable humans that caused the accidents, the "bad apples" (Dekker, 2014c, p.1). This, too, is very similar to the way the cybersecurity field responds once they have identified the one human action that triggered an adverse event.

However, as the socio-technical safety systems developed and grew more complex over time, safety scientists realised that the previous approach was no longer fit-for-purpose. Many organisational and environmental factors and continuously changing system conditions impacted safety. Furthermore, the growing complexity of systems consisting of highly interconnected and tightly coupled components led to indeterminate behaviours (Perrow, 1981): System outcomes were emergent and often unpredictable (Dekker et al., 2011), as are those in cybersecurity systems. An event, A, no longer necessarily led to an effect, B. Instead, an event, A, sometimes led to effect C or triggered a completely unexpected reaction.

The traditional safety approach also considered people to be the weak point and human behaviour a problem to be controlled (Dekker, 2014c). Yet, an analysis revealed that the number of accidents was actually incredibly low given the complexity of the systems being studied. Examples of these studies include the US Air Traffic Control and US Navy nuclear aircraft carriers (Rochlin et al., 1998). Analysing these so-called high-reliability organisations (HROs) (Roberts, 1989), the researchers isolated particular factors that contributed to this high performance. These included high degrees of redundancy, flexibility, and deference to expertise. Employees were given an active role within the system and the freedom to react to changing system conditions.

Furthermore, the organisations demonstrated a "culture" of high reliability. This was characterised by active seeking for, and elimination of threats, and a no-blame approach where employees could report errors without fearing negative consequences, thereby allowing the organisation to learn from errors (Roberts, 1990). Even though this initial research was descriptive in nature, and the factors unsuited to widespread application, the insights marked an important milestone towards the transition to "Safety, Differently", where humans were no longer viewed as "a problem to control" (Dekker, 2014b, p.13), but rather as "a solution to harness" (Dekker, 2014b, p.235).

These researchers and practitioners from different areas independently realised that they needed to change their paradigms, and each found ways of empowering the people in their organisations. The result, in all these cases, was more of the desired outcomes, not disaster.

### 3.4. Cybersecurity

Within the area of cybersecurity initial attempts were made to steer the field away from seeing the human agent the problem or "enemy" (Adams and Sasse, 1999). These focused on improving the design of technology interfaces to enhance usability so as to align with human needs and limitations (Adams and Sasse, 1999; Balfanz et al., 2004). For example, Adams and Sasse (1999) urged interface designers to strive to understand the users' perspective and to design interfaces with the human in mind, not merely to consider them to be the cause of the problem. The relatively young field of "Usable Security" constitutes an important step towards empowering the human. Instead of excluding the human from the system, they argue that their needs and limitations should be given due consideration during system design.

### 3.5. Summary

The insights of these "human-as-solution" approaches (Dekker, 2012; Hart, 2013; Marquet, 2013) inform a new set of reference points. The novelty of the new approach lies in the fact that insights from various disciplines and approaches are combined and adapted to be applicable to the field of cybersecurity. The aim of this approach is to push the current efforts to no longer view the human as an "enemy" even further, and to foster the use of all available resources in socio-technical systems, including the human actor, to maintain and enhance cybersecurity. To fully develop the human actor's potential to be a contributor to cybersecurity, a shift in perspective is needed. We thus propose the 'Cybersecurity, Differently' mindset and describe its key principles next.

---

## 4. New reference points: key principles of 'Cybersecurity, Differently'

In the light of the ever increasing number of security incidents, we suggest adopting a new direction in the cybersecurity domain. An overview of the key principles of the new mindset that we call 'Cybersecurity, Differently' is depicted in Fig. 6, highlighting how the key principles depend on, and reinforce, each other.

'Cybersecurity, Differently' can be described as a new perspective on the human's role within complex socio-technical systems that incorporates insights from a number of related areas including Safety (Dekker, 2012; 2014b; Hollnagel, 2014; Roberts, 1989; Weick et al., 2008), Medicine (Wachter and Pronovost, 2009), Aviation (Beaty, 2010), Management (Hart, 2013) and the Military (Marquet, 2013).

Fig. 7 shows how the human in 'Cybersecurity, Differently' can be at the centre and the starting point for maintaining and enhancing cybersecurity. In this diagram, the mindset direction is inside-outwards. In the following sections, we will explain how humans can be made part of the solution instead of being a problem to be controlled.

### 4.1. Socio-technical systems — decomposable vs. emergent

This assumption needs to be refuted at the outset, because it serves as foundation for the other assumptions enumerated in Section 2.3. While assuming decomposability is enticingly simple and supports the deployment of traditional tools, such as root cause analyses, it is also naïve in the face of cyber reality. As such, it can no longer be supported unquestioningly, given the complex, inter-dependent and evolving nature of cyber socio-technical systems.

In reality, the emergence of any behaviour, including errors or accidents, is a consequence of an interplay of different factors that interact and conspire together (Hollnagel et al., 2006, p.13).

The WEF 2017 Global Risks Report found that cyber attacks, software glitches, and other factors could spark systemic failures that "cascade across networks and affect society in unanticipated ways." (World Economic Forum, 2017, p.5). This suggests that the idea of flattening a socio-technical system and considering it the simple sum of its parts does not do the true situation justice. The system becomes more than the sum of its parts: creating interconnectedness, complexity and unpredictable, emergent outcomes. 'Cybersecurity, Differently' acknowledges the complexity, unpredictability and interconnected nature of socio-technical systems, with many dynamically interacting elements. Such elements include computers, networks, human actors in different roles and with different levels of security expertise, governance structures, operating systems, and the influences of the wider environment.

Adverse security events do need to be addressed and remedied. However, assuming decomposability and then focusing attention solely on one component of a complex socio-technical system is unrealistic, given the emergent nature of the underlying system's outcomes.

From this, we propose a more nuanced underlying assertion that:

→ **Today's socio-technical systems are complex and the outcomes thereof emergent, indeterminate and unpredictable.**

### 4.2. Human as problem vs. human as solution

'Cybersecurity, Differently' considers the human as integral and indispensible to the functioning of the socio-technical system as the facilitating technology. As such, they are indispensable contributors to security. We are not the first to suggest this kind of paradigm shift (Carroll and Edmondson, 2002; Dekker, 2014a; Hart, 2013; Hollnagel, 2014; Marquet, 2013); here we encapsulate the new mindset in a set of principles that apply to cyber security, extending the ideas proposed by other researchers (Brostoff and Sasse, 2001; Pfleeger et al., 2014), who also make the case for applying insights from safety to cybersecurity.

Our proposed new mindset does not assume that humans do not make mistakes. Instead, it acknowledges that error and success are two sides of the same coin and that either label can only be assigned in hindsight (Hollnagel, 2014). Human performance variability might well contribute to errors, but, more importantly, also contributes to normal operation or success in the majority of instances (Hollnagel, 2014). Constraining humans or excluding them from the system means that we limit mistakes, but also that we limit all human agents' capacity to contribute actively to maintaining and improving security. Human actors should be allowed to participate in security efforts. Burkhead (2014, p.114) notes that "The detection and identification of incidents is heavily reliant on human reporting or human-assisted reporting".

In the cybersecurity arena, the Microsoft report recognises that humans are often called the weakest link in security but also that "with the training and education they can also be the first line of defense" [p.20] (Hatekar et al., 2018). As an example they describe how employees spotting and reporting a suspicious mail can halt phishing attacks. A Verizon report (Widup et al., 2018) also finds that in a normal organisation 78% of employees do not fall for a single phish all year, showing how employees are often successful in spotting phishing emails. Because the focus is usually on errors, this important fact is not celebrated or highlighted. Moreover, by focusing on the negative aspects of human behaviour - errors - we demonise the human agents in the system and curtail their ability to play a positive role.

The mindset change we are advocating requires us to move on from focusing on the negative aspects of variability in human behaviour to realising that such variability is actually a strength that can be our greatest ally in cybersecurity. Moreover, embracing the human as the solution requires us to accept that the overwhelming majority of human actors within a socio-technical system have the intention to "do a good job" rather than to commit errors (Dekker, 2012, p.99) (This excludes malicious human actors). This requires us to abandon knee-jerk negative characterisations, and rather to acknowledge that the majority of employees are trying to do their best in a complex and challenging environment.

Following this line of argument, we derive the first principle of 'Cybersecurity, Differently':

→ **Principle A: Acknowledge the Human Actor's Ability to be Part of the Solution**

### 4.3. Policy adequacy vs. deference to expertise

"Deference to expertise" means that, regardless of hierarchy, the person with the highest level of expertise for the task in hand should be part of any decision process (Dekker, 2014b).

Cybersecurity expertise is important. However, human actors in socio-technical systems are not only IT specialists, administrators and software developers with high security expertise, but also all other human actors as "end users" with less expertise in security, but a great deal of expertise in their chosen profession. 'Cybersecurity, Differently' suggests that even human actors with minimal security expertise should be recognised as task experts. These are those who can best describe their tasks, their specific goals, the processes they engage in and identify the factors influencing these (e.g. time constraints). They should thus be actively involved in decision processes and the future development of cybersecurity mechanisms. Appropriate security measures should be derived jointly by security experts and the relevant task experts, instead of the former imposing security measures. Thus, the person with the highest level of expertise for a certain task, e.g. the IT staff in case of a security threat, should be involved in making decisions even though they might be ranked lower than the managers who make budgetary decisions. This helps to transfer security expertise to non-experts and align security processes with the human actors' context and tasks.

For example, Kirlappos et al. (2013) found that the main reason for non-compliance with security policies was that security conflicted with productivity. They concluded that the employees, as task experts, are the principal agents in deciding how security should be implemented in their specific contexts.

This new reference point is encapsulated in the next principle:

→ **Principle D: Defer to Expertise**

### 4.4. Exclude, train, constrain, control vs. encourage learning, communication and collaboration

We suggest that, when considering an adverse event, researchers and practitioners should focus on the 'why', instead of on the 'who' (Dekker, 2012). Organisations should always act to learn from errors and encourage risk-free reporting rather than focusing on punishing individuals (Castelli et al., 2018; Dekker, 2012). All components of socio-technical systems can benefit from highlighting positive as well as negative events. To learn from events, and to be able to react quickly, reporting is essential. However, reporting is unlikely if employees or customers fear negative consequences such as blaming, shaming, financial loss, prosecution or job loss.

Safety scientists suggested establishing reporting systems that explicitly protect the individual (Dekker, 2009) and focus on the 'why'. Apart from errors or failures, the protected reporting of so-called "near misses" should be encouraged (Beaty, 2010). These are actions or situations that have the potential to go wrong but have not (yet) resulted in negative consequences. Similar approaches would also be feasible in the security area. Advantages include an extended quantitative database, the maintenance of a desirable level of alertness, and fostering insights into potentially insecure actions and situations (Van der Schaaf et al., 2013).

Edmondson (2004) explores the challenges of changing reference points in this way, and says this can be achieved by "an environment of psychological safety that fosters open reporting, active questioning, and frequent sharing of insights and concerns" [p.ii3]. Edmondson carried out a case study within a hospital and found that, by good leadership, learning was empowered and supported, changing the focus from error-detection and -prevention to learning and celebration of successes.

Furthermore, we suggest approaching cybersecurity incidents proactively, as compared to merely reacting to past cybersecurity incidents. Hudson (2003) explains that a proactive approach, as opposed to a reactive approach, can engender high reliability in an organisation. Hollnagel (2008) advises that the barriers to protect a system from threats must not become entirely reactive because safety cannot genuinely be improved by only looking into past events.

The proactive handling of, and learning from, incidents is summarised in the principle:

→ **Principle E: Encourage Learning.**

Learning from incidents and experiences can be fostered by communication and collaboration: There are two aspects to be considered here: (1) collaboration between humans and technology, and (2) communication between different human actors.

**(1) Collaboration between humans and technology:** Machines outperform humans in some areas and humans outperform machines in others. For example, humans are better at pattern recognition, improvisation, and decision-making with incomplete information. Machines, instead, are better at repeating tasks with high precision and speed or error-free retention of meaningless information. One approach to function allocation is HABA-MABA: Humans are better at, Machines are better at (Dekker and Woods, 2002; Fitts et al., 1951) that highlights the fact that humans and machines have different strengths and weaknesses.

There is no suggestion that automation is always a bad idea, nor is it feasible to shift from "blaming" humans for errors to "blaming" technology or automation. Instead, we acknowledge that there are areas where automation is important, but there are also areas that cannot, or should not, be automated (Beaty, 2010). Instead of automating the human out of the system, 'Cybersecurity, Differently' suggests that every member of the wider socio-technical system be treated as an equal partner instead of mere substitution. It encourages the harnessing of both partners' strengths to create a sense of synergy or "team-work". Using automation in a way that excludes the human from the system might lead to misunderstandings, security failures, or "automation surprises" (Sarter et al., 1997) between those involved in an interaction. We therefore argue that when processes are automated, humans ought to be kept in the loop so that they can interact with the systems and extend their own expertise too (Ruoti et al., 2016).

**(2) Communication between human actors:** Communication between humans and technology and between different human actors is essential. It starts with the communication within work teams, but also between different organisational departments and with humans outside the organisation, such as customers or cooperating partners. PwC, for example, also calls for leaders in industry and governments to work together across national borders to identify and target cybersecurity threats and increase resilience (Castelli et al., 2018). The communication about cybersecurity should not only include experiences of handling threats and adverse events, but also the sharing of success stories that can be beneficial in deriving lessons for improving resilience.

From this, we derive the principle:

→ **Principle C: Communicate & Collaborate.**

### 4.5. Prevent errors vs. focus on successes

The 'Cybersecurity, Differently' mindset focuses on successes and normal operation, the large majority of events that "go right" (Hollnagel, 2014). Similar to the safety area, the focus in security has long been on adverse events and human errors, which emerges from our review. Even though it is still important to analyse adverse events, we believe that organisations and researchers can learn a lot by changing their perspective to also learning from successes and near misses (Tinsley et al., 2011): what are people doing right that assures the security of an organisation's information?

In the large majority of cases, the same factors that contribute to an error or accident also contribute to the safe functioning of the system so that the label "error" or "success" can only be awarded in hindsight (Hollnagel et al., 2006, p.13). Dekker, for example, found that the same factors, e.g. work-arounds and deviations from procedures, in a few adverse events in the health care sector contributed to successful patient care in the large majority of cases (Dekker, 2018). It is thus important to evaluate both sides of the coin, negative and positive outcomes, before appropriate measures can be identified to enhance, facilitate, or communicate factors that contribute to cybersecurity.

The PwC report also suggests that organisations should "pursue resilience as a path to rewards – not merely to avoid risk." (Castelli et al., 2018, p.12). This indicates a call for a shift in focus from avoiding the negative to increasing positive outcomes. While this might not sound too different, the change in perspective influences the evaluation of outcomes, the measures undertaken to deal with them and also the type and proportion of analysed events. While incident or accident analysis conducted to avoid threats focus on the small percentage of adverse events, also analysing near misses and positive outcomes enlarges the database by including myriad "normal" events. This allows for statistical analyses often not possible with small numbers of negative incidents and a comparison of factors influencing positive vs. negative outcomes.

The MITRE Corporation, for example, embraced this idea (MITRE Corporation, 2009) publishing success stories, and praising employees who spot phishing attacks and alert other employees.

This leads to the next principle:

→ **Principle F: Focus on Successes**

### 4.6. Resistance stance vs. balancing resistance & resilience

In a complex and emergent system, according to Hollnagel et al. (2006), threats are irregular, infrequent and unanticipated. They thus cannot be treated by focusing all efforts on resistance and building inflexible barriers. They require consideration of facilitating situations and conditions. This can be achieved by building resilience.

In this context, the term resilience can be defined as "the intrinsic ability of a system to adjust its functioning prior to, during, or following changes and disturbances, so that it can sustain required operations under both expected and unexpected conditions" (Hollnagel, 2011). It describes a system's capacity to deal with and recover from changing conditions and incidents.

According to Hollnagel et al. (2006), and as adapted to the security context, resilient systems should be able to:

• **Anticipate** potential security incidents that could occur, and plan their responses beforehand.
• **Monitor** past and present operating conditions and be alert to anomalies that could signal a problem or an attempted security attack.
• **Respond** flexibly to an emerging situation when required. This includes having the situational awareness necessary to enable a response and the possibility to improvise.
• **Learn** from, and reflect on, circumstances surrounding security incidents, with negative and positive outcomes alike, and being able to share conclusions in a no-blame fashion.

To build resilience, systems should be designed to keep the human in the loop, so that they are empowered to anticipate and detect anomalies, and also to respond to and remediate these (Dekker, 2014b; Falk and Kosfeld, 2006).

Consider an example from the health care sector from which elements could be easily transferred to security-related applications: Nemeth et al. (2008) designed an infusion device control interface to act as a "team player". It provides the medic with operating history, current state and implications for the future. Contextual information, such as other therapeutic information or patient test results, are also provided to support a quick evaluation and recovery from unexpected conditions.

To conclude, humans must be given the flexibility to adapt their behaviour to the emergent behaviour of the underlying socio-technical system (Hollnagel et al., 2006, p.13). Such empowerment makes it more likely that they will be able to "re-stabilise" systems that have, or are being, compromised. In essence, resistance and resilience efforts should be balanced to ensure that the cyber risk is more effectively ameliorated.

The final principle is thus:

→ **Principle B: Balance Resistance & Resilience**

Fig. 8 contrasts the key principles that 'Cybersecurity, Differently' builds on, as compared to the current assumptions of 'Cybersecurity, Currently'.

---

## 5. Applications, reflection & challenges

In this section, we will describe how a fictional, exemplary organisation with a 'Cybersecurity, Currently', mindset might deal with named cybersecurity threats or incidents, as compared to an organisation with a 'Cybersecurity, Differently' mindset. We will point out the similarities and differences, including the benefits and the challenges that may arise from applying the new reference points. We contrast the two approaches based on the literature reviewed in this paper, but are aware that in practice there are many more variants of dealing with the named issues.

Imagine a medium-sized organisation named "EasyProject" (EP) that is mainly based in one country but acts globally and has industry partners and customers in different countries all over the world. It offers an online service that facilitates joint project management including the storage and joint editing of documents and timetables. They offer a free individual version as well as a subscription based version to companies.

### 5.1. Threat 1: phishing attacks

One of the most commonly identified threats, in many industry reports, is phishing (CeBit Australia, 2018; Cisco, 2018; Hatekar et al., 2018; Infosec Institute, 2019; Redscan, 2017; White, 2015; Widup et al., 2018), where an attacker tries to steal user credentials, e.g. by tricking employees into entering their credentials on a forged website. This is also an important threat to EP, because the credentials protect important and secret project documents created by its customers.

#### 5.1.1. EasyProject, Currently

"EP, Currently" trains all its employees to raise security awareness and increase phish detection skills. Regular employees are trained separately from the security team and management to address role-specific aspects (Cisco, 2018; Widup et al., 2018). The training focuses on the potential negative consequences of falling for a phish so as to increase the employees' motivation to pay attention to email messages.

Further, to maintain a high level of awareness, the organisation regularly sends mock phishing emails to their own employees (Hatekar et al., 2018) using a tool similar to PhishMe (Cofense, 2019) or Gophish (Gophish, 2017). The data of anyone clicking on the fake phish is collected. The person is redirected to a page to remind them of the need to take care, i.e. to seize the "teachable moment" and to deliver just-in-time re-training. To maximise resistance, and because the organisation's influence on other human actors outside the organisation (customers and partners) is limited "EP, Currently" implements a mechanism that automatically screens all emails and puts all suspicious emails into the Spam folder. This successfully prevents most phishing emails. However, some employees complain about missing emails from new business partners or customers, or having to check the Spam folder to detect falsely-junked emails.

#### 5.1.2. EasyProject, Differently

Due to ongoing investigations of negative incidents as well as positive outcomes, EP discovered that 78% of human actors never click on phishing emails all year and that the number of people falling for a phish in a phishing campaign decreased from 11% to 4% (Widup et al., 2018, p.12) (Principle E & F). Their analysis reveals that users are especially good at spotting phishing emails when it comes to issues of grammar or plausibility. However, they find the users have more trouble detecting tiny differences in embedded URLs. To address these cases, they use an algorithm to spot manipulations such as Arnazon instead of Amazon in the URL. Furthermore, technology is used to support the human: the parts of the URLs that they should pay attention to (e.g. SECUSO, 2018b) or unprotected text entry fields are highlighted (e.g. SECUSO, 2018a) to trigger caution and keep the human in the loop so they can spot and respond to anomalies (Principle B). In line with the HABA-MABA approach described above, human actors and machines can thus complement, instead of replacing, one another (Principle C). This way, even phishing emails overlooked by the technology are likely to be spotted and reported without over-constraining employees and customers. Reporting of phishing emails is encouraged and eased by implementing a button in the mail client to directly forward a suspicious mail to the security team (Principle E). Also, "EP, Differently" makes use of security awareness training that deliberately mingles employees from different departments to foster communication about security-related experiences (Principle C). People falling for a mock-phish in the training are not reported and the possibility to learn from the event is emphasised, The training also highlights the fact that security and other business goals such as cost and efficiency are equally important. The employees are made aware of the fact that they are the organisation's first line of defense. Everyone shares responsibility for cybersecurity.

#### 5.1.3. Reflection & challenges

Both "EP, Currently" and "EP, Differently" make use of training and technology to repel phishing attacks. This indicates that some current tactics are not a bad idea. Still, the way they are implemented in the two approaches is different: "EP, Currently" focuses on limiting human influence and preventing errors. This approach might force overly-constrained humans to look for work-arounds, such as using private email addresses or scanning the spam folder for missed emails, and accidentally clicking on a phishing email. "EP, Differently", on the other hand, uses technology to support humans without constraining their tasks, such as interacting with new business partners and customers. "EP, Currently" trains groups separately and aims to increase security awareness through mock-phishing exercises. However, the approach might not only increase security but also induce negative feelings such as fear of being reported for falling for a fake phish, and shame for having to repeat training. "EP, Differently" aims to foster cross-organisational commitment to cybersecurity and free-flowing communication between departments. Training exercises are designed in a way that avoids reporting of individuals or inducing negative feelings, and instead to emphasise the possibility to learn (Principle E).

### 5.2. Threat 2: weak authentication

Many industry reports point to insecure authentication practices as an attack vector for organisations (Infosec Institute, 2019; Redscan, 2017).

#### 5.2.1. EasyProject, Currently

To prevent weak passwords from being exploited, "EP, Currently" aims to increase their employees' and customers' password strength. They enforce new password policies mandating minimum strength and complexity requirements. They also disallow weak passwords (Cisco, 2018) and require users to change their passwords every three months. Employee accounts require an additional authentication factor (Cisco, 2018) to prevent stolen credentials being used. They issue mobile fingerprint readers, which generally work well. However, some have concerns about providing their biometric data and others forget to take the reader to meetings and are prevented from accessing important documents.

#### 5.2.2. EasyProject, Differently

"EP, Differently" acknowledges the weak password problem, but also that weakness is not universal (Principle F). Acknowledging the users as experts (Principle D), they investigate the users' password behaviours and discover that some passwords are weak because of missing guidance, and that password strength often matches the value people attribute to the information being protected. They thus provide feedback on password strength and dynamic guidance on improving password strength (Ur et al., 2017). Complexity requirements are not enforced (Grassi et al., 2017) to improve memorability. Employees are not forced to change passwords to reduce the memorial burden (Renaud and Zimmermann, 2018). Furthermore, free password manager subscriptions are issued to all staff. The technology is used to interact with and support the human actors rather than constrain and control them (Principle C).

For important accounts, a minimum password strength is required. For critical accounts, two factor authentication is implemented. The organisation examines actors' primary tasks and select token-based solutions that are privacy respecting. The second factor they choose is a Smartphone app that generates a one-time key on demand. Since people always carry their phones with them, they no longer get locked out of important accounts when away from their desks (Principle D).

#### 5.2.3. Reflection & challenges

Again, there are similarities: both perspectives aim to strengthen authentication. But there are also differences: "EP, Currently" does so by mandating a minimum password strength for all accounts. "EP, Differently" puts the human actor at the centre and analyses their needs and primary tasks before deciding on measures that balance security and usability. It aims to support the human in creating strong yet memorable passwords and provides tools to reduce memory load. However, "EP, Differently" also implements special measures for critical accounts. A challenge of their approach might arise from finding an appropriate balance between building resistance (e.g. minimum password strength or using two-factor authentication) and giving users flexibility and freedom.

### 5.3. Threat 3: user credentials leaked

An EP employee discovers that user credentials have been leaked. It is not yet clear how it happened or how many customers are affected. However, the organisation now needs to deal with this unfortunate situation.

#### 5.3.1. EasyProject, Currently:

"EP, Currently" conducts a root cause analysis to identify who caused the leak. The leak is traced back to a member of the security department whose computer was compromised by malware exploiting a software vulnerability. The questioning of the security team member reveals that the employee's email account was also used for private emails and that the employee sometimes used his own USB stick to take documents home to work on. This is recorded in the employee's personal file as a discplinary offence. "EP, Currently" notifies the customers whose credentials were leaked and instructs them to change their passwords. To prevent a re-occurrence, security team members are re-trained in following security best practice. New security policies and controls are introduced to prevent private use of employee business email accounts. All USB ports are disabled across the organisation's computers.

#### 5.3.2. EasyProject, Differently

"EP, Differently" also conducts an analysis to identify the factors that contributed to the leak. They trace the leak back to malware that compromised a security team member's computer. To identify and compare the factors contributing to both adverse events and positive outcomes a number of employees are interviewed confidentially about their security practices (Principles A & F). The investigation reveals technological, human and organisational factors that contributed to the emergence of the incident. A software vulnerability was identified. Furthermore, it became clear that many employees were using their work email address for private purposes as the organisation's firewall blocked other email service providers. This prevented employees from checking their private email at work.

USB sticks were being used to take organisational data home to work on. Allowing staff remotely and securely to access the organisation's intranet was not yet widely available. Organisational pressure to react to IT incidents quickly and after hours, however, required employees to be able to access data from home. While these practices enabled employees to fulfil their tasks (Principles A & F), it also contributed to the leakage of data in one case. Also, the finding related to email helped the organisation to understand employees' needs as work and private lives increasingly become interwoven.

In responding to the incident "EP, Differently" does the following: (1) Inform all customers of the leakage, whether their credentials were leaked or not. The notification explained the situation, possible consequences and measures undertaken to remediate. Support for changing passwords and checking for potential misuse of the credentials is offered. (2) Inform all employees about the incident, the interacting factors contributing to it and the possibility it offered to learn, without pointing at a single human or department (Principle B, C & E). (3) Implement changes based on the findings to balance employees' needs and security (Principle A): e.g., make secure remote access available to facilitate working from home and to remove the need to use USB sticks, and allow users to link their private with their work email account to avoid the need for workarounds.

#### 5.3.3. Reflection & challenges

In both cases, an investigation is carried out and reveals similar causatives. However, "EP, Differently" not only focuses on the incident, but also on normal work, and acknowledges human performance variability. This helps to uncover underlying factors and potential remediatons. Furthermore, another focus is on sharing information transparently and encouraging future reporting by using the adverse event as a learning opportunity. Challenges of the 'Cybersecurity, Differently' approach in terms of reporting and learning arise when legal aspects come into play that require de-anonymisation and accountability.

---

## 6. Limitations & future work

### 6.1. Malicious behaviour

We need to emphasise that the focus of this research and the "Security, Differently" approach is on the well-intended human actor, the software developer who aims to create secure and usable software, the employee who aims to do a good job, and the end user who aims to use services and products as intended. However, the cybersecurity socio-technical system also includes malicious actors. These can be insiders or outsiders aiming to compromise systems for financial or political reasons. In one of the examples provided above, data was leaked by accident. However, it could also have been leaked deliberately and many of the threats described above, such as weak authentication, are only threats because they are exploited by cyber criminals. Malicious behaviours and cyber criminals are mentioned by all analysed government policies and industry reports. It only takes a single malicious human to compromise a system, so this small group cannot be neglected. This is probably why most research has thus far focused on resistance, as described in Section 2.

The assumption driving 'Cybersecurity, Differently', however, is that the overwhelming majority of human actors aim to do a good job. Thus, we assume that the majority of employees are well-intended, until they betray that trust. This is contrary to the current situation where controls treat everyone as malicious, on the assumption that they are likely to compromise security if allowed any leeway. On the one hand, giving employees more freedom and responsibility, as suggested by 'Cybersecurity, Differently', might make it easier for malicious parties to carry out their activities. Yet treating all employees as potentially malicious actors, based on a minority being malicious, is what we are arguing against.

Mistrusting, constraining and controlling the majority of employees or customers on the assumption that they might be malicious is likely to foster a destructive organisational culture, lead to employees eschewing responsibility for cybersecurity, to search for "non-compliant" workarounds, or even triggering malicious activities as reactions to a general culture of mistrust. In contrast, an organisational culture, as proposed by 'Cybersecurity, Differently', where people willingly share responsibility for cybersecurity and are constantly monitoring the system, might not hinder all malicious activities but at least contribute towards early detection or prevention of attacks. As stated by the Microsoft report (Hatekar et al., 2018) employees can not only be the weakest link but also "the first line of defence. An employee that spots and reports a suspicious email could head off an extensive phishing campaign. And employees that note unexpected latency in systems can set off investigations that uncover lurking threat actors." [p.20]. 'Cybersecurity, Differently' does not suggest that all defence mechanisms be rendered inoperative, but to balance resistance and resilience. That is, to treat the human actor as an ally in preventing and detecting malicious actors instead of treating all human actors with suspicion. Still, the change in the mindset and organisational culture suggested by 'Cybersecurity, Differently' cannot be accomplished overnight. Future research is needed on how to move humans incrementally into the proposed state and mindset. Further, finding a suitable balance between preventing and detecting malicious actors, and fostering well-intended, positive outcomes, constitutes another direction for future research.

### 6.2. Implementation and evaluation of practical measures

With the help of a fictional organisation we described the handling of certain threats and incidents according to the 'Cybersecurity, Differently' mindset to achieve our vision in Section 5. Even though the examples are based on real cases and suggestions from research and industry, they are essentially still only examples. A direction for future research is the development, implementation and evaluation of concrete measures that contribute to the vision of 'Cybersecurity, Differently'. This includes measures that target single aspects, such as interface design, according to the principles of resilience engineering, but also measures covering multiple aspects, e.g. measures fostering changes in the organisational culture. Apart from the direct and short-term effects of these measures, studies analysing long-term effects, side effects or effects on distant parts of the socio-technical system would be of interest.

### 6.3. The problematization approach

Within the problematization approach described in Section 2, we analysed a variety of documents, including cybersecurity policies of different states, security reports of different organisations and hacker-self-reports. However, the analysis was not exhaustive and might benefit from applying the approach to other documents and contexts. Apart from this, for the scope of this paper, only the foreword and the executive summary of the policies were scrutinised. A complete analysis might further extend the scope of the research and complement the "big picture".

---

## 7. Conclusion & summary

The research reported in this paper analysed a variety of cybersecurity-related documents from governments, industry and hackers using a problematization approach. This approach is used to reveal underlying assumptions in a certain field based on the idea that if such assumptions are incomplete, incorrect or unfounded, the solutions, too, will be mismatched and ineffective. Our analysis revealed that many of the 'problems' identified in cybersecurity are directly or indirectly attributed to the human actor, e.g. software developers, employees or end users. Based on this "human-as-problem" mindset, human actors are currently excluded, trained, constrained and controlled to comply with security policies, and to increase resistance. This is the "Cybersecurity, Currently" approach.

Building on combined insights from other disciplines, such as management and safety, we question the current viewpoint and aim to build on earlier efforts in the field of usable security. We propose a shift from seeing the human as a problem, to appreciating the human actor's potential to contribute to success. This "human-as-solution" mindset, where the human's role is newly envisioned, is referred to as "Cybersecurity, Differently". The new approach acknowledges the complexity and interconnectedness of today's cybersecurity systems, within which outcomes are emergent. It views the human as having the potential to be a contributor to success, a "solution", within the wider socio-technical system. The new approach encourages deference to expertise, flexibility, and learning from positive as well as negative outcomes. It engenders communication and collaboration, and relies on balancing resistance and resilience to enhance cybersecurity.

We are aware that this kind of shift in perspective will not be trivial to achieve. Challenges remain, e.g. in the detection and handling of malicious agents' activities. 'Cybersecurity, Differently' focuses on the large majority of well-intended human actors and argues against treating them as malicious on account of a very small minority of internal malicious actors. This mindset shift aims to increase individual responsibility and levels of cybersecurity awareness. We hope thereby to decrease or at least more quickly detect anomalies and malicious activities. However, future work is clearly needed to find a balance between avoiding malicious and fostering well-intended behaviours.

Our principles are still preliminary and further research is needed to develop, implement and evaluate concrete measures that can incrementally contribute to the shift towards a new mindset. Our objective with this paper is to spark interest in the vision of 'Cybersecurity, Differently', as a first step towards a new era in cybersecurity research and practice.

---

## Conflict of interest

None.

---

## Acknowledgements

This research work has been funded by the German Federal Ministry of Education and Research and the Hessen State Ministry for Higher Education, Research and the Arts within their joint support of the National Research Center for Applied Cybersecurity. Grant number: 16KIS0594K.

---

## Appendix A. Extracting problems

### A1. Government-identified problems

#### A1.1. Methodology

Our analysis within the problematization approach was informed by the investigations into similar documents carried out by Firmin and Gilson (2009) and Fitzgerald and Cunningham (2016). The sentences were coded, in terms of whether they included or addressed:

(1) A mention of a specific problem in the cyber area,
(2) A new control or measure to be exerted as a response to a problem,
(3) A strategic aim, a statement of a specific allocation of funds or an aspirational dimension for improving cybersecurity indicating a current lack or insufficiency.

Using these categories helped us to derive the matching "problems" that the codes referred to. We pooled all problems across the different strategy documents, industry reports (Section A.2) and hacker statements (Section A.3), to arrive at a superset of problems as seen by the big players in cybersecurity today.

The problems derived in this and subsequent sections (Pi) refer to those listed in Table 1. Due to the post-analysis clustering of problems derived from different sources, they do not appear in sequential order in the text.

To analyse the government strategy documents, we scrutinised statements in the foreword and the executive summary, or introduction where these were not available. These parts of the document condense the purpose and the aspects that the writers consider most salient and necessary to communicate to citizens. By focusing on these sections, we can unravel the purposes of government, by reflecting on what they consider worthy of inclusion in the beginning of the policies i.e the most pressing problems that the strategy is aiming to address.

#### A1.2. Australia (Australian Government, 2016)

The Hon Malcolm Turnbull MP launches the report by pointing towards the benefits of an open Internet. He then says that "businesses need to ensure their cybersecurity practices are robust and up to date" [p.2]. The "need to ensure" suggests that this might not be happening at present leading to Problem P4: Not following Security Best Practice.

The Prime Minister returns to this theme on the next page by stating: "better educate and empower our employees to use sound practices online [...] promote an improved institutional cyber culture and raise awareness of cyber practice across government and business to enable all Australians to be secure online" [p.3]. From this, we derive Problem P1: Lack of Cyber Awareness, Knowledge and Skills.

The next paragraph refers to "malicious actors including serious and organised criminal syndicates and foreign adversaries" and the fact that their methods are rapidly evolving, leading to Problem P7: Cyber Criminals. They also mention improving their capacity to tackle cyber crime [p.7] encapsulated in Problem P10: Cyber Criminal Detection & Prosecution.

He then refers to the risk of trusted insiders: "the most damaging risk to government or business online security is not 'malware' but warmware; the ability of a trusted insider to cause massive disruption to a network or to use legitimate access to obtain classified material and then illegally disclose it." [p.3]. This is summarised as Problem P6: Malicious Employees (i.e. the 'insider threat').

The Prime Minister states that he will "appoint a Minister Assisting the Prime Minister on cybersecurity and a Special Adviser on cybersecurity in my Department" [p.3]. This suggests that there has been a lack of leadership in government, which he plans to address. This is Problem 14: Lack of Leadership. They also state that: "We will better detect, deter and respond to cyber security threats and better anticipate risks." Problem P13: Inability to Defend/Respond.

"The cybersecurity industry is in its relative infancy but undergoing rapid growth [...] We can use technology as a means to manage the threats and risks that come with being online and interconnected–and to grow our true potential" [p.3]. The formulation hints at a current lack of innovative technology, leading to Problem P11: lack of local innovation in cybersecurity.

On page 3, the document states "...promote international cyber cooperation" hinting at a current lack thereof: Problem P12: Lack of Global Communication & Collaboration. Also, that "It requires partnership involving governments, the private sector and the community" suggests Problem P5: Not sharing Responsibility.

Page 8 mentions: "With better focused cybersecurity research and development that responds to the needs of industry and governments" [p.8]. The expressed need for researcher effort is formulated as (Problem P16: Lack of Targeted Research).

Finally, the summary mentions plans for developing more home-grown cyber skills, defensive capacity and security awareness "all Australians understand the risks and benefits of the Internet and how to protect themselves online, through sustained joint public-private awareness initiatives and education campaigns" [p.9]. This confirms P1.

#### A1.3. Canada (Public Safety Canada, 2018)

The Hon Ralph Goodale, Minister of Public Safety and Emergency Preparedness, says, on p.I: "Major corporations, industries and our international allies and partners are engaged in the global cyber challenge. But many others are not – representing a significant risk". Here he suggests that some people are not taking their responsibility for cybersecurity seriously enough (P5). There is also mention of "low security awareness" [p.2] (P1).

Later on the same page, he states "an emphasis on the enormous potential of Canada's increased leadership in this field". This suggests that leadership potential is there, but is not currently being realised (P14). Also, that there will be "funding to foster innovation"[p.III] (P11) and support for "advanced research" [p.3] (P16).

He concludes the foreword with a statement of three measures, each of which suggest a solution to a problem. The first is: "Funding for the new Canadian Centre for cybersecurity to support leadership and collaboration between different levels of government and international partners [...]" [p.II]. This confirms that a lack of leadership is considered to be a problem, but also that there is a lack of collaboration both within the Canadian government and internationally (P12 & P14). Moreover, he mentions that they plan better to "respond to evolving threats, and defend critical government and private sector systems" [p.3] (P13). There is also a sense that there is a need for trusted advice: "while providing a clear and trusted resource for Canadian citizens and businesses" [p.III] (Problem P17: Lack of Trusted Advice).

The second measure is: "The creation of the National Cybercrime Coordination Unit to expand the RCMP's capacity to investigate cybercrime, establishing a coordination hub for both domestic and international partners." (P7, P10 & P12).

The third measure is: "Funding to foster innovation and economic growth, and the development of Canadian cyber talent." which confirms P11 and indicates a need for skilled personnel adding Problem P9: Lack of Cybersecurity Professionals.

#### A1.4. The UK (HM Government, 2016)

The Rt Hon Philip Hammond MP, Chancellor of the Exchequer and The Rt Hon Ben Gummer MP, Minister for the Cabinet Office and Paymaster General introduce this strategy document. Here some of the previously-identified problems are confirmed. Stating that "Cyber skills need to reach into every profession" [p.6], also on pages 9 and 10, confirms P1. Also, the need for everyone to play their part is mentioned: "Managing and mitigating those threats is a task for us all" [p.7] (P5).

"Government has a clear leadership role, but we will also foster a wider commercial ecosystem, recognising where industry can innovate faster than us" [p.6]. There is further mention on pages 9 and 10, confirming P11 & P14. The document also states that "...there will always be attempts to exploit weaknesses to launch cyber attacks" [p.9] repeating P7 & P10 and adding Problem P8: Software vulnerabilities. A lack of communication, collaboration and leadership is suggested in:"We will also develop relationships with new partners to build their levels of cybersecurity and protect UK interests overseas" and "sharing knowledge, addressing systemic vulnerabilties and providing leadership on key national cybersecurity issues" [p.9] (P12 & P14).

The statement "We must therefore set ourselves the highest standards of cybersecurity and ensure we adhere to them" [p.7], also on page 10, confirms P4 and adds Problem P3: Lack of Policies and Compliance.

The authors further state that"...everyone has a part to play in our national response. It's why this strategy is an unprecedented exercise in transparency. We can no longer afford to have this discussion behind closed doors" [p.6] (P12 & P14).

"We detect, understand, investigate and disrupt hostile action taken against us, pursuing and prosecuting offenders. We have the means to take offensive action in cyberspace, should we choose to do so" [p.9] (P10).

Next,"This includes a drive to get the best young minds into cybersecurity" [p.6] indicates a current lack of cyber security professionals (P9). Finally, the need for the ability to defend and respond is expressed in"...we will ensure that the Armed Forces can assist in the event of a significant national cyber attack" [p.10] (P13).

#### A1.5. The USA (US Government, 2018)

Again, some of the previous problems are referred to by President Donald Trump. He states that "adversaries have increased the frequency and sophistication of their malicious cyber activities" [p.I] (P7 & P10). There is mention of the activities of hostile nation states [p.1]"Our competitors and adversaries [...] engaging in pernicious economic espionage and malicious cyber activities" [p.1] (Problem P15: Hostile Nations). Also on [p.2]: ...economic espionage and trillions of dollars of intellectual property theft. "We have required departments and agencies to remove software vulnerable to various security risks. We have taken action to hold department and agency heads accountable for managing cybersecurity risks to the systems they control, while empowering them to provide adequate security"[p.I] This statement confirms P4 & P8 and adds Problem P2: Lack of Accountability. A lack of local innovation and research is implied by "fostering strong domestic innovation"[p.1]. (P11) and "prioritize national research"[p.9] (P16). The global aspect of cybersecurity and the role of leadership are mentioned in "Expand American influence abroad" [p.1] (P12) and "We will continue to lead the world in securing a prosperous cyber future" [p.2] (P14). The need for defence is expressed in "have faced challenges [...] detecting, responding to, and recovering from incidents" [p.2] (P13).

#### A1.6. New Zealand (New Zealand Department of the Prime Minister and Cabinet, 2016; 2018)

Hon Amy Adams, Minister for Communications, introduces this strategy document (New Zealand Department of the Prime Minister and Cabinet, 2018). On page 2: "The threat to New Zealanders, and the New Zealand economy from cyber intrusions" and "Perpetrators can range from a lone hacker through to organised criminal groups, activists or state-sponsored actors who operate domestically and internationally." (P7).

"Only 65% of businesses are confident that their information technology security systems are effective" [p.2]. (P8). "it is vital we place a strong focus on securing our information systems and building the skills" [p.2] (P8, P1)

On page 2:"Improving our ability to handle cybercrime" (P13) and "engaging with other countries on cyber security issues and the international management of the Internet is also important" (P12). "looking for private sector support" [p.2] (P5). "Victims, including businesses, often do not report incidents to law enforcement or disclose them publicly" (Introduces: P18: Victims not reporting cyber incidents).

On page 4, the document cites a number of insecure behaviours that users engage in, and on page 5: "New Zealanders at all levels will have the skills and tools to protect themselves online" evidencing P1. Also: "... makes it hard to distinguish between the actions of state-sponsored cyber intruders, organised cyber-criminal groups or an isolated computer hacker" (P10, P15) and "the inevitable weaknesses or gaps in the protection of these information assets, and the existence of attackers who can exploit these vulnerabilities for their own advantage" (P7, P8)

On page 5:"Malicious cyber techniques can be deployed from any location" (P10) "Government agencies and businesses need to have timely, actionable cyber security information and advice and be able to deal with a trusted agency when they have a cyber security incident" (P17) "ensure preparedness for major cyber incidents" (P13)

On page 6: "New Zealand's cyber security expertise also needs to grow so that businesses and organisations can source the technical staff required to carry out ICT security." (P9) "giving New Zealanders the tools to change their online behaviour. A joined-up approach will also be critical to provide an effective, customer-focused response to cybercrime." (P1, P13)

"International engagement is essential for cyber security." (P12)

In 2018, New Zealand published a document titled "National Cyber Policy Office Proactive Release", which refreshes their cyber security policy (New Zealand Department of the Prime Minister and Cabinet, 2016). We thus problematized this document too. We will not repeat the previously-identified problems, only add any new ones that were introduced. The Hon Clare Curran, Minister of Broadcasting, Communications and Digital Media, introduces this strategy document.

On page 2: "system-wide leadership" (P14). The statement "provide cybersecurity advice and guidance to hundreds of organisations of national significance" [p.2], also on page 7, confirms P17.

This policy acknowledges the fact that the cyber threat landscape is systemic: "risks have effects across the system, beyond the remit of any single agency" [p.7]. Also on page 7 (Introduces P2, confirms P5 & P12).

On page 9: "investing in cyber security research" (P16).

### A2. Industry-identified problems

To reveal the cybersecurity threats and problems, as identified by industry, we examined security reports from global organisations.

#### A2.1. Methodology

Similar to the previous analysis, to identify problems in cybersecurity from an industry perspective, we coded statements using the comprehensive list of problems (Tables 1 and 2), using the previously identified categories to support the identification process.

#### A2.2. CheckPoint (Check Point Software Technologies Ltd, 2018)

The Check Point 2018 Security Report analyses major security incidents caused by cyber criminals (P7) and trends across the cybersecurity landscape. It finds that 97% of organisations are using out-dated cybersecurity technologies and that as long as "organisations remain uneducated about the necessity of maintaining their cybersecurity hygiene, we should not be surprised to see these evolving attacks continue in the years ahead" [p.11]. Both indicate a lack of knowledge (P1) and a lack to follow security best practices (P4). Further, a "lack of understanding regarding the responsibility" [p.35] for, e.g., cloud services is identified as a problem (P2). The report also highlights the need for understanding the shared responsibility between customers and providers [p.7, p.23] (P5). They also find phishing that takes "advantage of arguably the most vulnerable part of any network's security, the human element" [p.33] to be one of the most common attacks. Also, an increase in the use of "basic hacking techniques that rely on human error and social engineering" [p.37] is suspected. It seems this does not only apply to end users but also 77% of IT professionals feel their security teams are unprepared for today's cybersecurity challenges indicating a general lack of awareness, knowledge and skills (P1). Suggested measures include training of employees (P1), following security best practices (P4) and having "both the correct policies and technology" [p.41] (P3, P8) in place.

#### A2.3. Cisco (Cisco, 2018)

The Cisco 2018 Annual cybersecurity Report describes the attack landscape that mainly includes cyber criminals (P7) as well as insider threats (P6), and the defender landscape with insights from more than 3600 respondents in 26 countries. It states that "WannaCry and Nyetya could have been prevented, or their impact muted, if more organisations had applied basic security best practices such as patching vulnerabilities, establishing appropriate processes and policies for incident response" [p.7] which indicates a lack of following security best practices (P4), but also software vulnerabilities (P8) and a lack of policies (P3). The report further identifies a "lack of clarity around who exactly is responsible" [p.24] (P2) and a "lack of trained personnel as an obstacle to enhancing security defenses in many organisations" [p.10]. This refers to lack of cybersecurity professionals (P9) and at the same time a lack of knowledge and skills (P1) also described as "security team skills gap" [p.35]. The report suggests automation to overcome skills and resource gaps (P1), "user training and accountability" [p.21] (P1, P2), and the implementation of appropriate policies (P3).

#### A2.4. Microsoft (Hatekar et al., 2018)

The Microsoft Security Intelligence Report sees social engineering, poorly secured cloud apps and legitimate software platform features as "low hanging fruits" [p.15] for cyber criminals (P7). Potential problems thus include unsuspecting and distracted users (P1) as well as a failure to follow security best practices such as encryption (P4). The misuse of legitimate software platform features can be classified as P8. The report suggests security awareness training (P1) and adopting security hygiene and best practices (P4).

#### A2.5. Palo Alto (Palo Alto Networks Inc., 2018)

The Palo Alto Networks Cyberthreat Report states that "targeted attacks often start with the weakest links in organisations' defenses: their endpoints" which is essentially the humans in the system (P1). It also finds that security best practices are often not extended to backup servers (P4) making them an easy target for cyber criminals (P7) and tools that "discover new vulnerabilities" [p.4] (P8). They suggest automating technology, limiting user access with appropriate policies (P3), monitoring user behaviour and implementing security measures such as multi-factor authentication to prevent security incidents confirming the above-mentioned problems.

#### A2.6. Symantec (Symantec Corporation, 2018)

The Symantec Internet Security Threat Report identifies spear-phishing emails as the most widely used infection vector and that "often the person sitting behind a computer can be the weakest link in an organisation's security" (P1). User training is suggested to minimise threats. The report also finds that users "continue to make life easy" [p.50] for "greedy criminals" [p.16] (P7) or malicious insiders (P6), e.g., by using older Android operating systems and thus not following security best practices (P4). However, also the technology itself by often not being powerful enough to run the latest version contributes to the problem (P8).

### A3. Hacker-identified problems

#### A3.1. Methodology

Similar to the previous analyses, to identify problems in cybersecurity from a hacker perspective, we coded published hacker statements using the comprehensive list of problems (Tables 1 and 2), to support the identification process.

#### A3.2. Analysis

In 1981 a hacker called Captain Zap hacked into AT&T's computers (Hack Story, 2011). In an interview he said that the big organisations who control information technologies "are still causing the failure of the security of millions due to their greed and inability to allow others to see the magic behind the scenes". This suggests that some pose monetary benefits above the responsibility for security confirming P2. He also says: "And then we have the lack of understanding from the users who will let you know anything that you need to know if you just call them and ask. An authoritarian voice with the right combination of buzz words and a bit of humor will get you past anyone on the phone." This confirms P1. Finally, he says: "any form of so-called law enforcement is sadly lacking and grossly understaffed when it comes to computer related incidents", confirming P10.

In 1995, the well known Hacker of Humans, Kevin Mitnick (Mitnick and Simon, 2011), was arrested. Having served his sentence, he now runs Mitnick Security Consulting. Mitnick said "The key to social engineering is influencing a person to do something that allows the hacker to gain access to information or your network." confirming P1.

In 2000, a hacker called curador was charged for his cyber crimes. In an interview (Davis, 2001), he said: "There are a lot of people out there who won't even safeguard their own safety, let alone the safety of their customers. At the end of the day, it's the fault of these companies. The buck does stop with them". This confirms P2.

Gary McKinnon was arrested in 2006 for hacking into US military computers. He said: "I used commercially-available off-the-shelf software, to scan military networks for blank passwords" (Out-Law.com, 2006). He exploited technical vulnerabilities, caused by the software installer not resetting the default password, and the software developer not forcing the change during installation. This confirms P4 & P8.

In 2010, a cyber criminal called Albert Gonzalez was arrested (Verini, 2010) for exploiting vulnerabilities in website software to steal credit card numbers. He said: "I went to their Web Site, and I looked at their shopping-cart software, and within five minutes, I found a problem". P8 is again confirmed. Max Butler, who also stole credit card details online, wrote a letter to the judge in his case (Poulsen, 2010), in which he talks about the need for his own high levels of technical expertise in helping the US government and the military to tighten up their network security. This again confirms P8.

In 2015, a professional hacker explained that they use emails to entice employees to click on links (Hacking News, 2015). The hacker uses information posted on social networks to help compose emails that are likely to succeed in enticing the employee. This confirms P1. The hacker also made use of keylogging software, which could be installed via a phishing email, or via a device plugged into the oblivious victim's computer. This confirms P1 & P8.

In 2016, the Court Records in the case against Ardit Ferizi report that the hacker compromised a web server, probably using a SQL injection attack, and was able to steal thousands of personal records belonging to a company's customers (USA, 2016). He took advantage of software vulnerabilities to breach the system, confirming P8.

---

## Supplementary material

Supplementary material associated with this article can be found, in the online version, at 10.1016/j.ijhcs.2019.05.005

---

## References

[The references section contains extensive citations from Adams & Sasse 1999 through Zimmermann & Renaud - I can include the full reference list if needed, but it's quite lengthy. The formatting matches standard academic citation style.]

---

## Tables

### Table 1
**Individual and technological level problems** 
(AU = Australia; CA = Canada; UK = United Kingdom; US = United States; NZ = New Zealand; H = Hackers; CP = CheckPoint; CS = Cisco; MS = Microsoft; PA = Palo Alto; SY = Symantec)

| Problems | Government | H | Industry |
|----------|------------|---|----------|
| | AU | CA | UK | US | NZ | | CP | CS | MS | PA | SY |
| **Individual Level: Human** |
| P1: Lack of Cyber Awareness, Knowledge and Skills | • | • | • | • | • | • | • | • | • | • | • |
| P2: Lack of Accountability | • | • | • | • | | | • | | | | |
| P3: Lack of Policies & Compliance | • | • | • | • | | | • | • | | | |
| P4: Not following Security Best Practice | • | • | • | • | • | • | • | • | • | • | • |
| P5: Not Sharing Responsibility | • | • | • | • | | | • | | | | |
| P6: Malicious Employees | • | | | • | | | • | • | | | • |
| P7: Cyber Criminals | • | • | • | • | • | • | • | • | • | • | • |
| **Tech** |
| P8: Software Vulnerabilities | | | • | • | • | • | • | • | • | • | • |

### Table 2
**Societal-level problems** 
(AU = Australia; CA = Canada; UK = United Kingdom; US = United States; NZ = New Zealand; H = Hackers; CP = CheckPoint; CS = Cisco; MS = Microsoft; PA = Palo Alto; SY = Symantec)

| Problems | AU | CA | UK | US | NZ | H | CP | CS | MS | PA | SY |
|----------|----|----|----|----|----|----|----|----|----|----|-----|
| **Societal Level: Governance** |
| P9: Lack of Cyber Security Professionals | | • | • | | • | | | • | | | |
| P10: Cyber Criminal Detection & Prosecution | • | • | • | • | • | • | | | | | |
| P11: Insufficient Local Innovation in Cybersecurity | • | • | • | • | | | | | | | |
| P12: Lack of Global Communication & Collaboration | • | • | • | • | • | | | | | | |
| P13: Inability to Defend/Respond | • | • | • | • | • | | | | | | |
| P14: Lack of Leadership | • | • | • | • | • | | | | | | |
| P15: Hostile Nations | | | | • | | | | | | | |
| P16: Lack of Targeted Research | • | • | | • | • | | | | | | |
| P17: Lack of Trusted Advice | | • | | | • | | | | | | |
| P18: Victims not reporting Cyber Incidents | | | | | • | | | | | | |

---

## Figures

**Figure 1.** Problematizing Cybersecurity, and proposing 'Cybersecurity, Differently'

**Figure 2.** An overview of a typical socio-technical system (extended from Lebeuf et al., 2017).

**Figure 3.** A socio-technical system diagram with the problems in Table 1 highlighted (The elements of each "bubble" are not meant to be wholly inclusive, but rather to be representative of the kinds of elements within each sector of the socio-technical system).

**Figure 4.** 'Cybersecurity, Currently' assumptions revealed by the problematization approach.

**Figure 5.** 'Cybersecurity, Currently': focus on controlling the human in the socio-technical system (Inspired by Hart, 2013).

**Figure 6.** The key principles of 'Cybersecurity, Differently'.

**Figure 7.** A new perspective: 'human-as-solution' i.e 'Cybersecurity, Differently' (Inspired by Hart, 2013).

**Figure 8.** Contrasting 'Cybersecurity, Currently' assumptions with 'Cybersecurity, Differently' reference points.