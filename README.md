# Use-Azure-Synapse-Link-for-Azure-Cosmos-DB
Azure Synapse Link for Azure Cosmos DB is a cloud-native hybrid transactional analytical processing (HTAP) technology that enables you to run near-real-time analytics over operational data stored in Azure Cosmos DB from Azure Synapse Analytics.


## ⭐ Objective
In this lab, you will learn how to use Azure Synapse Analytics to perform near real-time analytics on operational data stored in Azure Cosmos DB using Azure Synapse Link. This hybrid transactional and analytical processing (HTAP) capability eliminates the need to move data to a separate data warehouse.

---

## 📘 Learning Outcomes
- Integrate Azure Cosmos DB with Azure Synapse Link  
- Query and analyze data using Synapse Studio  
- Access Cosmos DB data with serverless SQL pools  
- Understand and apply HTAP architecture  

---

## 🔧 Prerequisites
- An active Azure subscription  
- Azure Cosmos DB (Core/SQL API)  
- Azure Synapse Analytics workspace  

---

## 🚀 Steps

### 1. Create Azure Cosmos DB
- In Azure Portal, create a new Cosmos DB account (SQL API).
- Enable the "Analytical Store" feature.

### 2. Enable Azure Synapse Link
- Activate Synapse Link on your Cosmos DB account.
- Ensure the analytical store is enabled for the target database and containers.

### 3. Connect via Synapse Studio
- Open Synapse Studio.
- Go to "Manage > Linked services" and connect to your Cosmos DB account.
### 4. Query Data with Serverless SQL Pool
``sql
SELECT TOP 10 *
FROM OPENROWSET(
    'CosmosDB',
    'Account=<account>;Database=<database>;Collection=<collection>',
    'SELECT * FROM c') AS documents '

## 📊 Real-World Scenario
In a retail system, customer orders are stored in Cosmos DB. With Azure Synapse Link, you can query those order records in near real time to monitor trends, forecast demand, and make data-driven inventory decisions without ETL processes.

---
## Screenshots

![lab14](https://github.com/user-attachments/assets/3c0b60ff-7a16-4dd9-8c43-2eff81e99af8)
![lab142](https://github.com/user-attachments/assets/c5b0e243-051b-4933-96a5-05e9b6b8a38e)
![lab143](https://github.com/user-attachments/assets/7365e072-47ea-4e6a-9001-28fc7c68dfdc)
![lab144](https://github.com/user-attachments/assets/c7b2f1c4-0203-45f9-b55b-f5cf1881cd28)
![lab145](https://github.com/user-attachments/assets/47a1c243-344f-49b8-9935-cc0cedb022c5)
![lab146](https://github.com/user-attachments/assets/44ebfc6a-d59a-4a18-9779-fb612d36601a)
![lab147sales](https://github.com/user-attachments/assets/a058de13-c075-494c-9bad-e7be4847fbb0)
![lab148](https://github.com/user-attachments/assets/6ff3dca1-792c-4565-9742-cacccf59483f)
![lab148code2](https://github.com/user-attachments/assets/a47ecafb-d263-4f58-bbfc-c5814a6cab42)
![lab148sql](https://github.com/user-attachments/assets/eadc9da8-db2e-48e1-bb96-89b2dd4f2649)
![lab148sql2](https://github.com/user-attachments/assets/d81b1bfa-10d0-4a8c-941f-e70644020abe)
![lab148keys](https://github.com/user-attachments/assets/5b390ac0-562a-45de-b45d-6c78781a806d)
![lab149credential](https://github.com/user-attachments/assets/62c749ee-6e42-4718-8edf-978d26dafe72)
![lab149credential2](https://github.com/user-attachments/assets/da59e026-aac3-4165-b167-c371fa6b9a87)
![lab149credential3](https://github.com/user-attachments/assets/63455e7c-e493-4401-b04a-57493aeca9c0)
![lab149newitem](https://github.com/user-attachments/assets/569a7c7e-cf8d-48ee-817c-cac1df41a195)
![lab149newitem2](https://github.com/user-attachments/assets/062f1b80-1fc2-481a-9080-32487d53d8a1)

  
