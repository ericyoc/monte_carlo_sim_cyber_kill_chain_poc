# Monte Carlo Simulation of Attack Scenario using Cyber Kill Chain

This project demonstrates a Monte Carlo simulation of an attack scenario using the Cyber Kill Chain model. The scenario involves an attacker (Eve) attempting to compromise a system, a defender (Alice) trying to detect and stop the attack at various stages, and a victim (Bob) whose system is being targeted.

## Motivating Article
Fowler, S., Joiner, K., & Ma, S. (2024). Cyber Evaluation and Management Toolkit (CEMT): Face Validity of Model-Based Cybersecurity Decision Making. Systems, 12(7), 238.
https://www.mdpi.com/2079-8954/12/7/238


## Cyber Kill Chain

The Cyber Kill Chain is a model that describes the stages of a cyberattack. It helps in understanding the tactics, techniques, and procedures used by attackers and enables defenders to develop effective strategies to prevent, detect, and respond to attacks.

The Cyber Kill Chain consists of seven stages:

1. **Reconnaissance**: Eve gathers information about Bob's system and identifies potential vulnerabilities.
2. **Weaponization**: Eve creates or selects malware tailored to exploit the identified vulnerabilities in Bob's system.
3. **Delivery**: Eve delivers the malware to Bob's system, often through phishing emails or infected websites.
4. **Exploitation**: The malware exploits the vulnerabilities in Bob's system to gain unauthorized access.
5. **Installation**: The malware installs itself on Bob's system, establishing a persistent presence.
6. **Command & Control**: Eve establishes a communication channel with the installed malware to remotely control and manipulate Bob's system.
7. **Actions on Objectives**: Eve carries out malicious activities on Bob's system, such as data exfiltration or lateral movement to other systems.

## Roles in the Scenario

- **Eve**: The attacker who attempts to compromise Bob's system by following the stages of the Cyber Kill Chain.
- **Alice**: The defender who aims to detect and stop Eve's attack at various stages of the Cyber Kill Chain.
- **Bob**: The victim whose system is being targeted by Eve.

## Monte Carlo Simulation

The Monte Carlo simulation is used to estimate the probabilities of Eve successfully completing the attack and Alice detecting and stopping the attack at any stage. The simulation consists of multiple iterations, each representing a possible outcome of the attack scenario based on the given probabilities for each stage.

The simulation takes into account the success probability of Eve and the detection probability of Alice at each stage of the Cyber Kill Chain. By running a large number of simulations and averaging the results, we can obtain reliable estimates of the overall probabilities for Eve's success and Alice's detection.

## Results and Significance

The Monte Carlo simulation provides valuable insights into the likelihood of a successful attack and the effectiveness of defense mechanisms at different stages of the Cyber Kill Chain.

The simulation results align closely with the theoretical probabilities, demonstrating the effectiveness of the Monte Carlo method in estimating probabilities in such scenarios. The results highlight the importance of implementing strong defense mechanisms at each stage of the Cyber Kill Chain to minimize the chances of a successful attack.

By understanding the probabilities associated with each stage, organizations can prioritize their security efforts and allocate resources effectively to strengthen their defenses against cyberattacks.

## Usage

1. Make sure you have Python installed (version 3.6 or above).

2. Install the required dependencies:
   ```
   pip install numpy matplotlib prettytable
   ```

3. Run the simulation:
   ```
   python monte_carlo_simulation.py
   ```

4. The simulation results will be displayed in the console, including a table with the stage-wise probabilities and the overall probabilities obtained from the simulation and the theoretical calculations.

5. A plot will be shown, visualizing the convergence of the cumulative probabilities of Eve's success and Alice's detection towards the theoretical values as the number of simulations increases.

## Data Driven Decision Making

The Monte Carlo simulation of the attack scenario using the Cyber Kill Chain provides valuable insights into the probabilities of a successful attack and the effectiveness of defense mechanisms at each stage. By understanding these probabilities, organizations can make informed decisions to strengthen their cybersecurity posture and mitigate the risk of successful attacks.

The simulation highlights the importance of implementing robust security controls and detection mechanisms at each stage of the Cyber Kill Chain to prevent, detect, and respond to cyberattacks effectively. By adopting a proactive approach and leveraging the insights gained from the simulation, organizations can enhance their resilience against evolving cyber threats.

## Disclaimer
This Pyhton code and associated results are for research and academic purposes only.
