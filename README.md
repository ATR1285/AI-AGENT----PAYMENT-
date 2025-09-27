# AI Payment Reminder Agent – Finance & Banking  

A workflow automation project developed by **Team BugSlayers** (Dr. SNS Rajalakshmi College of Arts and Science, Coimbatore-20) to streamline **payment reminders** in the finance and banking sector using AI and workflow automation.  

***

### Team Details  
- **Team Name**: BugSlayers  
- **Members**: Richard A T, Praveen Kumar, Niranjan, Vignesh Ram, Vishwa  

***

### Problem Statement  
Timely payment collection is critical to ensure healthy cash flow. However, manual reminder processes are:  
- Time-consuming and error-prone  
- Prone to inconsistencies in record management  
- Inefficient in separating paid vs. unpaid customers  
- Dependent on staff for regular reminders  

Without automation, many customers miss reminders, and staff spend excessive time on manual updates.  

***

### Proposed Solution  
We developed an **AI-powered Payment Reminder Agent** that:  
- Reads customer payment data (from Google Sheets)  
- Automatically identifies unpaid customers  
- Sends reminder emails with due date and payment details  
- Updates records in real time  
- Stores paid customer records separately for reference  

***

### Workflow  
1. **Data Input**  
   - Customer payment records (Name, Email, Due Date, Amount, Payment Status) stored in Google Sheets.  

2. **AI Processing**  
   - Reads payment data from Google Sheets.  
   - Flags unpaid customers (Payment Status = Pending).  
   - Moves paid entries to a separate **Paid Customers** sheet.  

3. **Email Reminder**  
   - Sends automated reminder emails to unpaid customers.  
   - Includes Payment Amount, Due Date, and instructions.  

4. **Sheet Update**  
   - Updates Payment_Status in Google Sheets to reflect “Reminder Sent.”  
   - Archives paid entries to a dedicated sheet.  

***

### Technology Stack  
- **n8n** – Workflow automation platform  
- **Google Sheets** – Customer data storage & status tracking  
- **Gemini 1.5 (Flash)** – AI Agent Node for payment status logic  
- **Email Send Node** – Automatic reminder emails  
- **Append/Update Row Node** – Real-time update of Google Sheets  

***

### Outcome  
- Reduced manual effort for staff in chasing payments  
- Improved **payment completion rates** through timely reminders  
- Accurate separation of **paid vs. unpaid customers**  
- Fully automated system – requires **no manual intervention** once set up  

***

### System Flow  

**Database (Google Sheet) → AI Processing → Reminder Emails → Updated Records → Paid Customer Archive**  

**Example Output:**  
- **Paid Customers** moved to a separate archive  
- **Pending Customers** receive automated reminders  

***

### Future Enhancements  
- Integration with **WhatsApp/SMS notifications** alongside email  
- Dashboard view for real-time payment tracking  
- Multi-bank integration for large-scale deployments  

***

### License  
This project is licensed under the MIT License.  

***

Would you like me to also add a **diagram (MermaidJS flowchart code)** inside the README so GitHub renders a nice **workflow visualization** directly?
