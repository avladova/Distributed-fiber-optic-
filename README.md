# Distributed-fiber-optic-
Problem formulation
Distributed fiber optic measurements already have become powerful tool for continuous real time monitoring of the operations in the oil and gas industry. The field is actively developing with new technologies and applications appearing regularly. The most widespread fiber optic measurements are distributed acoustic sensing (DAS) and distributed temperature sensing (DTS). They provide complementary information and the preferred mode of operation is to have both measurements in the well. Unfortunately, sometimes one of them is not available or part of the data are missing. Thus, the question arises – can one reconstruct realistically missing data (DAS or DTS), if the data from another measurement are available, or can one reconstruct realistically data, if part of the dataset is missing completely? The task is further complicated by the fact that the data volume is large (typical DAS data size is 100s Mb per minute)

Required solution
The solution would be a software that works on the dataset and reconstructs missing parts of the dataset.

Development of a containerized AI algorithm for missing data reconstruction in DAS/DTS data stream
Solution shall be implemented in Python 
Output: reconstructed dataset
Details of challenge
Solution
Containerized solution with callable functions
Input: DAS/DTS data stream – Data have to be available as input in .h5 (DAS), .xlsx (DTS) format

Output: Reconstructed data stream (time/depth) on time grid indicated in the challenge data (note that time grid for DTS and DAS data differ) – export into .h5 (DAS), .xlsx (DTS) format

Available data
Dataset with missing parts will be provided to the participants
Time stamps for missing DTS (in .xlsx file) and DAS data (note)
Evaluation of solution performance
The performance will be evaluated by comparing the reconstructed data with the original dataset. L1/L2 norm will be used, L2 norm normalized by the signal amplitude, etc.
Reconstruction accuracy based on the original datasets
Time duration of training and estimation
Quality of code solution
