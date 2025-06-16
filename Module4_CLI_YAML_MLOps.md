# Module4 CLI YAML MLOps

**Q: How to submit a job in CLI v2?**  
A: az ml job create --file job.yml

**Q: How to deploy a model in CLI v2?**  
A: az ml endpoint create --file endpoint.yml

**Q: Which YAML keys are required?**  
A: compute, command, environment, code

**Q: What must be versioned for CI/CD?**  
A: models, datasets, environments

**Q: How do you define compute in YAML?**  
A: compute: azureml:my-cluster

**Q: What command retrieves run logs?**  
A: az ml job show --name <job-name>

**Q: How do you register a model?**  
A: az ml model create --name <model-name> --path outputs/

