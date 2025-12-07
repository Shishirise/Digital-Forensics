# Digital Forensics: Raghubansi Murder Case

This repository contains a case study presentation on the Raghubansi Murder Case.  

[View Presentation](https://www.canva.com/design/DAGxgghX0xU/VzPImFQ1EfZPO8Bm85SjuA/edit?utm_content=DAGxgghX0xU&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton
)

## AI forensic pro..

[View Presentation](https://docs.google.com/presentation/d/1TTrJrfMkUKbtdivgwu8npbobUBAW4A-hl_mO42tL-cc/edit?usp=sharing)





| FEATURE                                   | NORMAL DATA                     | MALICIOUS DATA (Attack)                      |
|-------------------------------------------|---------------------------------|----------------------------------------------|
| **Source IP**                             | 10.20.130.10                    | 10.20.130.10 (same IP repeating)             |
| **Destination IP**                        | 192.168.1.53                    | 192.168.1.53                                  |
| **Timestamp**                             | Steady, spaced (10:11:22)       | Rapid hits (14:21:55 → every 0.12s)          |
| **Protocol**                              | TCP                             | TCP                                          |
| **Port**                                  | 443                             | 443                                          |
| **Packet Size**                           | ~214 bytes                      | ~524 bytes (larger burst traffic)            |
| **Login Result**                          | SUCCESS (or few FAILS)          | FAILED repeatedly                            |
| **Failed Login Count (30s)**              | 2–5                             | 187                                          |
| **Total Failed Logins (45s)**             | <10                             | ~1000                                        |
| **Packets Per Second (PPS)**              | ~18–20                          | 420                                          |
| **Avg Time Between Attempts**             | ~2.1 seconds                    | ~0.12 seconds                                |
| **Unique Usernames Attempted**            | 1 user                          | 16 usernames (attacker cycling)              |
| **Burst Activity**                        | NO                              | YES (continuous flood)                       |
| **Baseline Deviation**                    | LOW                             | HIGH (900% increase)                         |
| **AI Behavior Score**                     | NORMAL                          | ABNORMAL                                     |
| **Detected Pattern**                      | Normal login                    | Brute-force password attack                  |
| **Classification Result**                 | Legitimate user behavior        | BRUTE-FORCE ATTACK (97% confidence)          |
| **Response**                              | Allow traffic                   | Block IP + Send Alert                        |


