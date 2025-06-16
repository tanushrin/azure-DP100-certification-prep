# DP100 Renewal Exam – Full Question & Answer Bank (2025)

This file contains all 25 renewal exam questions with answers and brief explanations.

---
### Question 1
**Q:** You manage an Azure Machine Learning workspace. You create a datastore that has an existing Azure Blob Storage account. The account is configured to use identity-based authentication. You need to authenticate a user to the storage account. What should you use?

**✅ A:** `Microsoft Entra ID`

**Explanation:** For identity-based authentication in Azure Storage accounts, Microsoft Entra ID (formerly Azure AD) is the correct mechanism. Account keys or SAS are key-based, not identity-based.

### Question 2
**Q:** You manage an Azure Machine Learning workspace. You create a datastore in Azure Machine Learning. You need to access the datastore from a notebook running in the workspace. Which protocol should you use to access the datastore?

**✅ A:** `abfss`

**Explanation:** abfss (Azure Blob File System Secure) is the protocol used to securely access Azure Data Lake Gen2-compatible storage in notebooks.

### Question 3
**Q:** You manage an Azure Machine Learning workspace. You create a Python script. You want to run the script as a job. You set the input parameter input_data to an MLTable. What should you do to read the data?

**✅ A:** `Use the load method to read the data`

**Explanation:** The MLTable asset is read via the `load()` method in Azure ML SDK; direct use of `read_csv()` won't recognize Azure ML's data asset context.

### Question 4
**Q:** You manage an Azure Machine Learning workspace. You need to experiment on a small subset of training data in a notebook. Which compute target should you select?

**✅ A:** `Compute instance`

**Explanation:** Compute instances are dedicated VMs designed for interactive workloads like notebooks and small-scale experimentation.

### Question 5
**Q:** You manage an Azure Machine Learning workspace. You save your production-ready code as a script. You must configure a GPU compute cluster to run the script using the Azure ML Python SDK v2. You need to specify the virtual machine type of each node within the cluster. Which parameter should you define?

**✅ A:** `size`

**Explanation:** `size` defines the VM SKU (e.g., Standard_NC6) used in compute clusters. It’s required for specifying node configuration.

### Question 6
**Q:** You run a batch inference pipeline. You want to ensure the output is versioned and reusable in downstream steps. Which Azure ML class should you use?

**✅ A:** `OutputFileDatasetConfig`

**Explanation:** OutputFileDatasetConfig helps manage outputs in pipeline steps, enabling reuse and versioning of results.

### Question 7
**Q:** You are configuring a YAML job in Azure ML CLI v2. You must submit a job to a compute target and specify the environment and code directory. Which YAML keys are mandatory?

**✅ A:** `compute, environment, code, command`

**Explanation:** These keys define where the job runs (`compute`), the software environment, the code path, and what to execute.

### Question 8
**Q:** You are evaluating a model with Responsible AI dashboard in Azure Machine Learning. You want to analyze how slight changes in features affect the model’s output. Which feature should you use?

**✅ A:** `Counterfactuals`

**Explanation:** Counterfactual analysis explains how minimal changes in input features could change predictions — ideal for debugging and fairness checks.

### Question 9
**Q:** You’re using the Azure ML Responsible AI dashboard and want to understand errors across different data segments. What tool should you use?

**✅ A:** `Error analysis`

**Explanation:** Error analysis helps identify which data cohorts (groups) are producing poor results and why.

### Question 10
**Q:** You want to deploy a model to a real-time endpoint using CLI v2. What command should you use?

**✅ A:** `az ml endpoint create --file endpoint.yml`

**Explanation:** This CLI command creates a managed online endpoint for real-time inference using the specified YAML file.

### Question 11
**Q:** You want to track data drift over time in Azure Machine Learning. What is required to enable drift monitoring?

**✅ A:** `Baseline dataset`

**Explanation:** A baseline dataset is needed to compare incoming data distributions and detect significant changes over time.

### Question 12
**Q:** You're designing an Azure ML pipeline. You want to read a dataset registered in the workspace and pass it as input to a training step. What method do you use?

**✅ A:** `mlclient.data.get()`

**Explanation:** `mlclient.data.get()` retrieves a registered dataset or data asset for use in training or other steps.

### Question 13
**Q:** Which Python library would you use for model explainability in Azure ML’s Responsible AI dashboard?

**✅ A:** `InterpretML`

**Explanation:** InterpretML supports explainability visualizations such as SHAP values, tree-based interpretations, etc.

### Question 14
**Q:** You want to trigger a model retraining pipeline upon detecting data drift in production. What approach should you take?

**✅ A:** `Use Azure ML pipelines triggered via Azure Event Grid or Logic Apps`

**Explanation:** Azure ML doesn’t auto-retrain on drift. You must set up automated retraining pipelines using external triggers like Event Grid or Logic Apps.

### Question 15
**Q:** You configure a data drift monitor. Which metric determines if a drift occurred?

**✅ A:** `Statistical threshold`

**Explanation:** Drift detection is based on statistical tests (e.g., KS Test) and triggers when deviations exceed defined thresholds.

### Question 16
**Q:** Which Azure ML visual highlights SHAP values across features to show their contribution to predictions?

**✅ A:** `Feature importance plot`

**Explanation:** The SHAP-based feature importance plot shows how much each feature impacts the model’s output.

### Question 17
**Q:** You want to audit your AI system for fairness across age and gender groups. Which tool should you use?

**✅ A:** `Fairlearn`

**Explanation:** Fairlearn is designed for fairness assessment across sensitive attributes such as age, gender, ethnicity, etc.

### Question 18
**Q:** In Responsible AI dashboard, which visual helps show model performance across defined cohorts?

**✅ A:** `Error heatmap`

**Explanation:** Error heatmaps show how error rates vary across combinations of categorical features or cohort groups.

### Question 19
**Q:** Which dashboard in Azure ML supports debugging model behavior by analyzing prediction errors and feature contributions?

**✅ A:** `Responsible AI dashboard`

**Explanation:** The Responsible AI dashboard combines multiple interpretability tools including SHAP, error analysis, counterfactuals, etc.

### Question 20
**Q:** You're using Azure ML dataset monitor and detect frequent alert notifications. What could be the reason?

**✅ A:** `Drift threshold too low`

**Explanation:** If the threshold for drift is set too low, even minor variations can trigger alerts, resulting in frequent notifications.

### Question 21
**Q:** You want to ensure reproducibility in model training. Which of the following should be versioned?

**✅ A:** `Datasets, environments, models`

**Explanation:** Reproducibility in ML workflows depends on consistent versions of data, code environments, and trained models.

### Question 22
**Q:** You're debugging your model’s prediction issues. You want to understand why the model gave a certain output. What do you use?

**✅ A:** `SHAP values`

**Explanation:** SHAP values help explain the contribution of each feature to a particular prediction — ideal for debugging and explainability.

### Question 23
**Q:** You want to determine the minimal changes required to flip a prediction result. Which Responsible AI tool do you use?

**✅ A:** `Counterfactual analysis`

**Explanation:** Counterfactuals show how tweaking certain input features would alter the model's output.

### Question 24
**Q:** You want to monitor model predictions post-deployment. What component can track prediction inputs over time?

**✅ A:** `Dataset Monitor`

**Explanation:** Azure ML’s Dataset Monitor helps track and analyze incoming data for drift and usage patterns.

### Question 25
**Q:** You're using Azure ML and want to view all drift detection runs. Where should you go?

**✅ A:** `Dataset Monitor tab in Azure ML Studio`

**Explanation:** Drift metrics and run history are displayed under the Dataset Monitor section of Azure ML Studio.
