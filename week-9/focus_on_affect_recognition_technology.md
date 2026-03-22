# Focus on Affect Recognition Technology

*This document was researched and written by Claude (claude.ai), an AI assistant made by Anthropic. It was compiled in March 2026 at the request of a human researcher and is intended as a study aid and research primer. All sources are cited with links and listed in the bibliography. Readers are encouraged to verify citations independently and consult primary sources directly.*

---

## Section 1: Latest Updates, Trends, and Thoughts

### What Is Affect Recognition?

Affect recognition — also called Facial Emotion Recognition (FER), Emotion AI, or affective computing — refers to AI systems that attempt to detect, classify, and infer human emotional states from facial expressions, voice patterns, physiological signals, and other biometric data. Kate Crawford's *Atlas of AI* (2021) examines the "affect" industry as part of the broader extractive logic of AI: systems that read human bodies as data sources to be monetized, often without the knowledge or meaningful consent of the people being read.

### Technical Developments (2023–2026)

The field has advanced significantly in recent years. Research from 2019 to 2025 has increasingly focused on deployment challenges and interpretability, with lightweight architectures like MobileNet and EfficientNet explored for on-device emotion recognition in mobile and edge environments. Vision Transformers, Graph Neural Networks, and Explainable AI frameworks have opened new directions by enabling global reasoning and transparency in emotion inference. [Kaur et al., 2024, *Expert Systems*, Wiley](https://onlinelibrary.wiley.com/doi/10.1111/exsy.13670); [Li et al., 2025, *Discover Artificial Intelligence*, Springer](https://link.springer.com/article/10.1007/s44163-025-00553-w)

The technology has moved well beyond facial analysis alone. Multimodal emotion recognition now combines facial expressions with speech, physiological signals, and wearable devices — making real-time emotion detection feasible in everyday settings. [PMC: Comprehensive Review of Multimodal Emotion Recognition, 2025](https://pmc.ncbi.nlm.nih.gov/articles/PMC12292624/)

Systems now claim to interpret non-verbal cues with over 90% accuracy by integrating Facial Expression Analysis, Vocal Emotion AI, and Physiological Sensing. The market is being deployed across retail, healthcare, automotive, and corporate settings. [iWeaver AI: Emotion Recognition Technology Guide, 2026](https://www.iweaver.ai/blog/emotion-recognition-technology-complete-guide/)

### The EU Ban and Regulatory Developments

A landmark regulatory development occurred in Europe: the EU banned emotion AI in workplaces and educational settings — with exceptions for medical and safety contexts — and this ban took effect on August 1, 2024. The EU AI Act explicitly points out the "limited reliability, lack of specificity and limited generalisability" of technologies that claim to infer individuals' states of mind. [University of Michigan School of Information: "Emotion AI Will Not Fix the Workplace," March 2025](https://www.si.umich.edu/about-umsi/news/emotion-ai-will-not-fix-workplace); [Global Workplace Law & Policy: The Prohibition of AI Emotion Recognition Under the AI Act](https://legalblogs.wolterskluwer.com/global-workplace-law-and-policy/the-prohibition-of-ai-emotion-recognition-technologies-in-the-workplace-under-the-ai-act/)

Despite this, the emotion AI market is expected to grow to $446.6 billion by 2032, and its use in HR and workplace monitoring continues to expand in the U.S. without targeted regulation. [University of Michigan School of Information, 2025](https://www.si.umich.edu/about-umsi/news/emotion-ai-will-not-fix-workplace)

### Three Main Arguments Against the Technology

**1. The Science Is Fundamentally Flawed**

Critics argue that the entire enterprise rests on shaky empirical foundations. Scholars from multiple fields have highlighted the lack of scientific basis behind emotion recognition technologies, including the definitional challenges surrounding the concept of "emotions" and their deeply context- and culture-dependent nature. [Global Workplace Law & Policy, Wolters Kluwer](https://legalblogs.wolterskluwer.com/global-workplace-law-and-policy/the-prohibition-of-ai-emotion-recognition-technologies-in-the-workplace-under-the-ai-act/)

A furrowed brow does not mean the same thing in every culture, situation, or on every face. A system trained to read it as "anger" or "stress" is making a profound category error. The foundational "universality hypothesis" — the claim that facial expressions are universally linked to specific emotions — has been increasingly challenged in peer-reviewed literature. [MDPI: "Not in My Face," *Machine Learning and Knowledge Extraction*, 2024](https://www.mdpi.com/2504-4990/6/4/109)

**2. Systemic Bias and Discrimination**

FER systems are built with limited datasets with potential annotation biases, lack cultural context, and exhibit significant unreliability, with misclassification rates influenced by race and background. An emotional analysis conducted by Face++ and Microsoft AI on images of professional basketball players revealed a tendency to assign negative emotions to Black players compared to their White counterparts. [MDPI, "Not in My Face," 2024](https://www.mdpi.com/2504-4990/6/4/109)

Algorithmic biases sustain the oppression of marginalized groups through the underrepresentation of minority groups in training datasets. [MDPI: "Ethical Considerations in Emotion Recognition Research," 2025](https://www.mdpi.com/2813-9844/7/2/43)

**3. Privacy, Consent, and Emotional Autonomy**

Privacy over affect should be considered a civil right. Emotion AI's impact on people's expressions and autonomy remains destructive, with no clear path to ensuring meaningful consent for its use. Harms include chilling effects upon recognition of emotion surveillance, and discrimination as a result of biased and inaccurate inferences — and data could be leveraged to manipulate subjects into making decisions. [ACM FAccT 2025: "Regulating Emotion AI in the United States"](https://dl.acm.org/doi/full/10.1145/3715275.3732014); [University of Michigan School of Information, 2025](https://www.si.umich.edu/about-umsi/news/emotion-ai-will-not-fix-workplace)

### Three Main Arguments in Favor of the Technology

**1. Healthcare and Mental Health Monitoring**

Proponents point to transformative possibilities in medicine. In therapeutic settings, AI could help therapists track a patient's emotional progress over time through longitudinal facial and vocal analysis, and systems could identify subtle markers of depression and anxiety, enabling earlier intervention and personalized care plans. [iWeaver AI, 2026](https://www.iweaver.ai/blog/emotion-recognition-technology-complete-guide/); [Springer: "Advances in Facial Expression Recognition Technologies," 2025](https://link.springer.com/article/10.1007/s10791-025-09699-8)

**2. Safer, More Responsive Human-Machine Interaction**

Advocates argue the technology will make environments smarter and more attuned to human needs. In workplaces, AI analyzing non-verbal cues during video calls could detect fatigue or disengagement, suggesting breaks when stress levels peak, and by monitoring subtle changes in expression, AI assistants could help employees identify early signs of chronic stress. In education, systems focused on real-time student progress tracking aim to support adaptive and personalized teaching strategies by improving the detection of students' emotions. [*Scientific Reports*, "A Comprehensive Deep Learning Framework for Real Time Emotion Detection in Online Learning," 2025](https://www.nature.com/articles/s41598-025-26381-7)

**3. Improving Objectivity and Removing Human Bias**

Supporters claim the technology can reduce the bias humans bring to emotional assessment. Self-report measures of emotion are often unreliable due to recall bias, cognitive bias, acquiescence bias, and social desirability — and emotion recognition AI bypasses these limitations by providing an objective observer rating for emotions. [*Multivariate Behavioral Research*, "A Tutorial on the Use of Artificial Intelligence Tools for Facial Emotion Recognition in R," 2025](https://www.tandfonline.com/doi/full/10.1080/00273171.2025.2455497)

> **Note:** These "pro" arguments are themselves contested. Researchers at the University of Michigan's School of Information argue that emotion AI often exacerbates the very problems its advocates claim it solves, and that claiming it will fix worker well-being, hiring fairness, or patient care is unrealistic — failing to address deeper structural problems. [University of Michigan, 2025](https://www.si.umich.edu/about-umsi/news/emotion-ai-will-not-fix-workplace)

---

## Section 2: Impact on Marginalized Groups

### Overview

Beyond general ethical concerns, affect recognition technology creates acute and compounding problems for specific populations whose emotional expression, facial movement, and social behavior do not conform to the neurotypical, Western, majority-culture norms on which these systems are predominantly trained. For these groups, being misread is not an inconvenience — it carries the potential for material harm in employment, healthcare, education, and surveillance.

### 1. Autistic Individuals and the "Atypical Expression" Problem

This is where the research is most extensive and the implications most serious. FER systems are trained almost entirely on neurotypical facial expressions, meaning they are calibrated to a standard of emotional display that autistic people may not share.

A 2026 study in *npj Digital Medicine* analyzed 184 naturalistic video sessions from 99 autistic children and 85 typically developing peers, and found that autistic children exhibited increased prominence of expressions the system classified as anger, altered emotion transition probabilities, and heightened facial muscle activation patterns. In other words, the system reads genuinely neutral or positive internal states as negative or hostile — not because the child *is* angry, but because their muscular patterns don't conform to the neurotypical template the system was built on. [*npj Digital Medicine*: "Naturalistic Facial Dynamics Enable Quantitative Clinical Assessment of Atypical Expression Phenotypes in ASD," 2026](https://www.nature.com/articles/s41746-026-02375-1)

Research confirms that atypical and subtle facial expression patterns in autistic individuals pose a significant challenge for automated emotion recognition systems — systems that are designed and trained around neurotypical expression norms. [Radočaj & Martinović: "Emotion Recognition in Autistic Children Through Facial Expressions Using Advanced Deep Learning Architectures," *Applied Sciences* (MDPI), 2025](https://www.mdpi.com/2076-3417/15/17/9555)

#### The Double Empathy Problem

A deeper theoretical challenge is raised by what researchers call the **Double Empathy Problem**, now well-established in the peer-reviewed literature. This framework considers deficits in social communication as residing *between* autistic and non-autistic communicators, rather than solely within the autistic individual. Social interaction difficulties are not rooted entirely in autistic individuals, but in the dynamic interaction between different cognitive and perceptual styles. [*Frontiers in Psychiatry*: "Neuro-affirmative Support for Autism, the Double Empathy Problem and Monotropism," 2025](https://www.frontiersin.org/journals/psychiatry/articles/10.3389/fpsyt.2025.1538875/full); [PMC: "Evaluating the Emotional Accuracy of AI-Generated Facial Expressions in Neurotypical Individuals," 2025](https://pmc.ncbi.nlm.nih.gov/articles/PMC12175737/)

This reframing is critical: if the problem is relational rather than individual, then a system trained exclusively to read neurotypical expressions and deployed as a universal standard does not merely fail — it pathologizes difference. A 2025 scoping review in *Autism Research* (Pandey et al., Wiley) documents that most major facial expression databases used to train AI systems contain no data from autistic individuals at all, meaning the systems have no referent for how autistic people actually express emotion. [*Autism Research*: "Facial Expression Databases and Autism Spectrum Disorder: A Scoping Review," 2025](https://onlinelibrary.wiley.com/doi/10.1002/aur.70030)

### 2. ADHD and Specific Learning Disorders

A systematic review published in the *Journal of Attention Disorders* (2023, Universidad del Rosario) found a facial emotion recognition deficit specific to ADHD, with ADHD symptoms and comorbidities appearing to influence the nature and extent of those deficits. A person with ADHD who is being assessed by a hiring algorithm or monitored in an educational setting may have their emotional responses systematically misread — not because they are inscrutable, but because they process and express emotion through different neurological pathways. [PMC: "Establishing the Relationship Between ADHD and Emotional Facial Expression Recognition Deficit: A Systematic Review," *Journal of Attention Disorders*, 2023](https://pmc.ncbi.nlm.nih.gov/articles/PMC10466982/)

A 2025 systematic review in *Journal of Attention Disorders* (Shepard et al., University of Rhode Island) found that 58% of retrieved articles reported significantly decreased emotion recognition accuracy among individuals with ADHD relative to neurotypical peers. [PMC: "Emotion Recognition Accuracy Among Individuals with ADHD: A Systematic Review," 2025](https://pmc.ncbi.nlm.nih.gov/articles/PMC11781233/)

A 2025 comparative study in the *Journal of Autism and Developmental Disorders* evaluated facial emotion recognition in 540 children aged 8–16, including autistic, ADHD, and Specific Learning Disorder (SLD) groups compared to a neurotypical control. The study found that FER difficulties vary by task type, emotion intensity, and the specific neurodevelopmental condition — confirming that no single "deficit profile" applies uniformly, and therefore no single algorithmic model can accurately assess any of these populations. [Springer: "Facial Emotion Recognition in Neurodevelopmental Disorders: A Comparative Study," *Journal of Autism and Developmental Disorders*, 2025](https://link.springer.com/article/10.1007/s10803-025-07120-3)

Research also shows a significant negative correlation between delayed literacy acquisition and facial emotion recognition scores — meaning children whose reading and language development followed an atypical timeline also showed differences in emotion recognition performance, with direct implications for FER system accuracy. [*Alpha Psychiatry*: "Emotion Recognition Skill in Specific Learning Disorder," 2022](https://www.imrpress.com/journal/AP/23/6/10.5152/alphapsychiatry.2022.22219/pdf)

### 3. Cross-Cultural and Socially Variable Expression

A 2023 study in *Scientific Reports* directly demonstrated that an emotion recognition model trained on a regionally specific database collected from North America may fail to recognize standard emotional expressions from another region, such as East Asia. [*Scientific Reports*: "Study on Emotion Recognition Bias in Different Regional Groups," Lukac et al., 2023](https://www.nature.com/articles/s41598-023-34932-z)

A comprehensive review in *Machine Learning and Knowledge Extraction* (2024) found that FER systems are built on the controversial "universality hypothesis" — the claim that facial expressions are universally linked to specific emotions — and that recent research highlights significant variability in how emotions are expressed and perceived across different cultures and contexts. [MDPI: "Not in My Face," 2024](https://www.mdpi.com/2504-4990/6/4/109)

A 2025 systematic review in the journal *Emotion* (Li et al., Sage) synthesized 105 studies on cross-cultural differences in facial emotion perception and found meaningful divergences in how Eastern and Western populations process audio-visual emotional cues. Eastern participants showed reduced interference from irrelevant facial cues and heightened interference from audio information, in contrast to their Western counterparts — a distinction that current FER systems are simply not designed to detect or accommodate. [*Emotion*: "Why Do Cultures Affect Facial Emotion Perception? A Systematic Review," Li et al., 2025](https://journals.sagepub.com/doi/10.1177/00220221251334811)

A 2026 systematic review in *Frontiers in Psychology* (Gallant et al.) found that the production of emotional expressions — not just their recognition — shows culturally variable nuances that depend on whether expressions are spontaneous or posed, and that most cross-cultural FER studies focus only on recognition while ignoring production. This means the very training stimuli used to build these systems may not represent how emotions are genuinely expressed in non-Western contexts. [PMC: "Cultural Differences in the Production of Emotional Facial Expressions: A Review," *Frontiers in Psychology*, 2026](https://pmc.ncbi.nlm.nih.gov/articles/PMC12907163/)

### 4. The Compound Problem

What is particularly alarming is the compounding effect of these vulnerabilities. A 2025 study on perception bias in FER for social robotics (Bryant & Howard, Springer) found that girls of color were more prone to misclassification even with similar facial expressions to White girls, and that White annotators were more accurate in classifying expressions in White girls — demonstrating that the biases embedded in training data annotation flow directly into biased AI behavior. [Springer: "Perception Bias in Facial Expression Recognition: Implications for Social Robotics," Bryant & Howard, 2025](https://link.springer.com/chapter/10.1007/978-981-96-3522-1_20)

A neurodivergent person of color from a non-Western cultural background sits at the intersection of all three failure modes simultaneously — and faces a system that was not designed with them in mind, cannot read them accurately, and is increasingly deployed in high-stakes contexts like hiring, education, healthcare, and surveillance where being misread carries real consequences.

---

## Section 3: Follow the Money — Who Stands to Gain

### The Market Scale

The affect recognition industry is one of the fastest-growing sectors in technology. The global emotion detection and recognition market was valued at $37.82 billion in 2024 and is projected to reach $113.32 billion by 2032. Customer experience monitoring was the single largest application segment, accounting for 27% of market share in 2024. [Fortune Business Insights: Emotion Detection and Recognition Market, 2025](https://www.fortunebusinessinsights.com/industry-reports/emotion-detection-and-recognition-market-101326)

The corporations at the center of this market are not fringe players. Major companies operating in the space include Microsoft, Google (Alphabet), IBM, Amazon Web Services, and Affectiva (acquired by Smart Eye AB), alongside specialized firms such as iMotions, HireVue, Realeyes, Uniphore, and Eyeris Technologies. [Emergen Research: "Top 10 Companies in Emotion AI Market," 2025](https://www.emergenresearch.com/blog/top-10-companies-in-global-emotion-ai-market)

Government agencies captured 31% of the emotion detection market share in 2024, meaning public sector institutions — including law enforcement and border control — are significant buyers and beneficiaries of this technology. In July 2024, eGates equipped with facial recognition and emotion-sensing technology were deployed at Hazrat Shahjalal International Airport in Bangladesh, and at CES 2024, Smart Eye and FORVIA demonstrated Emotion AI integration inside vehicles, merging camera systems with Affectiva's affect recognition technology. [GM Insights: Emotion AI Market Size, 2025](https://www.gminsights.com/industry-analysis/emotion-ai-market)

HireVue bundles affect recognition technology — along with word choice and speaking voice — into an overall, automatically generated "employability score" for each job candidate during online interviews, and has over 700 customers globally, including a third of Fortune 100 companies. [RTI International: Facial Emotion Recognition Report](https://www.rti.org/brochures/facial-emotion-recognition)

### Insurance Companies: A Growing Beneficiary

Insurance companies represent one of the less-examined but potentially most consequential sectors standing to profit from affect recognition technology. The mechanisms are multiple and span health, life, disability, and automotive insurance.

**Underwriting and Risk Assessment**

Insurers are already deeply invested in AI-driven risk profiling. AI-driven underwriting can analyze driving behavior, lifestyle choices, physiological signals, and behavioral data to set premiums and assess risk. Insurers using IoT data have reported a 20% reduction in claim losses. [SmartDev: "AI in Insurance Underwriting: The Ultimate Guide," 2025](https://smartdev.com/underwriting-and-risk-assessment-in-ai-revolution/)

The next logical step in this trajectory is the integration of affect data. Unstructured data — including speech in recorded interviews and behavioral signals — can reveal emotional and psychological aspects of risk that structured data may miss. Insurance underwriting platforms are already incorporating sentiment analysis and voice recognition to better understand customers. [Riskonnect: "AI in Insurance Underwriting," 2025](https://riskonnect.com/risk-management-information-systems/ai-in-insurance-underwriting-revolutionizing-policies-for-customers/)

**Mental Health and Life Insurance**

The most direct and alarming intersection between affect recognition and insurance is in mental health and life insurance risk classification. If affect recognition systems are used — even indirectly — to infer emotional instability, chronic stress, depression, or anxiety, this data could become an input for premium pricing, coverage denial, or benefit assessment. A 2025 review paper published via the Geneva Association, a leading international insurance research body, confirms that insurers are actively exploring AI tools to monitor emotional well-being in health contexts. [PMC: "AI Revolution in Insurance: Bridging Research and Reality," 2025](https://pmc.ncbi.nlm.nih.gov/articles/PMC12014612/)

A 2025 paper published in *Law and Innovation* (van Bekkum, Zuiderveen Borgesius & Heskes, Radboud University) directly addresses this: insurers are captivated by two AI trends — data-intensive underwriting and behaviour-based insurance — and notes that while these trends bring advantages, they may also have discriminatory effects on society, particularly when sensitive inferences are drawn from behavioral and emotional data. [*Law and Innovation*: "AI, Insurance, Discrimination and Unfair Differentiation," Radboud University, 2025](https://www.tandfonline.com/doi/full/10.1080/17579961.2025.2469348)

**Proxy Discrimination**

Regulators have already flagged the concern that facial and vocal recognition data could enter life insurance underwriting — not necessarily as explicit inputs, but as proxy variables. In regulatory meetings shaping Colorado's first-in-the-nation life insurance AI regulation, facial and vocal recognition were explicitly cited as examples of External Consumer Data and Information Sources (ECDIS) that may function as proxy variables for protected characteristics. [Gen Re: "Algorithmic Accountability and Proxy Discrimination in Life Insurance," 2022](https://www.genre.com/us/knowledge/publications/2022/november/algorithmic-accountability-and-proxy-discrimination-in-life-insurance-the-regulatory-environment-en)

The New York State Department of Financial Services Insurance Circular Letter No. 7 (2024) directly acknowledged that external consumer data and AI systems "may reflect systemic biases and its use can reinforce and exacerbate inequality," raising significant concerns about the potential for unfair adverse effects or discriminatory decision-making that may disproportionately affect vulnerable communities. [New York DFS: Insurance Circular Letter No. 7, 2024](https://www.dfs.ny.gov/industry-guidance/circular-letters/cl2024-07)

Despite this, nearly one-third of U.S. health insurers still do not regularly test their models for bias or discrimination. [Fenwick: "Tracking the Evolution of AI Insurance Regulation," 2025](https://www.fenwick.com/insights/publications/tracking-the-evolution-of-ai-insurance-regulation)

**The Core Problem for Consumers**

When combined with the known failures of affect recognition on neurodivergent, non-Western, and racially diverse individuals detailed in Section 2, the insurance application of this technology represents a compounding injustice: populations already misread by the system are precisely the populations most likely to be adversely categorized during the underwriting process — and least likely to know why their premiums were set as they were, or their coverage was denied.

### The Responsibility Gap

The question of who bears responsibility when these systems cause harm is one of the most contested issues in AI governance, and the research literature is clear that accountability is systematically diffuse. Studies have shown that practitioners prioritize different responsible AI principles than policymakers, and companies mainly focus on maximizing immediate productivity and revenue while complying with external regulations. Policymakers and the general public, by contrast, focus on society as a whole and long-term developments. [Springer, *AI & Society*: "Challenges of Responsible AI in Practice," 2024](https://link.springer.com/article/10.1007/s00146-024-01880-9)

A lack of transparency prevents accountability since it becomes impossible to identify the human decision that caused harm, or whether to blame the machine itself. This opacity is not incidental — it is the architecture of deflection. [Springer, *AI & Society*, 2024](https://link.springer.com/article/10.1007/s00146-024-01880-9)

The phenomenon of "AI washing" — where companies claim ethical responsibility through the language of responsible AI while continuing harmful practices — has been formally described in peer-reviewed literature. A 2025 paper in *Sage Marketing Management* (Ozturkcan & Bozdağ) frames this as a cycle of AI booing and AI washing that erodes consumer trust. [*Sage Marketing Management*: "Responsible AI in Marketing: AI Booing and AI Washing Cycle of AI Mistrust," Ozturkcan & Bozdağ, 2025](https://journals.sagepub.com/doi/10.1177/14707853251379285)

AI capabilities advanced faster than institutions, labor markets, and governance frameworks could adapt in 2025, exposing a growing gap between reassuring narratives and real-world results — while many providers emphasized responsibility through process and compliance, only a few leaders publicly acknowledged systemic risks and called for explicit limits on deployment. [AIhub: "Top AI Ethics and Policy Issues of 2025 and What to Expect in 2026," 2026](https://aihub.org/2026/03/04/top-ai-ethics-and-policy-issues-of-2025-and-what-to-expect-in-2026/)

### "Let the Consumer Decide" — Why That Framing Is Contested

One of the most recurring patterns in the industry is the argument that harm avoidance is ultimately a matter of consumer choice. Rosalind Picard, who co-founded Affectiva, has directly challenged this logic, arguing that all use of such technologies should be opt-in, and that companies should be required to disclose how their technologies were tested and what their limitations are — adding: "What we have today is that companies can make these outrageous claims which are just false, because right now the buyer is not that well educated. And we shouldn't require the buyers to be well educated." [MIT Technology Review: "Emotion AI Researchers Say Overblown Claims Give Their Work a Bad Name," 2020](https://www.technologyreview.com/2020/02/14/844765/ai-emotion-recognition-affective-computing-hirevue-regulation-ethics/)

This statement from one of the field's own founders is pivotal: the argument that consumers ought to govern themselves presupposes an informed consumer, but the entire structure of the industry works against meaningful consumer information. A World Economic Forum report on responsible AI found limited incentives for companies to report on responsible AI practices, because firms fear reputational and liability issues from disclosure — meaning the information asymmetry between corporations and consumers is not incidental but structurally maintained. [WEF: "Advancing Responsible AI Innovation: A Playbook," 2025](https://reports.weforum.org/docs/WEF_Advancing_Responsible_AI_Innovation_A_Playbook_2025.pdf)

The "shared accountability" model — which distributes responsibility across developers, deployers, and users — has also come under academic criticism. Shared accountability models could backfire by diluting individual responsibility if divisions remain unclear, and there is disagreement about whether executives can reasonably be held liable for AI systems they do not fully comprehend — while making end users accountable overlooks the power asymmetry involved. [*California Management Review*: "Critical Issues About AI Accountability Answered," 2023](https://cmr.berkeley.edu/2023/11/critical-issues-about-a-i-accountability-answered/)

A 2025 ACM FAccT paper on public attitudes toward emotion AI regulation is direct: the public's rejection of evasive tactics — such as the "mirror strategy" of deflecting blame to societal factors — underscores that deflecting blame erodes trust and intensifies reputational damage. Organizations that embed accountability, transparency, and co-creation into their operations will cultivate sustainable public trust in an increasingly algorithmic society. [ACM FAccT 2025: "The Organization–AI–User Responsibility Triangle"](https://journals.sagepub.com/doi/10.1177/27523543251365451)

### The HireVue Case as a Paradigm

The HireVue litigation illustrates how the consumer self-governance argument operates in practice. An active lawsuit alleges that HireVue's system — which uploads interview recordings to Affectiva for facial expression, eye contact, and voice analysis — was used by CVS to generate employability scores, with HireVue claiming the technology can detect whether an applicant "has an innate sense of integrity and honor" and screen out "embellishers." The job applicant did not meaningfully consent to emotional surveillance as a condition of employment consideration, and had no way to know the criteria by which they were being evaluated. In a setting where not participating means not being considered for the job, "opt-out" is not a genuine choice. [HRMorning: "AI Video Software Violates State Law," 2024](https://www.hrmorning.com/news/ai-hr-aware-hidden-danger/)

Meredith Whittaker, then co-director of AI Now Institute at NYU, drew the key distinction: "We are not impugning the entire field of affective computing. We are particularly calling out the unregulated, unvalidated, scientifically unfounded deployment of commercial affect recognition technologies." [MIT Technology Review, 2020](https://www.technologyreview.com/2020/02/14/844765/ai-emotion-recognition-affective-computing-hirevue-regulation-ethics/)

This is precisely what Kate Crawford names in *Atlas of AI*: the extraction of value from bodies and behaviors, sold back to institutions as a tool of governance, while the humans whose expressions generate that value bear all the risk and none of the reward.

---

## Bibliography

All sources listed alphabetically by author/organization.

---

**AIhub.** "Top AI Ethics and Policy Issues of 2025 and What to Expect in 2026." March 4, 2026.
https://aihub.org/2026/03/04/top-ai-ethics-and-policy-issues-of-2025-and-what-to-expect-in-2026/

**Banos, O. et al.** "Sensing Technologies and Machine Learning Methods for Emotion Recognition in Autism: Systematic Review." *International Journal of Medical Informatics*, Vol. 187, 2024.
https://pubmed.ncbi.nlm.nih.gov/38723429/

**Bryant, D. & Howard, A.** "Perception Bias in Facial Expression Recognition: Implications for Social Robotics." In *Social Robotics: ICSR + AI 2024*, Lecture Notes in Computer Science, Springer, 2025.
https://link.springer.com/chapter/10.1007/978-981-96-3522-1_20

**California Management Review.** "Critical Issues About AI Accountability Answered." November 6, 2023.
https://cmr.berkeley.edu/2023/11/critical-issues-about-a-i-accountability-answered/

**Chen, A. & Hao, K.** "Emotion AI Researchers Say Overblown Claims Give Their Work a Bad Name." *MIT Technology Review*, February 14, 2020.
https://www.technologyreview.com/2020/02/14/844765/ai-emotion-recognition-affective-computing-hirevue-regulation-ethics/

**Crawford, K.** *Atlas of AI: Power, Politics, and the Planetary Costs of Artificial Intelligence.* Yale University Press, 2021.

**Dominguez-Catena, I., Paternain, D. & Galar, M.** "Metrics for Dataset Demographic Bias: A Case Study on Facial Expression Recognition." *IEEE Transactions on Affective Computing*, published online July 2, 2024.
https://pubmed.ncbi.nlm.nih.gov/38315605/

**Emergen Research.** "Top 10 Companies in Emotion AI Market in 2025 Shaping Industry Trends." 2025.
https://www.emergenresearch.com/blog/top-10-companies-in-global-emotion-ai-market

**Fenwick.** "Tracking the Evolution of AI Insurance Regulation." December 11, 2025.
https://www.fenwick.com/insights/publications/tracking-the-evolution-of-ai-insurance-regulation

**Fortune Business Insights.** "Emotion Detection and Recognition Market Size, Share & Trends Report." 2025.
https://www.fortunebusinessinsights.com/industry-reports/emotion-detection-and-recognition-market-101326

**Frontiers in Psychiatry.** "Neuro-affirmative Support for Autism, the Double Empathy Problem and Monotropism." March 13, 2025.
https://www.frontiersin.org/journals/psychiatry/articles/10.3389/fpsyt.2025.1538875/full

**Gallant, I. et al.** "Cultural Differences in the Production of Emotional Facial Expressions: A Review." *Frontiers in Psychology*, 2026.
https://pmc.ncbi.nlm.nih.gov/articles/PMC12907163/

**Gen Re.** "Algorithmic Accountability and Proxy Discrimination in Life Insurance — the Regulatory Environment." November 2022.
https://www.genre.com/us/knowledge/publications/2022/november/algorithmic-accountability-and-proxy-discrimination-in-life-insurance-the-regulatory-environment-en

**GM Insights.** "Emotion AI Market Size, 2025–2034 Trends Report." February 2025.
https://www.gminsights.com/industry-analysis/emotion-ai-market

**Grant Thornton.** "Model Bias Rules Target Insurance Practices." 2023.
https://www.grantthornton.com/insights/articles/insurance/2023/model-bias-rules-target-insurance-practices

**HRMorning.** "AI Video Software Violates State Law." October 18, 2024.
https://www.hrmorning.com/news/ai-hr-aware-hidden-danger/

**Huang, K. & Wu, F.** "The Organization–AI–User Responsibility Triangle: Public Understandings of AI and Expectations for Organizational Responses in AI-Service-Failure Crises." Sage Journals, 2025.
https://journals.sagepub.com/doi/10.1177/27523543251365451

**iWeaver AI.** "Emotion Recognition Technology: 2026 Guide to AI Affective Computing." February 2, 2026.
https://www.iweaver.ai/blog/emotion-recognition-technology-complete-guide/

**Kaur, P. et al.** "Facial Emotion Recognition: A Comprehensive Review." *Expert Systems*, Wiley Online Library, June 26, 2024.
https://onlinelibrary.wiley.com/doi/10.1111/exsy.13670

**Levy, T. et al.** "Facial Emotion Recognition in Children and Youth with Attention-Deficit/Hyperactivity Disorder and Irritability." *European Child & Adolescent Psychiatry* 32, 2271–2280, 2023.
https://pubmed.ncbi.nlm.nih.gov/36050559/

**Li, R. et al.** "Why Do Cultures Affect Facial Emotion Perception? A Systematic Review." *Emotion*, Sage, 2025.
https://journals.sagepub.com/doi/10.1177/00220221251334811

**Li, Y. et al.** "Revolutionizing Facial Emotion Recognition: In-depth Analysis of Cutting-edge Models, Methodologies, and Datasets." *Discover Artificial Intelligence*, Springer Nature, December 17, 2025.
https://link.springer.com/article/10.1007/s44163-025-00553-w

**Lievore, R. et al.** "Facial Emotion Recognition in Neurodevelopmental Disorders: A Comparative Study in Children and Adolescents With and Without Autism, ADHD, and Specific Learning Disorders." *Journal of Autism and Developmental Disorders*, Springer, November 18, 2025.
https://link.springer.com/article/10.1007/s10803-025-07120-3

**Lukac, M. et al.** "Study on Emotion Recognition Bias in Different Regional Groups." *Scientific Reports* 13, 8414, 2023.
https://www.nature.com/articles/s41598-023-34932-z

**MDPI.** "Ethical Considerations in Emotion Recognition Research." *AI*, Vol. 7, No. 2, May 29, 2025.
https://www.mdpi.com/2813-9844/7/2/43

**MDPI.** "Not in My Face: Challenges and Ethical Considerations in Automatic Face Emotion Recognition Technology." *Machine Learning and Knowledge Extraction*, Vol. 6, No. 4, 2024.
https://www.mdpi.com/2504-4990/6/4/109

**MIT Technology Review.** "AI Isn't Great at Decoding Human Emotions. So Why Are Regulators Targeting the Tech?" August 14, 2023.
https://www.technologyreview.com/2023/08/14/1077788/ai-decoding-human-emotions-target-for-regulators/

**Nartey, J.** "The Ethics of Emotion Recognition Technology: Implications for Privacy and Consent." SSRN, April 1, 2025.
https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5200140

**New York State Department of Financial Services.** "Insurance Circular Letter No. 7 (2024): Use of Artificial Intelligence Systems and External Consumer Data and Information Sources in Insurance Underwriting and Pricing." 2024.
https://www.dfs.ny.gov/industry-guidance/circular-letters/cl2024-07

**Olaya-Galindo, M.D. et al.** "Establishing the Relationship Between Attention Deficit Hyperactivity Disorder and Emotional Facial Expression Recognition Deficit: A Systematic Review." *Journal of Attention Disorders* 27(11): 1181–1195, September 2023.
https://pmc.ncbi.nlm.nih.gov/articles/PMC10466982/

**Ozturkcan, S. & Bozdağ, A.A.** "Responsible AI in Marketing: AI Booing and AI Washing Cycle of AI Mistrust." *Journal of Marketing Management*, Sage, 2025.
https://journals.sagepub.com/doi/10.1177/14707853251379285

**Pagán, A. & Loveland, K.A.** "Evaluating the Emotional Accuracy of AI-Generated Facial Expressions in Neurotypical Individuals." *Discover Computing*, Springer, June 13, 2025.
https://pmc.ncbi.nlm.nih.gov/articles/PMC12175737/

**Pandey, R. & Bhushan, B.** "Facial Expression Databases and Autism Spectrum Disorder: A Scoping Review." *Autism Research*, Wiley Online Library, March 28, 2025.
https://onlinelibrary.wiley.com/doi/10.1002/aur.70030

**PMC / *Scientific Reports*.** "A Comprehensive Deep Learning Framework for Real Time Emotion Detection in Online Learning Using Hybrid Models." November 25, 2025.
https://www.nature.com/articles/s41598-025-26381-7

**PMC.** "AI Revolution in Insurance: Bridging Research and Reality." *Frontiers in Artificial Intelligence*, 2025.
https://pmc.ncbi.nlm.nih.gov/articles/PMC12014612/

**Radočaj, D. & Martinović, G.** "Emotion Recognition in Autistic Children Through Facial Expressions Using Advanced Deep Learning Architectures." *Applied Sciences* (MDPI), Vol. 15, No. 17, 2025.
https://www.mdpi.com/2076-3417/15/17/9555

**RTI International.** "Facial Emotion Recognition." Research Brief.
https://www.rti.org/brochures/facial-emotion-recognition

**Shepard, E.C. et al.** "Emotion Recognition Accuracy Among Individuals With ADHD: A Systematic Review." *Journal of Attention Disorders* 29(3): 174–194, February 2025.
https://pmc.ncbi.nlm.nih.gov/articles/PMC11781233/

**SmartDev.** "AI in Insurance Underwriting: The Ultimate Guide 2025." April 3, 2025.
https://smartdev.com/underwriting-and-risk-assessment-in-ai-revolution/

**Springer / *AI & Society*.** "Challenges of Responsible AI in Practice: Scoping Review and Recommended Actions." February 19, 2024.
https://link.springer.com/article/10.1007/s00146-024-01880-9

**Springer / *Discover Computing*.** "Advances in Facial Expression Recognition Technologies for Emotion Analysis." September 23, 2025.
https://link.springer.com/article/10.1007/s10791-025-09699-8

**Springer / *npj Digital Medicine*.** "Naturalistic Facial Dynamics Enable Quantitative Clinical Assessment of Atypical Expression Phenotypes in Children with Autism Spectrum Disorder." January 21, 2026.
https://www.nature.com/articles/s41746-026-02375-1

**Tandfonline / *Law and Innovation*.** "AI, Insurance, Discrimination and Unfair Differentiation: An Overview and Research Agenda." Van Bekkum, Zuiderveen Borgesius & Heskes, Radboud University. Published March 11, 2025.
https://www.tandfonline.com/doi/full/10.1080/17579961.2025.2469348

**Tandfonline.** "A Tutorial on the Use of Artificial Intelligence Tools for Facial Emotion Recognition in R." *Multivariate Behavioral Research*, 2025.
https://www.tandfonline.com/doi/full/10.1080/00273171.2025.2455497

**University of Michigan School of Information (Andalibi, N.).** "Emotion AI Will Not Fix the Workplace." *ACM Interactions Magazine*, March 2025. Published online March 6, 2025.
https://www.si.umich.edu/about-umsi/news/emotion-ai-will-not-fix-workplace

**ACM FAccT 2025.** "Regulating Emotion AI in the United States: Insights from Empirical Inquiry." *Proceedings of the ACM Conference on Fairness, Accountability, and Transparency*, 2025.
https://dl.acm.org/doi/full/10.1145/3715275.3732014

**ACM FAccT 2025.** "Technical Solutions to Emotion AI's Privacy Harms: A Systematic Literature Review." *Proceedings of the ACM Conference on Fairness, Accountability, and Transparency*, 2025.
https://dl.acm.org/doi/full/10.1145/3715275.3732074

**ACM FAccT 2025.** "Emotion AI in Job Interviews: Injustice, Emotional Labor, Identity, and Privacy." *Proceedings of the ACM Conference on Fairness, Accountability, and Transparency*, 2025.
https://dl.acm.org/doi/10.1145/3715275.3732002

**ACM CSCW 2024.** "What Should We Do with Emotion AI? Towards an Agenda for the Next 30 Years." *Companion Publication of the 2024 Conference on Computer-Supported Cooperative Work and Social Computing*.
https://dl.acm.org/doi/10.1145/3678884.3689135

**World Economic Forum.** "Advancing Responsible AI Innovation: A Playbook." 2025.
https://reports.weforum.org/docs/WEF_Advancing_Responsible_AI_Innovation_A_Playbook_2025.pdf

**Wolters Kluwer / Global Workplace Law & Policy.** "The Prohibition of AI Emotion Recognition Technologies in the Workplace Under the AI Act." 2025.
https://legalblogs.wolterskluwer.com/global-workplace-law-and-policy/the-prohibition-of-ai-emotion-recognition-technologies-in-the-workplace-under-the-ai-act/

---

*Compiled March 2026. This document is intended as a research primer and reading guide to accompany Kate Crawford's "Affect" chapter in* Atlas of AI *(Yale University Press, 2021).*
