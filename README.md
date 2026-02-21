# Cyber Threat Intelligence Dataset from Telegram using BERT

## Overview
Cyber Threat Intelligence (CTI) enables organizations to anticipate, detect,
and mitigate evolving cyber threats. Its effectiveness depends on the availability
of high-quality datasets that support model development, training, evaluation,
and benchmarking.

Attack vectors and adversary tactics evolve continuously, making dataset
construction a challenging task. Telegram has recently emerged as a valuable
source of CTI due to its timely and diverse threat-related information.

This project presents an end-to-end automated pipeline that systematically:

✔ Identifies relevant Telegram channels  
✔ Scrapes threat-related messages  
✔ Filters CTI-relevant content using BERT  
✔ Extracts malicious Indicators of Compromise (IOCs)

The pipeline:

- Scrapes messages from curated Telegram channels
- Uses a BERT-based classifier to filter CTI content
- Achieves classification accuracy of **96.64%**
- Extracts malicious Indicators of Compromise such as:

    - Domains
    - IP Addresses
    - URLs
    - File Hashes
    - CVEs

Finally, a high-fidelity CTI dataset is generated for cybersecurity
research and operational threat detection systems.

---

## Architecture

Telegram Channels → Message Scraper → BERT Classifier → IOC Extractor → CTI Dataset

---

## Dataset Details

| Parameter | Value |
|-----------|------|
Total Channels Identified | 150 |
Channels Used | 12 |
Messages Scraped | 145,349 |
Threat Messages Filtered | 86,509 |
Classifier Accuracy | 96.64% |
IOCs Extracted | Domains, IPs, URLs, Hashes, CVEs |

---

pip install -r requirements.txt
