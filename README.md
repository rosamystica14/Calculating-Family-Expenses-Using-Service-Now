# Calculating-Family-Expenses-Using-Service-Now


## 📌 Project Overview
The **Family Expenses Management** application is a custom ServiceNow table-based project designed to track and manage daily or monthly family expenses.  
It allows users to record, update, and monitor expenses efficiently within the ServiceNow platform.

---

## 🎯 Features
- Create, read, update, and delete (CRUD) expense records  
- Track expenses by **date, amount, and description**  
- Simple list and form views for easy data entry  
- Configurable table columns  
- Supports record-level access using ServiceNow ACLs  
- Extends the base `Task` table (optional) for better integration with workflows  

---

## 🧩 Table Details

| Field Name       | Type     | Description                         |
|------------------|----------|-------------------------------------|
| **Number**       | String   | Unique identifier for each record   |
| **Amount**       | Integer  | Expense amount                      |
| **Date**         | Date     | Date of the expense                 |
| **Expense Details** | String | Description or category of expense  |

**Table Name:** `u_st_family_expenses`  
**Label:** Family Expenses  
**Application:** Global  
**Extends Table:** (Optional) `Task`  

---

## ⚙️ Configuration Steps

1. Navigate to **System Definition → Tables**  
2. Click **New** → Create table **Family Expenses**
3. Add columns:
   - Number (String)
   - Amount (Integer)
   - Date (Date)
   - Expense Details (String)
4. (Optional) Set **Extends table** = `Task` for workflow and state fields  
5. Configure **List Layout** → Add the columns you created  
6. Configure **Form Layout** → Add fields in this order:
   - Label
   - Name
   - Extends table
   - Application
   - Show in Menu
   - Remote Table
7. Click **Update** and verify the form.

---

## 🧠 Usage
1. Open the **Family Expenses** table under the Application menu.  
2. Click **New** to add an expense record.  
3. Fill in all fields and save.  
4. Use the list view to monitor expenses or edit existing entries.

---


## 🧑‍💻 Technologies Used
- ServiceNow Platform
- GlideRecord (for backend scripting)
- UI Policy & Client Script (optional)
- Global Application Scope

---

## 🧱 Future Enhancements
- Add expense category dropdown (Food, Bills, Travel, etc.)
- Generate monthly expense reports
- Add approval workflow for high-value expenses
- Integrate with Service Portal for user-friendly UI

---

## 📚 Author
**Name:** [Rosa Mystica M , Sahaya Shiny Vaz A , Santhiya M , Snowfa P Rayer J] 
**Platform:** ServiceNow Developer Instance   

---
