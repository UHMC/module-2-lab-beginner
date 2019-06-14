# Module 2 - Beginner Lab: Bitcoin Mining and Consensus

## Background
Bitcoin is not the first digital currency, but it is the first to use what is now known as Nakamoto Consensus to negate the need for a central transaction-clearing authority. In this lab, we will explore the topic of trustless network consensus. To do so, we will play a game modeled after the famous Byzantine Generals Problem. The goal of this game is to try to win a reward through unanimous agreement or insidious chaos.

## Meta Information
| Attribute | Explanation |
| - | - |
| Summary | Bitcoin is a digital currency which relies on network consensus to validate transactions. |
| Topics | Consensus, Byzantine fault tolerance. |
| Audience | CS1 or later. |
| Difficulty | Beginner. |
| Strengths | This lab provides a hands-on introduction to network consensus. |
| Weaknesses | The topics may be considered quite abstract, and the actual implementation used in Bitcoin is beyond the scope of this lab. |
| Dependencies | At least 4 participants to a group, paper, writing implements, and rewards (see [Assignment Instructions](#assignment-instructions) for quantity of each). |
| Variants | There is an intermediate version of this lab which covers more technical aspects (signing, fault tolerance with reduced group size). |

## Assignment Instructions (20 Minutes)
1. Form groups of 4 to 7 players (denoted _n_ for each group).
2. Gather the required materials (for each group):
    * _(n-1)^2_ pieces of paper, i.e. 9, 16, 25, or 36 for a group of size 4, 5, 6, or 7, respectively.
    * _n_ writing implements (pens, pencils, markers, etc.)
    * _2n-2_ potential rewards.
3. Have each group randomly select a commander; the rest of the players in a group will be lieutenants.
4. Distribute the materials according to role:
    * Each commander receives _n-1_ pieces of paper and 1 writing implement.
    * Each lieutenant receives _n-2_ pieces of paper and 1 writing implement.
5. Let each player (regardless of role) now decide secretly if they are loyal or treacherous and register this status with only the reward giver (lab proctor).
    * There is incentive both for loyalty (1 reward) and treachery (2 rewards). The incentive for treachery is greater, but with increased risk (0 rewards).
6. The commander will now decide on a choice: attack, or retreat, and depending on status of loyalty, may send the same or different choice to each of the _n-1_ lieutenants via concealed, written messages.
7. Upon receipt of the commander's choice, each lieutenant will now send a choice via concealed, written message to each of the _n-2_ other lieutenants: the same as their receipt of the commander's choice if loyal, or the opposite if treacherous.
8. Each lieutenant, regardless of loyalty, now finds which of the choices they received is the majority choice and reports this choice to the reward giver.
9. Per group, the reward giver now distributes rewards as follows:
    * Loyal players each receive 1 reward.
    * If any loyal player disagrees with any other loyal player, each traitor receives 2 rewards; otherwise, traitors receive nothing.

## Credits
Dr. Debasis Bhattacharya  
Mario Canul  
Saxon Knight  
https://github.com/bitcoinbook/bitcoinbook  
The Byzantine Generals Problem - Leslie Lamport, Robert Shostak, and Marshall Pease
