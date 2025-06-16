# DP100 Renewal Exam – Full Question & Answer Bank (2025)

This file contains all 25 renewal exam questions with answers and brief explanations.

Each entry is exam-aligned and phrased to support fast GitHub-based review.
---
### Question 1
**Q:** You manage an Azure Machine Learning workspace. You create a datastore that has an existing Azure Blob Storage account. The account is configured to use identity-based authentication. You need to authenticate a user to the storage account. What should you use?
**✅ A:** `Microsoft Entra ID`
**🧠 Explanation:** For identity-based authentication in Azure Storage accounts, Microsoft Entra ID (formerly Azure AD) is the correct mechanism. Account keys or SAS are key-based, not identity-based.

### Question 2
**Q:** You manage an Azure Machine Learning workspace. You create a datastore in Azure Machine Learning. You need to access the datastore from a notebook running in the workspace. Which protocol should you use to access the datastore?
**✅ A:** `abfss`
**🧠 Explanation:** abfss (Azure Blob File System Secure) is the protocol used to securely access Azure Data Lake Gen2-compatible storage in notebooks.

### Question 3
**Q:** You manage an Azure Machine Learning workspace. You create a Python script. You want to run the script as a job. You set the input parameter input_data to an MLTable. What should you do to read the data?
**✅ A:** `Use the load method to read the data`
**🧠 Explanation:** The MLTable asset is read via the `load()` method in Azure ML SDK; direct use of `read_csv()` won't recognize Azure ML's data asset context.

### Question 4
**Q:** You manage an Azure Machine Learning workspace. You need to experiment on a small subset of training data in a notebook. Which compute target should you select?
**✅ A:** `Compute instance`
**🧠 Explanation:** Compute instances are dedicated VMs designed for interactive workloads like notebooks and small-scale experimentation.

### Question 5
**Q:** You manage an Azure Machine Learning workspace. You save your production-ready code as a script. You must configure a GPU compute cluster to run the script using the Azure ML Python SDK v2. You need to specify the virtual machine type of each node within the cluster. Which parameter should you define?
**✅ A:** `size`
**🧠 Explanation:** `size` defines the VM SKU (e.g., Standard_NC6) used in compute clusters. It’s required for specifying node configuration.
