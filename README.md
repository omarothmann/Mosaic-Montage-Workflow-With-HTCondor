# M101 Mosaic Montage Workflow with HTCondor
For this project, a HTCondor cluster consisting of 3 virtual machines running on  Amazon Linux 2 AMI (HVM) - Kernel 5.10 that was setup on Amazon Web Service’s Elastic  Computing Cloud (EC2) servers. The three virtual machines master, scheduler and worker was set up and paired with Network File System (NFS) before executing the workflow. The master and the scheduler shares a NFS server-client relationship respectively.

This setup was created to run a Montage m101 Mosaic workflow  where the output will be two mosaics of m101 and their corresponding area images. A linear  DAGMan workflow and a parallelized DAGMan workflow were created and executed to measure  the performance and efficiency of the workflows to see which one is better.



## :bulb: Running the program

To run the Linear DAG Workflow, type the following command:
```
$ condor_submit_dag run.dag
```
To run the Parallelized DAG Workflow, type the following command:
```
$ condor_submit_dag runparallel.dag
```
To check the status and progress of the job submisson, type the following command:
```
$ ls
$ condor_q
$ condor_q -nobatch
```
## 🎥 Demonstration Video

[![Demo](https://raw.githubusercontent.com/omarothmann/Mosaic-Montage-Workflow-With-HTCondor/main/presentation.JPG)](https://www.youtube.com/watch?v=tRkz9I3lH4c&ab "M101 Mosaic Montage Workflow with HTCondor & DAGManr")





