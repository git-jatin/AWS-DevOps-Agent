# AWS-DevOps-Agent
This project demonstrates how frontier AI agents leverage multi-agent frameworks to drastically reduce Mean Time to Resolution (MTTR) by abstracting repetitive diagnostic toil.


**The Architecture & Setup**
I wanted to see exactly how effectively a frontier AI agent could transition from a passive observer to an active, logical troubleshooting teammate.

The Target Infrastructure: Built a CloudFormation stack provisioning a t3.micro EC2 instance in a public subnet, backed by a CloudWatch alarm calibrated to trigger the moment CPU utilization sustained a metric >70%.

The Agent Space: Deployed an isolated AWS DevOps Agent Space, granting it secure IAM discoverability permissions to map the active resource topology.

The Incident Simulation: Connected via EC2 Instance Connect and fired a multithreaded CPU stress testing script (cpu-stress-test.sh), pinning the cores and forcing an immediate metric spike to 100%.


<img width="497" height="1024" alt="image" src="https://github.com/user-attachments/assets/72efe746-9c29-487c-9bb1-a15dc580a27b" />
