---
layout: default
title: III. BRIEF RANSOMWARE HISTORY
parent: § Understanding Ransomware Trajectory to Create an Informed Prediction  
grand_parent: U 
nav_order: 30 
---
<style>
.dont-break-out {
  /* These are technically the same, but use both */
  overflow-wrap: break-word;
  word-wrap: break-word;

     -ms-word-break: break-all;
  /* This is the dangerous one in WebKit, as it breaks things wherever */
  word-break: break-all;
  /* Instead use this non-standard one: */
  word-break: break-word;
}

.youtube-container {
    position: relative;
    width: 100%;
    height: 0;
    padding-bottom: 56.25%;
}
.youtube-video {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
}

</style>

<div class="dont-break-out" markdown="1">

1. TOC
{:toc}

## III. BRIEF RANSOMWARE HISTORY
Ransomware is one of the biggest focuses for cybersecurity experts right now [9]. Studying the events that have made ransomware what it is today is helpful in understanding the future of ransomware.

### *A. 1989*
First recorded ransomware, the AIDS Trojan, is deployed at the World Health Organization’s International Aids conference via 5¼ inch floppy disks mailed to the conference intentionally mislabeled “AIDS Information – Introductory Diskettes''. The first of its kind, the AIDS Trojan didn’t actually pose a threat because it used such simple, symmetric cryptography. The ransom was set at $189 USD to be sent to a PO box in Panama. Unlike most ransomware we know who the author was, Joseph L Popp, a biologist now considered the ‘father of ransomware’ [11]. Clearly ransomware was not a threat at this point, rather, in this era malware was used in pranks and vandalism to gain notoriety [7].

### *B. 1996*

Adam Young and Moti Yung, cryptographers, describe the concept of cryptographic ransomware and name it cryptovirology. They published a groundbreaking paper proposing that cryptography -- traditionally used defensively for privacy, authentication, and security -- could be used offensively for extortion-based attacks. They emphasize that asymmetric encryption is essential to these attacks, and warn that access to cryptographic tools should be well controlled [12]. Unfortunately, that warning fell on deaf ears, setting the stage for ransomware to come.

### *C. 2005*
Young and Yung implement the concept they had described years earlier and once again warn against the threat of ransomware. However, this time they also include some user countermeasures: backup your data, have a strong defense (firewall and antivirus), and only download from trusted sources [13]. This represents the first known crypto-ransomware implementation and established the expectation that cybersecurity experts publish ransomware countermeasures.

### *D. 2006*

The first criminal ransomware to make use of asymmetric encryption emerges, only one year after Yung and Young’s proof-of-concept. As they had warned, this represents a massive leap forward in the destructive potential of ransomware and the emergence of effective criminal cryptoransomware. There’s some debate over which ransomware virus did it first, but it was either Archiveus Trojan or GPcode. GPcode disguised itself in a malicious job application email attachment and targeted Russian internet users [11]. The author of GPcode continued to improve their ransomware by enhancing the encryption strength, releasing three versions in the span of five days; the third version used encryption that would have taken 30 years for a contemporary computer to crack [14]. Archiveus Trojan required victims to purchase items from an online pharmacy to receive the 30-digit decryption key [11].

### *E. 2007*
Lou & Liao, security researchers, published a paper claiming that users’ misuse of computer systems had resulted in privacy violations skyrocketing. In response they began promoting awareness and education of ransomware as a means of ransomware prevention [15]. Importantly, this was the first time researchers in information systems security addressed ransomware.

### *F. 2008*
Gazet, a computer virologist, analyzed three early families of ransomware based on their quality of code, ransomware functionality, and cryptographic strength. He concluded that researchers should continue to monitor ransomware, but at the time it was not mature and complex enough to warrant the attention it was receiving in the media, going as far as to say that it was doomed to failure as a mass extortion scheme [16]. At this point the research community had identified ransomware as a problem, but dismissed its severity without even offering potential solutions.

### *G. 2009*
Bitcoin enters the scene and revolutionizes ransomware, transforming it into an established black market. Up until now, ransoms had to be paid in roundabout ways because untraceable online payment was not an option. For example, victims have paid by mailing prepaid cash-equivalent cards, calling a premium rate phone number, or ordering goods from the attacker’s online store [10]. Ransomware attackers were eager to transition to Bitcoin because existing methods were inherently traceable [5].

### *H. 2013*

CryptoLocker is unleashed upon the world and spreads like wildfire. As the name suggests CryptoLocker is a crypto-ransomware; its infection methods include malicious email attachments sent to business professionals and misleading downloads on compromised websites [11]. CryptoLocker went on to infect roughly 500,000 machines and experts estimate CryptoLocker’s revenue at US$3 million conservatively and US$27 million on the high end [17]. Once the ransom note had been presented victims were only given three days to pay, after which the decryption key would be deleted or the price would jump dramatically, depending on the version. CryptoLocker demonstrated to cybercriminals and researchers that cryptoransomware was a mature business model characterized by reliable and untraceable payment. Within three months other cybercriminals adopted CryptoLocker’s business model and multiple copycat ransomwares began circulating [18]. The impact CryptoLocker had on the ransomware industry is best illustrated by looking at the number of attacks in 2013; 100,000 in January and 600,000 in December [7]. Attacking at such scale put a target on CryptoLocker’s back, and within one year security firms had infiltrated the cybercriminal network and set up an online decryption portal which helped keep the percentage of victims that paid the ransom low at 1.3% [17].

### *I. 2015*

A cybersecurity research group publishes a groundbreaking study in the same research area as Gazet. Similar to the previous study but larger, this study reviewed 1,359 ransomware samples from 2006-2014 and found that although a few ransomware samples were sophisticated and threatening, most used superficial techniques [19]. Once again the research community argued that stopping advanced ransomware attacks was simpler than the media was reporting. However, this paper took it one step further. In the process of studying so many ransomware extortion methods they determined that ransomware could theoretically be detected and distinguished from harmless applications by measuring system behavior. This discovery is massively important because it enables researchers to begin detecting ransomware attacks for the first time. Whereas previous research dismissed ransomware as a legitimate threat and stopped there, Kharraz et al. develops a foundational model of ransomware behavior and uses it to advance state-of-the-art defense.

### *J. 2016*
The next year a follow up study was published that implemented the method described in the 2015 paper. By monitoring file accesses and system behavior the research team was able to detect ransomware with a 96.3% accuracy [20]. This is the birth of detection-based defense, an important approach to ransomware defense. Much of the ransomware defense research that has since been published builds upon this study’s techniques, or in some way has these authors to thank.

### *K. 2017*
Ransomware has its most notorious year to date with the widespread attack of WannaCry. WannaCry leveraged an exploit created by the National Security Agency (NSA) that had been stolen and leaked by a group known as the Shadow Brokers. The initial infection likely occurred over an unprotected public internet connection, essentially coffee shop Wi-Fi. What made WannaCry especially devastating was its ability to self propagate like a true virus, meaning damage is not only limited to the machine infected but any other machine on that network [21]. In a matter of hours WannaCry infected hundreds of thousands of machines in more than 150 countries, targeting individual users, business organizations, and public agencies. Although not very profitable, WannaCry infamously targeted the United Kingdom’s National Health Service which catapulted ransomware into public consciousness [11].

### *L. 2019*
Early in the year a group of cybersecurity researchers published a study of contemporary ransomware and concluded it was rapidly diversifying. The recommendation to counter this diversification was to develop better models of ransomware behavior so defenders can more effectively detect and respond to attacks [6]. At this point the research community had fully embraced the idea that they could offer solutions to combat ransomware. Late in the same year MITRE ATT&CK, a cybersecurity expert curated ransomware model, was published online. ATT&CK stands for Adversarial Techniques, Tactics, & Common Knowledge. As the acronym suggests, the model catalogs ransomware methods and was freely available to any person or organization for the purpose of creating a safer world [22].

As you can gather from this brief timeline, in the last fifteen years defending against ransomware has become a serious challenge that we must not underestimate. Early on ransomware development moved slowly and was often pioneered by security research. Security experts were ahead of the curve until cryptocurrencies gave cybercriminals the tools they needed to criminally abuse academic research anonymously. Ransomware defense has been playing catch-up ever since, but even with ransomware attack on the forefront, development isn’t linear. Oftentimes one criminal or group innovates and makes a sporadic leap in ransomware progress that others copy, then that technique becomes widespread and eventually standard practice.

Also, ransomware developers have an inherent head start on large-scale defense efforts for two main reasons. First, even when security measures have been suggested by professionals and the dangers warned against, little preventative action has been taken. Only in recent years have we seen ransomware warnings finally taken seriously by governments and industries, but it's taken financial incentives to make that change. It would appear that only after being burnt are organizations willing to invest the resources necessary to heed the warnings that the stove is hot. Second, as new ransomware attack variants emerge, ransomware defenders need time to develop a suitable defense. Consider the criminal black market that ransomware innovation operates within today. Very little information is available to defense researchers for them to base their techniques upon, besides those observations they make themselves. Similar to a fighter facing a new opponent, defense researchers need to learn the strengths and weaknesses of their foe before making an educated decision on how to fight. Thankfully, in the last few years the fight is swinging in favor of defenders as they collectively share their cumulative knowledge and enjoy greater access to essential resources.

***

#### Table of Contents
{: .no_toc}

<ul><li> <a href="/docs/U/Understanding-Ransomware-Trajectory-to-Create-an-Informed-Prediction-1/">
I. INTRODUCTION</a></li><li> <a href="/docs/U/Understanding-Ransomware-Trajectory-to-Create-an-Informed-Prediction-2/">
II. BACKGROUND</a></li><li> <a href="/docs/U/Understanding-Ransomware-Trajectory-to-Create-an-Informed-Prediction-3/">
III. BRIEF RANSOMWARE HISTORY</a></li><li> <a href="/docs/U/Understanding-Ransomware-Trajectory-to-Create-an-Informed-Prediction-4/">
IV. RESEARCH JUSTIFICATION</a></li><li> <a href="/docs/U/Understanding-Ransomware-Trajectory-to-Create-an-Informed-Prediction-5/">
V. ATTACK OVERVIEW</a></li><li> <a href="/docs/U/Understanding-Ransomware-Trajectory-to-Create-an-Informed-Prediction-6/">
VI. DEFENSE OVERVIEW</a></li><li> <a href="/docs/U/Understanding-Ransomware-Trajectory-to-Create-an-Informed-Prediction-7/">
VII. CONCLUSION</a></li><li> <a href="/docs/U/Understanding-Ransomware-Trajectory-to-Create-an-Informed-Prediction-8/">
REFERENCES</a></li></ul>
***

</div>
