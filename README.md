<!-- ABOUT -->
## About

This is the hub for the Center for Cyber Defense (CCD) IoT Network Intrusion Dataset V1 (CCD-INID-V1)


The dataset is captured using 6 Raspberry Pis, 2 router/switches and 2 workstation servers.

The 6 Pis are edge devices. The 2 workstation servers act as fog nodes. The 2 router/switches functioned as endpoints to connect edge to fog.

The 6 edges devices consistently transmit data to cloud-based Firebase database.

This dataset folder consists the following:
Postprocessed - contains the processed data after using NFStream for feature engineering


## List of Attacks
The five attacks are Address Resolution Protocol (ARP) Poisoning, ARP Denial-of-Service (DoS), UDP Flood, Hydra Bruteforce with Asterisk protocol, and SlowLoris. Table 2 describes each attack in detail. Here are the reasonings behind the selection of each attack:

ARP Poisoning - ARP Poisoning generates minimum web traffic. It is extremely challenging for IDS to pick up the signature of this type of attack. We wanted to see how well our IDS can handle this attack signature with limited trace.

ARP DoS - This attack leaves plenty of "breadcrumbs" for IDS to pick up. We sent 600,000 messages at our only available socket at a one-second interval continuously for 12 h.

UDP Flood - Similar to the previous attack, however this attack uses a different protocol. We wanted to test how our IDS handle network traffic with different protocols.

Hydra Bruteforce with Asterisk protocol - This type of attack attempts to gain authentication using commonly used password combinations. Hydra is a well-known attack toolkit. The Asterisk protocol is an interesting choice for our attack selection because it is a protocol that is standard for voice-over-IP, which relates to many users that rely on communication tools such as Zoom, Skype, WeChat, WhatsApp during the COVID-19 pandemic.

SlowLoris - SlowLoris is a new representation for low-bandwidth Distributed Denial-of-Service attacks. First developed by a hacker named Robert "RSnake" Hansen, this attack can bring down high-bandwidth servers with a single botnet computer, as evidenced in the 2009 Iranian presidential election.


<!-- CITATION -->
## Citation

For citation, please use the following as reference:
Liu, Z., Thapa, N., Shaver, A., Roy, K., Siddula, M., Yuan, X., & Yu, A. (2021). Using Embedded Feature Selection and CNN for Classification on CCD-INID-V1: A New IoT Dataset. Sensors, 21(14), 4834.
or
https://doi.org/10.3390/s21144834

<!-- CONTACT -->
## Contact

Zhipeng (Nicholas) Liu - zliu2@aggies.ncat.edu







