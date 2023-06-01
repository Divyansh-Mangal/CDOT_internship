# CDOT_internship
This repository contains my contribution to CDOT-QKD efforts. This code is for efficienctly finding settings for lambda (temperature control) and current controls for matching of Bob's and Alice's lasers for MDI-QKD in the macro-frequency range (higher than 500MHz which is the sensitivity range for the FPGA used in the implementation). The assumption is that either Bob's of Alice's laser frequency is held constant while the other's parameters are tuned to match the frequency of the first one.

Note: This code implementation is based on assumption of linearity of response of frequency of the laser with respect to parameters (lambda and current). This assumption is based on the preliminary data collected in May, 2023 for characterizing the laser freq. response with respect to both parameters. 
In case linearity assumption does not hold, then there needs to a better determination of response function and more sofisticated algorithms (gradient descent etc.) would be required. 

This implementation assumes that the data is fed manually, but in case of automated frequncy readers, this algorith could be easily adopted for the automated version.
