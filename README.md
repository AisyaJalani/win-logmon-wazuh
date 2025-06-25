# Windows Log Monitoring & Alerting with Wazuh

**Objective:**  
Set up Wazuh Manager and Windows Agent to detect suspicious Windows events; customize alert rules; simulate real SOC workflows.

---

## 1. Environment Setup
See detailed instructions in `setup_guide/`:
- `01_install_wazuh_manager.md` – Install Wazuh Manager on Ubuntu
- `02_install_wazuh_agent_windows.md` – Install & configure Windows agent

---

## 2. Simulated Test Cases
Each test case includes the actions, events triggered, and dashboard screenshots:
- `failed_logon_4625.md`
- `user_creation_4720.md`
- `service_creation_7045.md`

---

## 3. Configuration Files
- `config/local_rules.xml`  
  - Custom rules for failed logins, suspicious processes, etc.
- `config/sample_agent-conf/ossec.conf`  
  - Example agent config for monitoring Windows event channels

---

## 4. Screenshots
Screenshots illustrating results and alerts are in `screenshots/`:
- `dashboard_failed_login.png`
- `dashboard_custom_rule.png`
- `agent_event_view.png`

---

## 5. Summary Report
High-level summary, analysis, and SOC response suggestions in `summary_report.pdf`

---

## 📁 How to Use This Repo
1. Clone the repo.
2. Follow `setup_guide` to build your environment.
3. Run each test case step-by-step in `test_cases/`.
4. Compare your results against screenshots.
5. Customize or expand rules in `config/local_rules.xml` as needed.

---

## 📄 License
[MIT](LICENSE)
