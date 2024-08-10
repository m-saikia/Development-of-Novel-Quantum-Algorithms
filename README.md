# Development-of-Novel-Quantum-Algorithms
Womanium Quantum+AI 2024 Projects

**Please review the participation guidelines [here](https://github.com/womanium-quantum/Quantum-AI-2024) before starting the project.**

_**Do NOT delete/ edit the format of this read.me file.**_

_**Include all necessary information only as per the given format.**_

## Project Information:

### Team Size:
  - Maximum team size = 3
  - While individual participation is also welcome, we highly recommend team participation :)

### Eligibility:
  - All nationalities, genders, and age groups are welcome to participate in the projects.
  - All team participants must be enrolled in Womanium Quantum+AI 2024.
  - Everyone is eligible to participate in this project and win Womanium grants.
  - All successful project submissions earn the Womanium Project Certificate.
  - Best participants win Womanium QSL fellowships with Classiq. Please review the eligibility criteria for QSL fellowships in the project description below.

### Project Description:
  - Click [here](https://drive.google.com/file/d/1PGNUShboB4ik_JHZGcIPTh3KYi-aajzp/view?usp=sharing) to view the project description.

## Project Submission:
All information in this section will be considered for project submission and judging.

Ensure your repository is public and submitted by **August 9, 2024, 23:59pm US ET**.

Ensure your repository does not contain any personal or team tokens/access information to access backends. Ensure your repository does not contain any third-party intellectual property (logos, company names, copied literature, or code). Any resources used must be open source or appropriately referenced.

### Team Information:


Team Member 1:
 - Full Name: Manimugdha Saikia
 - Womanium Program Enrollment ID : WQ24-Rhbgvb5vmtt0G9Q


Team Member 2:
 - Full Name: Sayantan Roy Chowdhury
 - Womanium Program Enrollment ID : WQ24-cdORm8OJWzcADW4


Team Member 3:
 - Full Name: Priya Bucha Jain
 - Womanium Program Enrollment ID : WQ24-jpE8OCL1Z9LmHam

### Project Solution:
Designing classically verifiable algorithm to demonstrate quantum compuattional advantage is challenging. Nevertheless,  **Gregory D. Kahanamoku-Meyer, Soonwon Choi, Umesh V. Vazirani, and Norman Y. Yao** have accomplished this in their paper <a href="https://www.nature.com/articles/s41567-022-01643-7"> Classically verifiable quantum advantage from a computational Bell test</a> by proposing an interactive protocol for finding preimages of a trapdoor claw free function. Their algorithm consists of three rounds of interaction between a quantum prover and a classical verifier. The first two rounds relies on measuring appropriate registers in expertly designed superpositions while the last round utilises a surprising connection to Bell's inequality to demostrate quantum advantage.

The authors have implemented their algorithm in Cirq, which we now do in Classiq. The major challenge the authors faced to implement this algorithm was designing an appropriate circuit that computes square of a number modulo N, which has already been implemented in Classiq. Instead, we invest our efforts in efficient transitioning from the first round  to the second and third rounds in the interactive protocol, which is comparitively harder for us due to the absence of measurement of a targeted register in Classiq. We circumvent this challenge by simulating round 1 enough number of times, recording the outputs, and then preparing the appropriate states for round 2 and round 3.

#### Organization of the files:
The repository contains the following two folders:

- Notebook: This folder contains the jupyter notebook `Classically_verifiable_quantum_advantage.ipynb` that contains a brief outline of the quantum protocol in the paper and our implementation. The notebook contains break-down of the major functions used to implement the protocol. The folder also contains an output file `outputs.txt` for our run of the code with 150 iterations.

- Qmod files: This folder contains `.qmod` and `.qprog` files of the quantum model and the quantum program of the Classiq Qmod language.

#### Execution Instructions:
The notebook `Classically_verifiable_quantum_advantage.ipynb` is executable. Please execute all the cells of the notebook in order with the Classiq Qmod environment installed in your kernel.

#### Acknowledgements:
We thank the <a href = "https://womanium.org/Quantum/AI"> Womanium </a> team for organizing this amazing program and providing us the opportunity to work on this project.


### Project Presentation Deck:
_Link a 5min. presentation recording or deck here._

