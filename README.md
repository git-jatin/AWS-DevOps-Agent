# AWS-DevOps-Agent
This project demonstrates how frontier AI agents leverage multi-agent frameworks to drastically reduce Mean Time to Resolution (MTTR) by abstracting repetitive diagnostic toil.


**The Architecture & Setup**
I wanted to see exactly how effectively a frontier AI agent could transition from a passive observer to an active, logical troubleshooting teammate.

The Target Infrastructure: Built a CloudFormation stack provisioning a t3.micro EC2 instance in a public subnet, backed by a CloudWatch alarm calibrated to trigger the moment CPU utilization sustained a metric >70%.

The Agent Space: Deployed an isolated AWS DevOps Agent Space, granting it secure IAM discoverability permissions to map the active resource topology.

The Incident Simulation: Connected via EC2 Instance Connect and fired a multithreaded CPU stress testing script (cpu-stress-test.sh), pinning the cores and forcing an immediate metric spike to 100%.


<img width="497" height="1024" alt="image" src="https://github.com/user-attachments/assets/72efe746-9c29-487c-9bb1-a15dc580a27b" />


#Screenshots

<img width="1440" height="900" alt="Screenshot 2026-05-26 at 6 29 29 PM" src="https://github.com/user-attachments/assets/e992b3a8-33ea-4b1b-b098-5cf360c49318" />
<img width="1440" height="900" alt="Screenshot 2026-05-26 at 6 31 19 PM" src="https://github.com/user-attachments/assets/a862a0a6-af28-46da-a2bb-83a6ac23fca7" />
<img width="1440" height="900" alt="Screenshot 2026-05-26 at 7 03 30 PM" src="https://github.com/user-attachments/assets/e4a58d74-e7ce-41ee-8351-a02f0efbb9e2" />
<img width="1440" height="900" alt="Screenshot 2026-05-26 at 7 03 56 PM" src="https://github.com/user-attachments/assets/6e16ca70-25cc-4e64-83fc-4bbf5f26dee6" />
<img width="1440" height="900" alt="Screenshot 2026-05-26 at 7 04 04 PM" src="https://github.com/user-attachments/assets/2e20eb81-a993-42e9-9106-5041abc96c7e" />

<img width="1440" height="900" alt="Screenshot 2026-05-26 at 7 04 14 PM" src="https://github.com/user-attachments/assets/908a5c98-7a02-4eb9-bc4e-22f111f8c970" />

<img width="1440" height="900" alt="Screenshot 2026-05-26 at 7 04 25 PM" src="https://github.com/user-attachments/assets/dc2f0c32-1cb5-49b6-aa75-0cf302910012" />

<img width="1440" height="900" alt="Screenshot 2026-05-26 at 7 04 28 PM" src="https://github.com/user-attachments/assets/919498a1-bd29-42e0-bd3e-c8d59157333e" />

<img width="1440" height="900" alt="Screenshot 2026-05-26 at 7 04 32 PM" src="https://github.com/user-attachments/assets/4c1d82b0-8f3f-4bbc-9cfc-c860bb2edd33" />

<img width="1440" height="900" alt="Screenshot 2026-05-26 at 7 04 45 PM" src="https://github.com/user-attachments/assets/d2c18729-29f9-496a-8e99-205cecb13c1d" />

<img width="1440" height="900" alt="Screenshot 2026-05-26 at 7 04 48 PM" src="https://github.com/user-attachments/assets/e54e7b55-9dc6-4700-831f-6c6a2e8128d2" />


