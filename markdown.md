## 1 - Screenshots of the VM creation and cost monitoring processes in both Azure and GCP
### **Azure**
<img width="1470" alt="Screenshot 2024-09-11 at 14 54 28" src="https://github.com/user-attachments/assets/b18fb4b0-b8be-4adc-8a9c-c7e08dfe44ed">
<img width="1470" alt="Screenshot 2024-09-12 at 17 15 21" src="https://github.com/user-attachments/assets/425dd4cd-caac-4f62-82d7-e2d07d744818">

### **GCP**
<img width="1470" alt="Screenshot 2024-09-11 at 15 03 01" src="https://github.com/user-attachments/assets/3eae2e1d-3866-4290-943b-59b68d34acaf">
<img width="1470" alt="Screenshot 2024-09-12 at 17 13 01" src="https://github.com/user-attachments/assets/3de60b9f-398b-4231-ba7b-eea55c6e2e31">


## 2 - Compare the costs of running a VM in Azure versus GCP. Consider factors such as the configuration used, the duration for which the VM was active, and any differences in cost visibility between the platforms

| Configuration    | Azure   | GCP    
| ---------------- | ------- | ----------
| OS  | Linux     | Linux
| VM architecture  | x64     | x86/64
| Size            | Standard D2s v3 (2 vcpus, 8 GiB memory)| 10 GB
| Zone            | North Europe    | US Central
| Time run         | ≈15 min     | ≈15 min
| Cost         | $0.3     | $0.02

- Azure cost $0.3 (storage, virtual network, and VM) and GCP $0.02 (computing engine). More details can be seen in the above screenshots.
- Both platforms provide various series and custom machine types. 
- Azure and GCP have pay-as-you-go. Azure has reserved instances (1 or 3 year commitments), while GCP has sustained use discounts or committed use contracts.
- In terms of billing granularity, Azure has per-minute billing and GCP has per-second billing with a 1 minute minimum. 
- Azure offers detailed insights with Azure Cost Management + Billing, and GCP provides cost management with Cloud Billing. 
- Both have pricing calculators for customization and cost estimation. 


## 3 - Reflect on the ease of starting, stopping, and monitoring VMs on each platform. Which platform did you find more intuitive or user-friendly? Why?
### **Azure**
In general, Azure's portal is clear and intuitive enough, though there are so many components that it can feel overwhelming for a beginner. 
VMs can easily be started and stopped with the appropriate icons at the top of the "Overview" page. 
Azure CLI and PowerShell also make it easy to script VM operations, which is handy for automation.
Lastly, Azure Monitor is a thorough solution that provides detailed metrics, logs, and alerts, with customizable dashboards. 
### **GCP**
GCP's interface is straightforward and allows for quick actions. 
Starting and stopping VMs can done by clicking on the "three dot" hamburger icon next to the VMs name. 
Additionally, the gcloud command-line is a powerful and straightforward tool for managing VM lifecycle operations.
## **Final Verdict**
Overall, I found GCP's platform to be more intuitive and user-friendly for those who are unfamiliar with either platform. 
Azure's portal had so many features and details that it became overwhelming. 
However, because of its intricacy, it would be better for users who need in-depth customization. 
GCP's interface is much simpler and cleaner, making it easier to navigate. I would say it probably has a lower learning curve than Azure. 
Both platforms are powerful, but the best option lies in a person or team's specific needs and preferences. 
