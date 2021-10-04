# DSGo Readme
## Employee Attrition Lab

This lab is built for use as a workshop at the Data Science Go (DSGo) conference in October 2021. It uses Oracle Cloud Infrastructure (OCI) Data Science to create a model to predict employee attrition. The workshop guides the user through developing a machine learning model and performing all the steps to deploy the model into production. The user creates a machine learning model then creates a model artifact and stores it in the Model Catalog. Using the console, the model is deployed and then called as a REST API endpoint to perform inference operations on the model.

### Prerequisites
  - None

This workshop is designed for users that will register for a new OCI trial account with free cloud credits.  The workshop provides instructions to sign up for a free trial account and then configure the tenancy for Data Science. The remainder of the workshop guides the user through the activities to build, train, and deploy a machine learning model.

**DSGo participants need to sign-up for their OCI account with the same email that was used to register for the conference.** By doing so, DSGo participants receive additional free cloud credits and do not have to provide payment verification.

Other users of this workshop may sign-up for a standard OCI trial account that provides free cloud credits but requires payment method verification as an identity check. (The user is not charged during the free trial and the user has the option to continue with free tier services or explicitly convert to a paid account at the end of the trial. Note that OCI Data Science is not included in the OCI free tier.)

If you choose to use an existing OCI trial account, your 30-day trial must still be active and you must have credits remaining on your account to cover the services used in this workshop. (Your trial status is displayed in the OCI console.)

You may of course also use a paid OCI account and your account will be charged for the services used during this workshop.

### Instructions
  - TODO

    Open a Data Science Notebook session (i.e. JupyterLab).
    Open a file terminal by clicking on File -> New -> Terminal.
    In the terminal run the following commands:
        odsc conda install -s mlcpuv1 to install the General Machine Learning for CPUs conda.
        mkdir /home/datascience/dataflow
        conda activate /home/datascience/conda/mlcpuv1 to activate the conda.
        pip install oci to install the OCI Python SDK.
    Copy the employee-attrition.ipynb into the notebook session.
    Open the notebook.
    Change the notebook kernel to Python [conda env:mlcpuv1].
    Read the notebook and execute each cell.

Note: Before you execute the "Invoke the Model HTTP Endpoint" section, ensure you have the right endpoint URI. You can obtain this information by going to the Data Science service in the console. Select the compartment where the model deployment is contained. Then select the appropriate Project. Under the Resources section select Model Deployments. You can copy the model deployment URI from the model deployment you created.
