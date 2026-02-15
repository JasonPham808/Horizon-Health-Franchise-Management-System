<img width="275" height="183" alt="image" src="https://github.com/user-attachments/assets/70bad7c0-4a7a-4798-b8f1-37fcfe5bb9e4" />

# Project Overview
This project presents the analysis and design of a mobile application to enhance Horizon Health’s franchise management. The solution leverages UML modeling, business process modeling, and AI-enhanced workflows to streamline operations across franchisees, administrators, and external systems.
The application focuses on:
- Efficient lead handling and allocation
- Seamless client servicing and conversion
- Automated invoicing and financial management
- Improved operational coordination among stakeholders
# Key Features 🔑 
- Use Case Diagram: Maps interactions between franchisees, call centre administrators, clients, and supporting departments.
- Sequence Diagram: Models end-to-end workflows from lead generation to invoicing, including exception scenarios.
- Domain Class Diagram: Defines system entities (Franchisee, Client, Lead, Service, Invoice) and their relationships for robust data management.
- Business Process Models (BPMs):
- Lead Generation
- Lead Transfer/Cancellation & Client Servicing
- Invoicing Clients
# Outcomes 🎯 
- Operational Efficiency: Franchisees gain a unified platform to manage leads, services, and invoices.
- Automation & Accuracy: Reduced manual effort with automated validation, invoicing, and reporting.
- Scalability: Supports Horizon Health’s franchise growth with structured processes and external system integration.
- Transparency & Accountability: Clear role delineation across administrators, franchisees, and managers.
- Enhanced Client Experience: Faster service delivery and accurate billing improve client satisfaction.
# Contents 📂 
## 1. Use Case Diagram Analysis
<img width="737" height="826" alt="image" src="https://github.com/user-attachments/assets/887e9845-ed00-4be1-9cd5-d05707776d56" />

Actors in the System
• 	Call Centre Administrator – Allocates, transfers, or cancels client leads.
• 	Client/Patient – Receives health services and communicates with the system.
• 	Franchisee – Main user; manages leads, converts clients, delivers services, creates invoices, and handles business obligations.
• 	Accounting System – External system for invoices and payments.
• 	Training Department – Provides manuals and answers franchisee queries.
• 	Operations Manager – Controls lead allocation based on qualifications/availability.
• 	Marketing Manager – Monitors performance and generates sales reports.

<img width="793" height="560" alt="image" src="https://github.com/user-attachments/assets/7366b1db-b495-499a-9e84-961578fb3202" />

Key Process Flows
- Franchisee Account & Allocation
- Franchisee registers, updates availability, views leads, creates services, and generates invoices.
- System validates, records updates, and sends invoices to clients and accounting.
- Lead Management
- Leads are assigned, viewed, and converted into clients.
- Services are scheduled; the Operations Manager applies restrictions.
- Banking & Accounting
- Payments recorded, monthly invoices generated, and financial reports produced.
- Training Updates
- Manuals distributed; franchisee queries answered by the Training Department.

## 2. Sequence & Domain Class Diagram
<img width="782" height="714" alt="image" src="https://github.com/user-attachments/assets/65715739-5c4e-4cc6-866b-ac5e64fbdc04" />

Sequence Diagram Summary – Key Flow
Actors Involved:
- Operations Manager – Controls lead allocation
- Franchisee – Registers, verifies accounts, manages services and invoices
- Client/Patient – Receives services and may request an early invoice
- Management System – Responds to all actions and updates records
Main Flow:
- Lead Restriction – Operations Manager sends restriction command to the system
- Franchisee Onboarding – Franchisee registers and requests verification
- Service Setup – Franchisee creates the service and confirms with the client
- Invoice Generation – Triggered after service or optionally before (if requested)
- System Response – Sends confirmations and updates records
Optional Flow:
- If the client requests an early invoice → system generates and sends the invoice before service completion
Purpose:
- Shows how actors interact with the system in real time
- Highlights both standard and optional paths
- Ensures clarity in franchisee operations from registration to invoicing
<img width="735" height="704" alt="image" src="https://github.com/user-attachments/assets/267a185c-b283-435d-9e4f-433cbba20c06" />

Purpose:
Represents the static structure of the Horizon Health mobile app, showing how franchisee operations, lead management, service delivery, and invoicing are connected.
Key Classes:
• 	Franchisee – Registers, manages leads, converts clients, creates services, and invoices.
• 	Call Centre Administrator – Assigns, views, and cancels leads.
• 	Client – Receives services; linked to multiple leads.
• 	Lead – Tracks potential opportunities (status, territory).
• 	Service – Represents scheduled or completed service delivery.
• 	Invoice – Handles financial transactions and payment status.
• 	Accounting System – External system for invoice processing.
• 	Operations Manager – Restricts lead allocation based on rules.
Relationships:
• 	Leads connect franchisees and clients.
• 	Each service links to one invoice; clients may have multiple leads/services.
• 	External systems integrate for accounting and reporting.
Outcome:
Provides a clear, scalable model of how actors and processes interact. Supports automation, financial tracking, and ensures the app design is structured, traceable, and ready for implementation.
## 3. Business Process Models
<img width="685" height="838" alt="image" src="https://github.com/user-attachments/assets/f9c478e0-0641-49d8-a525-bc5f48bc95f5" />

The system workflows are captured in three BPMs to ensure clear roles, automation, and accountability:
- Lead Generation
- Call Centre Admin enters lead details.
- System validates franchisee (territory, registration, availability).
- Leads are either allocated or flagged for reallocation.
- Lead Transfer / Cancellation & Client Servicing
- Admin cancels or transfers leads if the franchisee is not eligible.
- Franchisee contacts leads, converts them to clients, and schedules services.
- Optional: Pre‑service invoice if requested by client.
- Client Invoicing
- Triggered after service completion.
- System generates invoice, syncs data, and sends to Accounting.
- Client receives invoice and completes payment.
Supporting Processes:
- Accounting System – Deducts monthly fees and reconciles payments.
- Marketing Manager – Uses invoice data for sales and revenue reporting.
Outcome:
These BPMs streamline lead handling, client servicing, and invoicing, ensuring efficiency, transparency, and financial accuracy across Horizon Health’s franchise network.
## 4. BACCM Analysis
<img width="730" height="487" alt="image" src="https://github.com/user-attachments/assets/a473ab81-64b5-491d-a222-6f20a441d396" />

Figure 5: BACCM-based mind map for the problem space exploration
Change
- Shift from manual operations to a unified, AI‑enhanced mobile app.
- Digital support for franchisees (leads, services, invoicing).
- Automation of admin tasks and remote healthcare coordination.
Need
- Franchisees: efficient tools for daily operations.
- Horizon Health: oversight of activity and income.
- Clients: seamless service access and communication.
- Training/Marketing: structured engagement and reporting.
Solution
- Mobile app modules: onboarding, lead management, scheduling, invoicing, reporting, AI support.
- Integration with external accounting systems.
- Secure access, territory restrictions, tailored training.
Stakeholders
- Primary: Franchisees, Clients, Operations, Training, Marketing, Accounts.
- Supporting: Call Centre Admins, Accounting Systems.
- Indirect: Regulators, prospective clients.
Value
- Greater efficiency and scalability.
- Better franchisee tools → improved client service and compliance.
- Faster insights for decision‑making.
- Stronger brand reputation and profitability.
Context
- Business expansion via franchise model.
- Operating in regulated healthcare.
- Clients expect personalized, efficient care.
- Franchisees are semi‑independent but aligned with central processes.



