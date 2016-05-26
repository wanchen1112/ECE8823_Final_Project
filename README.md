# ECE8823_Final_Project
Heterogeneous Architecture Design for Mesh (Individual Project)

## Overview
This final project of the course - **Interconnection Networks** is to implement heterogeneous design for Mesh topology. It is developed on *garnet network* in *gem5 simulator*. Since the I am not sure if the source code can be published online, I just put my presentation slides and the report documents for your reference. 

## Implementation

The following statements are some brief introduction of the implemented functions. More details can be found in ```Final_report.pdf```.

- **Buffer utilization**:  
Monitoring the buffers in the routers and reporting the average utilization during the given execution cycles.  
  
- **Hot Spot Traffic Pattern**:  
Add a new traffic pattern for simulating one of the the real world cases - some of the machines experience higher traffic. In this project, the corner routers have more packets going through. 

- **Multiple Injection Rates**:  
The injection rates for a network can be different for the routers. 
    
- **Higher bandwidth on the diagonal routers**:  
Twice of the original bandwidth on the diagonal routers. It is performed by setting lower latencies for the links.

## Notes
During the final presentation, I got the peers' suggestions that higher bandwidth can be just done by adding more physical links for the routers in the simulator instead of changing the latency. Because lower latency does not necessarily mean higher bandwidth, and the result may not be accurate enough if I use the alternative approach. 
