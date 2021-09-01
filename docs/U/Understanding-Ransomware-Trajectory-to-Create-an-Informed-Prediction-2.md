---
layout: default
title: II. BACKGROUND
parent: § Understanding Ransomware Trajectory to Create an Informed Prediction 
grand_parent: U
nav_order: 20 
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

## II. BACKGROUND
Ransomware is a subset of malicious software designed to take a victim’s computer or data hostage and demand a ransom payment to regain access. The term comes from the combination of the “ransom” the victim is asked to pay and the “software” that takes hold of the computer system. These ransoms tend to be paid in cryptocurrencies such as Bitcoin, however, paying the ransom doesn’t guarantee the valuables will be released. When dealing with criminals there is always the possibility they won’t hold up their end of the deal. Unfortunately, due to ransomware’s newness and online anonymity, these criminals often fall through the cracks of international jurisdiction and go unpunished. Therefore ransomware has become an attractive low-risk criminal venture. Being victimized by one of these attacks is undeniably frightening and challenges users’ sense of online security.

Ransomware attacks usually follow a predictable pattern. Below are the basic steps of a standard ransomware attack; delivery, execution, payment, decryption, and liquidation [5].

### *A. Delivery*
The ransomware must be delivered to the victim’s system for the attack to begin. ‘Delivery’ doesn’t necessarily capture the harm occurring here though, and since ransomware is considered a disease this process is also colloquially referred to as ‘infection’. The actual payload delivered is called a binary and it’s composed of code that determines the actions of the ransomware. Infection methods vary greatly and I will address them in-depth in my “Infection method” section later.

### *B. Execution*
The ransomware binary activates and begins following the instructions that the attack developer set out. As you would expect in a black market execution instructions vary widely, making the creation of an accurate ransomware execution model particularly challenging. Still, ransomware execution can be divided into three generic stages; stealth operations, suspicious activities, and obvious actions [6].

- 1) *Stealth Operations:* The ransomware must familiarize itself with the victim’s system before initiating the attack. Cybercriminals want their ransomware to remain undetected during this initial step to prevent the attack from being interrupted prematurely [7]. 

- 2) *Suspicious Activities:* The ransomware initiates the damaging part of the attack without announcing itself, potentially remaining undetected. For locker ransomware this stage would include restricting the user interface, for crypto ransomware it would include encryption [6]. 

- 3) *Obvious Actions:* The ransomware announces its attack to the victim and makes its demands known by way of ransom note. At this point the damage has been done to the victim’s system so the ransomware is ready to reveal itself [6].

### *C. Payment*

Now that the ransomware has been executed it is time for the victim to decide if they’ll pay the ransom. If they choose to, payments are usually made in bitcoin rather than a national currency. Bitcoin is a cryptocurrency, a digital currency created to circumvent any central authority. Whereas national currencies are minted and legally enforced by a government, bitcoins are entirely decentralized [8]. This makes it attractive to criminals because it’s unregulated and users remain practically anonymous, providing cybercriminals a method of receiving ransom payments safe from prying eyes [5]. Additionally, transactions are irreversible and bitcoins are universally available for victims to purchase [9]. Oftentimes ransom notes contain instructions for the victim to buy bitcoin from online exchanges then send them to the attacker’s wallet address.

### *D. Decryption*
In the most likely case of a crypto-ransomware attack, after the payment has been received the ransomware may decrypt the files automatically or provide the victim with a decryption binary so they can do it manually [6]. Don’t forget we’re dealing with criminals though, and payment does not guarantee decryption. At this point the victim has already made their payment, so there’s little incentive for the attacker to follow through on decryption.

### *E. Liquidation*
Finally, time for the ransomware attacker to reap their rewards! The attacker cashes out their bitcoin in exchange for a national currency. This is the riskiest stage for the criminals because it links the proceeds of their crime to their identity. To mitigate this risk attackers will sometimes attempt to hide their tracks by shuffling ransom payments from different victims [5]. Once the ransom has been liquidated the attack is complete.

Ransomware has but one goal by definition, to exploit the victim. Cybercriminals employ a wide variety of methods to achieve this goal, but not all methods are created equal, and as such some gain popularity while others fall out of favor. An excellent example of this constant evolution is the transition from locker ransomware to cryptographic ransomware as the dominant attack method. Locker and crypto are the two main ransomware types [7], however, cybercriminals are creative and there are no rules to the game they play. These two types do not encompass the entirety of ransomware variety, others exist, but for the purposes of this example they are appropriate.

From approximately 2011 to 2012 locker ransomware was the dominant cyber extortion threat, only a few years after its emergence in 2008 [7]. Locker ransomware is based on the idea of locking the victim out of their computer. That is achieved by taking over the user interface, usually restricting user capabilities so that the computer can only be used to pay the ransom. Generally, locker ransomware only affects the user interface, leaving the users’ files unharmed. That allows tech-savvy victims to often fully recover from these attacks by restoring system settings or using security tools [7]. Additionally, if the victim is able to transfer the computer’s hard drive to an uninfected computer then no data is lost [10]. Therefore, locker ransomware isn’t the most effective ransomware variant. To make up for its weaknesses many locker ransomwares employ social-engineering techniques meant to prey on the victims’ fears and emotions to manipulate them into paying the ransom. For example, it’s common for locker ransomware to impersonate law enforcement, claiming to have caught the user engaging in illegal activity online, then asking the victim to pay a fine for their indiscretion. While it has the potential to be very effective against simple computers with limited user interface functionality, locker ransomware has its weaknesses against complex computers [7]. For these reasons cybercriminals began transitioning to cryptographic ransomware en masse in 2013 and haven’t looked back.

In 2013 crypto ransomware rose to become the dominant cyber extortion threat and continued to explode in popularity among cybercriminals [7]. By 2016 more than 95% of new ransomware was of the crypto variety [6]. Cryptographic ransomware is based on the idea of locking the victim out of their files, rather than just their computer, and the only person that can unlock that data is the attacker. A cryptograph is a coded message, so this variant of ransomware achieves its goals through encryption, translating valuable files into unreadable gibberish that only the attacker can decrypt. Encryption requires a key -- a string of letters and numbers, like a password -- so when an attacker locks your file with their key that file can only be unlocked with their key. In this way the attacker denies the victim access to their personal files while often leaving computer functionality otherwise untouched. Once struck by a crypto attack a victims only method of recovery is decryption of the affected files, whether that be via ransom or a decryption tool. The penetrating nature of cryptographic ransomware paired with the strength of mathematical encryption makes crypto-ransomware very effective [7]. Due to the ubiquitous nature of crypto ransomware in recent years any future references to ransomware will refer to crypto ransomware unless otherwise specified.

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
