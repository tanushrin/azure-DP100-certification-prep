# Module1 Training and Experimentation

**Q: What must you define in AutoMLConfig?**  
A: task, label_column_name, primary_metric, compute_target

**Q: How do you retrieve the best model after AutoML run?**  
A: run.get_output()

**Q: What is ScriptRunConfig used for?**  
A: Wraps script, compute target, and environment for training

**Q: How do you submit a training job in Azure ML?**  
A: experiment.submit(ScriptRunConfig)

**Q: What does the Run object track?**  
A: Metrics, logs, outputs, artifacts

**Q: What is PythonScriptStep used for?**  
A: Run Python scripts in Azure ML pipelines

**Q: What is DataPath or OutputFileDatasetConfig used for?**  
A: Send data between pipeline steps

**Q: How do you execute a pipeline?**  
A: Wrap steps in Pipeline and submit with Experiment.submit()

**Q: How do you deploy a model in SDK?**  
A: Use InferenceConfig + DeploymentConfig with Model.deploy()

**Q: What types of compute targets can be used?**  
A: Compute Instance, Compute Cluster, ACI, AKS

