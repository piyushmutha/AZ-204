# AZ-204
Quick reference to AZ-204 certification


### [Create serverless applications](https://docs.microsoft.com/en-us/learn/paths/create-serverless-applications/)

1. [Choose the best Azure service to automate your business processes](https://docs.microsoft.com/en-us/learn/modules/choose-azure-service-to-integrate-and-automate-business-processes/)
    
    Business processes modeled in software are often called **workflows**. Azure includes four different technologies that you can use to build and implement workflows that integrate multiple systems
    * Logic Apps
    * Microsoft Power Automate
    * WebJobs
    * Azure Functions
    
    These four technologies have the following similarities
    * Accept Inputs
    * Run Actions
    * Include Condition
    * Produce Output
    * Triggered on a schedule or other external events
    
    **Design-First Approach**<br/>
    It includes user interface in which you can design the workflow and includes the following technologies:
    * **Logic Apps**<br/>
        A service that you can use to automate, orchestrate and integrate disparate components of a distributed application. You can use Logic Apps Designer to define the workflow. Alternatively, you may prefer to code the workflow in JSON notations using the code-view.</br>
        A connector is a Logic Apps component that provides an interface to an external service. Logic Apps provides hundreds of pre-built connectors that you can use to create your apps. If you have an unusual or unique system that you want to call from a Logic Apps, you can create your own connector if your system exposes a REST API.
        
    * **Microsoft Power Automate**<br/>
        A service that you can use to create workflows even when you have no IT Pro experience. You can create workflows that integrate and orchestrate many different components by using the web or mobile app.</br>
        Under the hood, Microsoft Power Automate is built on Logic Apps. This fact means that Power Automate supports the same range of connectors and actions. You can also use custom connectors in Microsoft Power Automate.
    
    **Design-First technologies compared**
    |               | Microsoft Power Automate | Logic Apps |
    | ------------- | ------------------------ | ---------- |
    | Intended users  | Office workers and business analysts | Developers and IT pros |
    | Intended scenarios  | GUI only. Browser and mobile app | Browser and Visual Studio designer. Code editing is possible |
    | Application Lifecycle Management | Power Automate includes testing and production environments | Logic Apps source code can be included in Azure DevOps and source code management systems |
    
    **Code-First Approach**<br/>
    When you need more control over the performance of your workflow or need to write custom code as part of your business process, the following technologies would help:
    * **WebJobs and the WebJobs SDK**<br/>
        WebJobs are a part of the Azure App Service that you can use to run a program or script automatically. The two kinds are:
        * Continous</b>
        * Triggered</b>
        
        You can create a Webjob by using Shell Scripts (Windows, Powershell, Bash) or by writing a program in PHP, Python, Node.js, or Java. You can also program a WebJob by using the .NET Framework or the .NET Core Framework and a .NET language such as C# or VB.NET.<br/>
        Along with C# .NET you can use the WebJobs SDK which includes a range of classes, such as JobHostConfiguration and HostBuilder, which reduce the amount of code required to interact with the Azure App Service.</b>
        
    * **Azure Functions**</b>
        An Azure Function is a simple way for you to run small pieces of code in the cloud, without having to worry about the infrastructure required to host that code. You can write the Function in C#, Java, JavaScript, PowerShell, Python, or any of the languages that are listed in the [Supported languages in Azure Functions article](https://docs.microsoft.com/azure/azure-functions/supported-languages). In addition, with the consumption plan option, you only pay for the time when the code runs. Azure automatically scales your function in response to the demand from users.<br/>
        
        Following is the list of function triggers:
        * HTTPTrigger
        * TimerTrigger
        * BlobTrigger
        * CosmosDBTrigger
        
        Azure Functions can integrate with many different services both within Azure and from third parties. These services can trigger your function, or send data input to your function, or receive data output from your function.
        
    **Code-First technologies compared**
    
    In most cases, the simple administration and more flexible coding model provided by Azure Functions may lead you to choose them in preference to WebJobs. However, you may choose WebJobs for the following reasons:
    * You want the code to be a part of an existing App Service application and to be managed as part of that application, for example in the same Azure DevOps environment.
    * You need close control over the object that listens for events that trigger the code. This object in question is the JobHost class, and you have more flexibility to modify its behavior in WebJobs.
    <br/>

    |               | Azure WebJobs | Azure Functions |
    | ------------- | ------------- | --------------- |
    | Supported languages | C# if you are using the WebJobs SDK | C#, Java, JavaScript, PowerShell, etc. |
    | Automatic scaling | No | Yes |
    | Development and testing in a browser | No | Yes |
    | Pay-per-use pricing | No | Yes |
    | Integration with Logic Apps | No | Yes |
    | Package managers | NuGet if you are using the WebJobs SDK | Nuget and NPM |
    | Can be part of an App Service application | Yes | No |
    | Provides close control of JobHost | Yes | No |

1. [Create serverless logic with Azure Functions](https://docs.microsoft.com/en-us/learn/modules/create-serverless-logic-with-azure-functions/)

1. [Execute an Azure Function with triggers](https://docs.microsoft.com/en-us/learn/modules/execute-azure-function-with-triggers/)

1. [Chain Azure Functions together using input and output bindings](https://docs.microsoft.com/en-us/learn/modules/chain-azure-functions-data-using-bindings/)

1. [Create a long-running serverless workflow with Durable Functions](https://docs.microsoft.com/en-us/learn/modules/create-long-running-serverless-workflow-with-durable-functions/)

1. [Develop, test, and publish Azure Functions by using Azure Functions Core Tools](https://docs.microsoft.com/en-us/learn/modules/develop-test-deploy-azure-functions-with-core-tools/)

1. [Develop, test, and deploy an Azure Function with Visual Studio](https://docs.microsoft.com/en-us/learn/modules/develop-test-deploy-azure-functions-with-visual-studio/)

1. [Monitor GitHub events by using a webhook with Azure Functions](https://docs.microsoft.com/en-us/learn/modules/monitor-github-events-with-a-function-triggered-by-a-webhook/)

1. [Enable automatic updates in a web application using Azure Functions and SignalR Service](https://docs.microsoft.com/en-us/learn/modules/automatic-update-of-a-webapp-using-azure-functions-and-signalr/)


### [Connect your services together](https://docs.microsoft.com/en-us/learn/paths/connect-your-services-together/)

1. [Choose a messaging model in Azure to loosely connect your services](https://docs.microsoft.com/en-us/learn/modules/choose-a-messaging-model-in-azure-to-connect-your-services/)

1. [Implement message-based communication workflows with Azure Service Bus](https://docs.microsoft.com/en-us/learn/modules/implement-message-workflows-with-service-bus/)

1. [Communicate between applications with Azure Queue storage](https://docs.microsoft.com/en-us/learn/modules/communicate-between-apps-with-azure-queue-storage/)

1. [Enable reliable messaging for Big Data applications using Azure Event Hubs](https://docs.microsoft.com/en-us/learn/modules/enable-reliable-messaging-for-big-data-apps-using-event-hubs/)


### [Work with relational data in Azure](https://docs.microsoft.com/en-us/learn/paths/work-with-relational-data-in-azure/)

1. [Provision an Azure SQL database to store application data](https://docs.microsoft.com/en-us/learn/modules/provision-azure-sql-db/)

1. [Create an Azure Database for PostgreSQL server](https://docs.microsoft.com/en-us/learn/modules/create-azure-db-for-postgresql-server/)

1. [Scale multiple Azure SQL Databases with SQL elastic pools](https://docs.microsoft.com/en-us/learn/modules/scale-sql-databases-elastic-pools/)

1. [Secure your Azure SQL Database](https://docs.microsoft.com/en-us/learn/modules/secure-your-azure-sql-database/)

1. [Develop and configure an ASP.NET application that queries an Azure SQL database](https://docs.microsoft.com/en-us/learn/modules/develop-app-that-queries-azure-sql/)


### [Store data in Azure](https://docs.microsoft.com/en-us/learn/paths/store-data-in-azure/)

1. [Choose a data storage approach in Azure](https://docs.microsoft.com/en-us/learn/modules/choose-storage-approach-in-azure/)

1. [Create an Azure Storage account](https://docs.microsoft.com/en-us/learn/modules/create-azure-storage-account/)

1. [Connect an app to Azure Storage](https://docs.microsoft.com/en-us/learn/modules/connect-an-app-to-azure-storage/)

1. [Secure your Azure Storage account](https://docs.microsoft.com/en-us/learn/modules/secure-azure-storage-account/)

1. [Store application data with Azure Blob storage](https://docs.microsoft.com/en-us/learn/modules/store-app-data-with-azure-blob-storage/)


### [Deploy a website with Azure virtual machines](https://docs.microsoft.com/en-us/learn/paths/deploy-a-website-with-azure-virtual-machines/)

1. [Introduction to Azure virtual machines](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-virtual-machines/)

1. [Create a Linux virtual machine in Azure](https://docs.microsoft.com/en-us/learn/modules/create-linux-virtual-machine-in-azure/)

1. [Create a Windows virtual machine in Azure](https://docs.microsoft.com/en-us/learn/modules/create-windows-virtual-machine-in-azure/)

1. [Build and run a web application with the MEAN stack on an Azure Linux virtual machine](https://docs.microsoft.com/en-us/learn/modules/build-a-web-app-with-mean-on-a-linux-vm/)


### [Manage resources in Azure](https://docs.microsoft.com/en-us/learn/paths/manage-resources-in-azure/)

1. [Align requirements with cloud types and service models in Azure](https://docs.microsoft.com/en-us/learn/modules/align-requirements-in-azure/)

1. [Control Azure services with the CLI](https://docs.microsoft.com/en-us/learn/modules/control-azure-services-with-cli/)

1. [Automate Azure tasks using scripts with PowerShell](https://docs.microsoft.com/en-us/learn/modules/automate-azure-tasks-with-powershell/)

1. [Predict costs and optimize spending for Azure](https://docs.microsoft.com/en-us/learn/modules/predict-costs-and-optimize-spending/)

1. [Control and organize Azure resources with Azure Resource Manager](https://docs.microsoft.com/en-us/learn/modules/control-and-organize-with-azure-resource-manager/)

1. [Move Azure resources to another resource group](https://docs.microsoft.com/en-us/learn/modules/move-azure-resources-another-resource-group/)


### [Deploy a website to Azure with Azure App Service](https://docs.microsoft.com/en-us/learn/paths/deploy-a-website-with-azure-app-service/)

1. [Prepare your development environment for Azure development](https://docs.microsoft.com/en-us/learn/modules/prepare-your-dev-environment-for-azure-development/)

1. [Host a web application with Azure App service](https://docs.microsoft.com/en-us/learn/modules/host-a-web-app-with-azure-app-service/)

1. [Publish a web app to Azure with Visual Studio](https://docs.microsoft.com/en-us/learn/modules/publish-azure-web-app-with-visual-studio/)

1. [Stage a web app deployment for testing and rollback by using App Service deployment slots](https://docs.microsoft.com/en-us/learn/modules/stage-deploy-app-service-deployment-slots/)

1. [Scale an App Service web app to efficiently meet demand with App Service scale up and scale out](https://docs.microsoft.com/en-us/learn/modules/app-service-scale-up-scale-out/)

1. [Deploy and run a containerized web app with Azure App Service](https://docs.microsoft.com/en-us/learn/modules/deploy-run-container-app-service/)


### [Extract knowledge and insights from your data with Azure Databricks](https://docs.microsoft.com/en-us/learn/paths/data-science/)

1. [Introduction to Azure Databricks](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-databricks/)

1. [Read and write data by using Azure Databricks](https://docs.microsoft.com/en-us/learn/modules/read-and-write-data-using-azure-databricks/)

1. [Perform exploratory data analysis with Azure Databricks](https://docs.microsoft.com/en-us/learn/modules/perform-exploratory-data-analysis-with-azure-databricks/)

1. [Train, evaluate, and select machine-learning models with Azure Databricks](https://docs.microsoft.com/en-us/learn/modules/perform-model-training-evaluation-and-selection-with-azure-databricks/)

1. [Deep learning with Azure Databricks](https://docs.microsoft.com/en-us/learn/modules/deep-learning-in-azure-databricks/)

1. [Perform text analytics with Azure Databricks](https://docs.microsoft.com/en-us/learn/modules/perform-text-analytics-with-azure-databricks/)


### [Secure your cloud data](https://docs.microsoft.com/en-us/learn/paths/secure-your-cloud-data/)

1. [Security, responsibility, and trust in Azure](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/)

1. [Top 5 security items to consider before pushing to production](https://docs.microsoft.com/en-us/learn/modules/top-5-security-items-to-consider/)

1. [Configure security policies to manage data](https://docs.microsoft.com/en-us/learn/modules/configure-security-policies-to-manage-data/)

1. [Secure your Azure Storage account](https://docs.microsoft.com/en-us/learn/modules/secure-azure-storage-account/)

1. [Configure and manage secrets in Azure Key Vault](https://docs.microsoft.com/en-us/learn/modules/configure-and-manage-azure-key-vault/)

1. [Secure your Azure resources with role-based access control (RBAC)](https://docs.microsoft.com/en-us/learn/modules/secure-azure-resources-with-rbac/)

1. [Secure your Azure SQL Database](https://docs.microsoft.com/en-us/learn/modules/secure-your-azure-sql-database/)
