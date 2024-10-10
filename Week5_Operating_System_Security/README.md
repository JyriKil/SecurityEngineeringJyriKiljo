# Week 5

### Grading

Task #|Points|Description|
-----|:---:|----------|
[Task 1](#task1-bring-your-own-devices) | 1 | Bring Your Own Device
[Task 2](#task2-attacks-on-cpu-execution) | 1 | Attacks on CPU Execution
[Task 3](#task3-securing-os) | 1 | Securing OS
[Task 4](#task4-logging) | 1 | Logging 

---

# Tasks

### Task1: Bring your own devices

Following link containing NIST:s [security recommendations for workplace bring your own device](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.1800-22.pdf). On the page 12 is listed following 9 threat events, and your job is to make one A4 sized poster or otherwise shortly summarize what each listed threat event means based on the document or your own research.

- Intrusive application practices
- Account credential theft through phishing
- outdated phones
- Sensitive data transmissions
- Brute-force attacks to unlock a phone
- Application credential storage vulnerability
- Unmanaged device protection
- Lost or stolen data protection
- Protecting enterprise data from being
inadvertently backed up to a cloud service


Week 5 

 

Task 1 Answers: 

 

Intrusive application practices: Intrusive applications employ deceptive tactics to lure users into downloading them. The lure is often rewards or special features. After installation the applications prompts users to grant permissions for accessing sensitive data. 

 

Account credential theft through phishing: The act of obtaining user credentials through deceptive means by scamming. Common means to do this often includes posing as a trusted entity . Attackers use the credentials to gain unauthorized access and might use them in further attacks. 

 

Outdated phones: Smartphone manufacturers tend to not keep their older phones OS up to date, which means at some point their security won’t be patched and leaves the old phones vulnerable for known bugs and vulnerabilities, even when the newer phones won’t be vulnerable for same exploitations. 

 

Sensitive data transmissions: When sensitive data is leaked through bad security measures such as bad encryption etc. And an unauthorized party gets access to sensitive data.  

 

Brute-force attacks to unlock a phone: Brute-force is a trial and error technique for guessing unknown information like login credentials by trying different compositions one by one. 

 

Application credential storage vulnerability: Result of developers failure to use correct and essential protections to secure the data containing credentials. Examples: Failure to encrypt credential data, or store credentials in an easily accessible file. 

 

Unmanaged device protection: Employees personally owned devices that they set up and use. Since they are unmanaged and in personal use, there is a risk of absent security measures, which makes unmanaged devices vulnerable to attacks. 

 

Lost or stolen data protection: Pretty straightforward, losing or stolen data from you means someone might get access to your personal information without permission, for example payment card, passport or any other identity license, social security number etc. 

 

Protecting enterprise data from being inadvertently backed up to a cloud service: Safeguarding sensitive business data from accidentally being stored or uploaded to cloud-based backup systems without any authorization. 

 

 

 

 

 

 

 

 

 

 

https://blog.pradeo.com/the-suspect-list-part-2-intrusive-applications 

https://www.descope.com/learn/post/credential-phishing 

https://www.cnet.com/tech/mobile/is-that-old-used-refurbished-android-phone-safe-use-what-you-should-know-security/ 

https://escape.tech/blog/sensitive-data-exposure/ 

https://belkasoft.com/unlocking-ios-devices-with-brute-force 

https://www.veracode.com/security/credentials-management 

https://learn.microsoft.com/en-us/microsoft-365/business-premium/m365bp-managed-unmanaged-devices?view=o365-worldwide&tabs=Unmanaged 

https://tietosuoja.fi/en/have-you-misplaced-personal-data 

---

### Task2: attacks on CPU execution
spectre and meltdown are two original side channel attacks discovered in 2017 that target cpu, and over the years more have been discovered. [This wikipedia article](https://en.wikipedia.org/wiki/Transient_execution_CPU_vulnerability) list some of them. Pick 3 of them to research about how exactly each exploits the system,their differences, which systems they targeted and how they can be mitigated. 

Answer in max 300 words. You are free to use tables or otherwise make to comparison easier to read if you wish.


Retbleed (2022): Retbleed targets return instructions in speculative execution, which enables attackers to infer sensitive data by poisoning the return predictions. It impacts Intel CPUs (6th-8th gen) and AMD CPUs (Zen 1 and Zen 2). The attack exploits speculative execution similar to Spectre. Mitigations involve disabling certain speculative execution features, leading to performance hits (up to 39% in Intel and 14% in AMD). This vulnerability is mitigated by microcode updates and operating system patches. 

 

Downfall (2023): Downfall (Gather Data Sampling) affects Intel processors from Skylake to Ice Lake generations. It exploits weaknesses in speculative execution to leak sensitive data like encryption keys and passwords via the AVX (Advanced Vector Extensions) instruction set. This vulnerability can be mitigated with microcode updates, but they significantly reduce performance, especially in applications that heavily use AVX (up to 39% slowdown on Intel CPUs). ARM and AMD processors are unaffected by this vulnerability. 

 

Inception (2023): Inception targets AMD’s speculative execution in the Zen architecture (Zen 1 to Zen 4). By manipulating branch predictors, the attacker can force incorrect speculative execution paths, allowing data leakage. Mitigation includes microcode updates from AMD, although the company considers the practical threat low. Unlike Downfall, Inception doesn’t heavily degrade system performance when mitigated. 



These attacks vary in their methods (return instruction manipulation, AVX instructions, branch predictor manipulation) and target different CPU architectures, but all leverage speculative execution. Mitigations primarily involve microcode updates and disabling speculative features, often at the cost of performance. 



---

### Task3: Securing OS
Following is a list of some of the more common vulnerabilities and attack vectors existing in operating systems.  

- Malware and Viruses
- Exploiting Software Vulnerabilities
- Phishing and Social Engineering
- Drive-by Downloads
- Zero-Day Exploits
- USB/Removable Media Attacks
- Password Cracking

Make short write up about each that answers following questions 
1. What harm can it cause to you?
2. How OS of your choosing (Windows, Mac, Linux) can mitigate it?
     - Function of the OS itself or external tools?


---

### Task4: Logging
Log files are records of events or actions that occur in a system, application, or program. Logs are essential for troubleshooting, debugging, and analyzing the behavior of software or hardware.

Find answers to following questions:
1. What kind of information would be saved into following types of log files
- Application logs
- Event logs
- Service logs
- System logs

2. Where in each of the common Operating Systems those logs would be stored (Windows, Mac, Linux(changes per distro so provide in answer which you are using)
3. What kind of threats could you notice by monitoring each log file?
4. How would you go about monitoring logs on your personal computer?


remember to list sources for information you use!
