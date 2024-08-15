### STIG Compliance Automation Project

### Project Overview
This project demonstrates the automation of Security Technical Implementation Guide (STIG) compliance for a Linux environment. The goal is to harden the system according to Department of Defense (DoD) security standards, ensuring that it is compliant with industry best practices.

### Objectives
- **Automate the application of STIGs** to a Linux system.
- **Validate compliance** using automated scripts.
- **Generate reports** to track compliance status.
- **Educate** others on the importance and application of STIGs in cybersecurity.

### Project Structure
- **`/scripts/`**: Contains automation scripts for applying STIG configurations and checking compliance.
  - `apply_stigs.sh`: A Bash script to apply STIGs to a Linux system.
  - `check_compliance.sh`: A Bash script to validate the system's compliance with STIGs.
  
- **`/checklists/`**: Includes sample STIG checklists and documentation.
  - `stig_checklist.txt`: A sample checklist with comments explaining the hardening steps.
  
- **`/configs/`**: Contains example configurations for different services and settings.
  - `sshd_config`: A hardened SSH configuration file following STIG guidelines.
  - `sysctl.conf`: Kernel parameters set according to STIG requirements.

### Automation Process
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/STIG-Compliance-Automation.git
   cd STIG-Compliance-Automation
2. **Apply STIGs:**
- Run the apply_stigs.sh script to automatically apply the necessary configurations:
  ```bash
    sudo bash scripts/apply_stigs.sh
- **This script will**:
  - Disable unnecessary services
  - Enforce strong password policies
  - Set appropriate file permissions
  - Configure network parameters
3. **Check Compliance:**
  - Run the check_compliance.sh script to validate the system’s compliance:
    ```bash
    sudo bash scripts/check_compliance.sh
- **This script will**:
  - Compare the current system settings against the STIG requirements.
  - Generate a report highlighting compliant and non-compliant areas.
  
