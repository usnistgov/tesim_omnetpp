# Tennessee Simulator federated with OMNET++ networking model

## Summary

This software packet is used to co-simulate wireless netowrks and physical systems in cyber-physical system (CPS) evaluation. The details about the simulator design can be found in [1]. 

The wireless network simulator is built upon the open-source OMNET++ with the INET and MiXiM libraries. It enables the following features in the discrete event packet-level network simulation:
1. TDMA slot allocation for periodic process variable updates
2. IEEE 802.15.4-based transceiver
3. Industrial wireless channel model [2]
4. Co-channel interference (e.g., between IEEE 802.11 and IEEE 802.15.4 radios)

The physical system simulator is based on the Tennessee Eastman simulator C++ code [6]. It works as an independent function module in OMNET++ platform and share the same global clock with the radios (no time synchronization issues).


## Acknowledge
This software packet uses the open-licensed OMNET++ [3], the INET framework [4], and the MiXiM framework [5]. The physical system code is copied from the NIST TEsim repository written by Richard Candell [6]. 

## Reference
[1] Y. Liu, R. Candell, K. Lee, and N. Moayeri, “A Simulation Framework for Industrial Wireless Networks and Process Control Systems,” Proc. IEEE WFCS’16, Aveiro, Portugal, May 2016.

[2] M. Damsaz, D. Guo, J. Peil, W. Stark, N. Moayeri and R. Candell, "Channel modeling and performance of Zigbee radios in an industrial environment," 2017 IEEE 13th International Workshop on Factory Communication Systems (WFCS), Trondheim, 2017, pp. 1-10.

[3] https://omnetpp.org/

[4] https://inet.omnetpp.org/

[5] http://mixim.sourceforge.net/

[6] https://github.com/usnistgov/tesim

The co-simulator was mainly developed by Yongkang Liu, NIST. The contact information can be found in the project website: https://www.nist.gov/programs-projects/wireless-systems-industrial-environments
