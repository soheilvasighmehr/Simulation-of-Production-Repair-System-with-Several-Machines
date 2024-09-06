# Simulation of Production Repair System with Several Machines

Problem Statement
In a workshop with 70 milling machines, the goal is to maintain 63 machines in continuous operation while 7 machines remain as spares. Machines experience failures with lifetimes uniformly distributed between 100 and 200 minutes. Failed machines are sent to a repair station where repair times are uniformly distributed between 30 and 60 minutes. If repair technicians are busy, machines wait in a queue. Spare machines are immediately used to replace the failed ones, but if no spares are available, the failed machine’s position remains empty until a spare becomes available. The transportation time of machines to and from the repair station is uniformly distributed between 10 and 15 minutes. Once repaired, machines either replace a failed machine in the production line if space is available or are added to the spare machine pool.
The simulation aims to determine the optimal number of repair technicians required to maximize technician utilization and minimize the time lost due to the lack of spare machines. Additionally, the project investigates the impact of increasing the number of spare machines on system performance, given that the cost of lost opportunity is ten times higher than the cost of technician wages.

Simulation Approach
The project involves creating a conceptual model and identifying key state variables and events. The state variables include the number of machines in the queue for repair, the status of each repair technician (busy or idle), the number of machines in operation, and the number of spare machines. The primary events are machine failures and the completion of repairs.
The simulation was run for 40 hours to analyze the system performance under varying numbers of repair technicians. Key metrics collected include:
•	Technician utilization rates
•	Lost opportunity time due to lack of spare machines
•	Number of failures and instances of spare machine shortages
•	Repair times and the maximum queue length at the repair station
Python code was developed to simulate the system, incorporating random number generation for the various time distributions. The simulation was executed multiple times to estimate the optimal number of technicians by examining technician utilization and lost opportunity time.

Results and Analysis
The simulation results showed that the optimal number of technicians for minimizing lost opportunity time and maximizing technician utilization is around 14. This balance is evident from the fact that beyond approximately 14 technicians, the increase in technician utilization starts to diminish, while the time lost due to insufficient spare machines decreases significantly.
The analysis also indicated that increasing the number of spare machines reduces overall costs more effectively than increasing the number of technicians. With more spares, production downtime decreases, as spare machines can immediately replace failed ones, reducing the time lost due to machine unavailability. Conversely, increasing the number of technicians has a limited impact on reducing downtime and may result in higher labor costs without proportional benefits.

Recommendations
Based on the simulation outcomes, it is recommended to focus on maintaining an adequate number of spare machines rather than significantly increasing the number of repair technicians. This approach minimizes production downtime and overall costs more effectively. While additional technicians can improve repair efficiency, the benefit is limited compared to the advantages of having more spare machines available for immediate replacement.
In summary, the simulation provides valuable insights into optimizing repair resources and managing spare parts in a production environment. Ensuring a sufficient number of spare machines should be prioritized to enhance operational efficiency and reduce downtime, while carefully balancing technician resources to avoid unnecessary costs.
