# MS_Fabric_LAB_5
# Create and Use Dataflows Gen2 in Microsoft Fabric

This project demonstrates how to create and use **Dataflows Gen2** in **Microsoft Fabric** to extract, transform, and load (ETL) data into a **Lakehouse** for analytical purposes.

The lab is designed as an introductory exercise, providing hands-on experience with the core components of Fabric's data engineering tools without the complexity of a full enterprise scenario.

## 📚 Objective

- Learn how to build a workspace in Microsoft Fabric.
- Create a Lakehouse as a data destination.
- Set up a Dataflow Gen2 using Power Query Online.
- Perform basic data transformations.
- Load the transformed data into the Lakehouse.
- Automate the data integration process using a Pipeline.

## 🛠️ Steps Completed

### 1. Workspace Creation
- Created a new workspace in Microsoft Fabric, enabling trial capacity.

### 2. Lakehouse Setup
- Built an empty Lakehouse to serve as a storage location for structured data.

### 3. Dataflow Gen2 Creation
- Set up a new Dataflow Gen2 from a public CSV file:
  - Data source: [Orders.csv](https://raw.githubusercontent.com/MicrosoftLearning/dp-data/main/orders.csv)
  - Connection type: Anonymous
- Performed transformations in Power Query:
  - Added a calculated column `MonthNo` extracting the month from the `OrderDate` field.

### 4. Configure Dataflow Output
- Configured the Dataflow to write the data directly into the previously created Lakehouse.
- Mapped the output to create a table named **Orders**.

### 5. Pipeline Creation
- Designed a Pipeline to automate the execution of the Dataflow.
- Scheduled and manually triggered the Pipeline to run and load the data into the Lakehouse.

### 6. Validation
- Refreshed the Lakehouse.
- Verified the presence of the **Orders** table containing the processed dataset.

## 💡 Key Learnings

- **Microsoft Fabric Dataflows Gen2** enable seamless ETL operations integrated into Fabric's unified environment.
- **Power Query Online** provides a user-friendly interface for building transformation logic without writing code.
- **Lakehouse architecture** supports scalable and structured storage for analytical workloads.
- **Pipelines** in Fabric streamline the orchestration of data movements and transformations.

## ⏱️ Duration

Approximate time to complete: **30 minutes**

## 🔗 References

- [Microsoft Fabric Home](https://app.fabric.microsoft.com/)
- [Official Documentation - Microsoft Fabric](https://learn.microsoft.com/fabric/)
- [Orders Dataset Source](https://raw.githubusercontent.com/MicrosoftLearning/dp-data/main/orders.csv)

---

**Note:**  
This lab exercise is an excellent entry point for professionals looking to explore Microsoft Fabric’s data engineering capabilities, providing a strong foundation for future advanced projects.

