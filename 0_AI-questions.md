# Planning and Managing Azure AI Solutions: Sample Questions and Answers 

Costa Rica

[![GitHub](https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff)](https://github.com/)
[brown9804](https://github.com/brown9804)

Last updated: 2025-01-16

----------

> [!NOTE]
> The questions and answers provided in this study guide are for practice purposes only and are not official practice questions.
> They are intended to help you prepare for the [AI-102 Microsoft certification exam](https://learn.microsoft.com/en-us/credentials/certifications/azure-ai-engineer/?practice-assessment-type=certification).
> For additional preparation materials and the most up-to-date information, please refer to the [official Microsoft documentation](https://learn.microsoft.com/en-us/credentials/certifications/azure-ai-engineer/?practice-assessment-type=certification#certification-prepare-for-the-exam).

> - Plan and manage an Azure AI solution <br/>
> - Implement content moderation solutions <br/>
> - Implement knowledge mining and document intelligence solutions

<details>
<summary><b>List of References </b> (Click to expand)</summary>

- [Microsoft Certified: Azure AI Engineer Associate](https://learn.microsoft.com/en-us/credentials/certifications/azure-ai-fundamentals/) - Overview of the AI-102 certification, including skills measured and exam details.
- [Study Guide for Exam AI-102: Designing and Implementing an Azure AI Solution](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/ai-900) - Detailed study guide with topics covered in the exam and links to additional resources.
- [Course AI-102T00-A: Designing and Implementing an Azure AI Solution](https://learn.microsoft.com/en-us/training/courses/ai-900t00) - Training course that covers designing and implementing AI solutions using Azure AI services.

</details>

<details>
<summary><b>List of questions/answers </b> (Click to expand)</summary>

</details>

## Q: Deploying Anomaly Detector API Containers

> You plan to use containerized versions of the Anomaly Detector API on cloud devices for testing and in on-premises datacenters. You need to ensure that containerized deployments meet the following requirements:
> - Prevent billing and API information from being stored in the command-line histories of the devices that run the container. <br/>
> - Control access to the container images by using Azure role-based access control (Azure RBAC). <br/>
> Which four actions should you perform in sequence? To answer, move the appropriate actions from the list of actions to the answer area and arrange them in the correct order.

**Actions:**

- [X] Create a custom Dockerfile. 1️⃣ `This is correct because creating a custom Dockerfile is the first step in defining the container environment.`
- [X] Pull the Anomaly Detector container image. 2️⃣ `This is correct because pulling the Anomaly Detector container image is necessary to get the base image for your custom Dockerfile.`
- [X] Build the image. 3️⃣ `This is correct because building the image compiles the Dockerfile and creates the container image.`
- [X] Push the image to an Azure container registry. 4️⃣ `This is correct because pushing the image to an Azure container registry allows you to control access using Azure RBAC.`
- [ ] Distribute a docker run script. ❌ `This is incorrect because distributing a docker run script is not necessary for controlling access or preventing billing and API information from being stored in command-line histories.`
- [ ] Push the image to Docker Hub. ❌ `This is incorrect because pushing the image to Docker Hub does not meet the requirement of controlling access using Azure RBAC.`

## Q: Ensuring Transparency and Privacy in a Sales System

> You are developing a new sales system that will process video and text from a public-facing website. You plan to monitor the sales system to ensure that it provides transparent and secure results. Which two responsible AI principles provide guidance to meet the monitoring requirements? Each correct answer presents part of the solution.

**Options:**

- [X] transparency ✅: `This is correct because transparency ensures that AI systems are understandable and explainable, which is crucial for monitoring and providing transparent results.`
- [ ] fairness ❌: `This is incorrect because fairness focuses on providing unbiased outcomes, not directly on transparency and security.`
- [ ] inclusiveness ❌: `This is incorrect because inclusiveness focuses on ensuring diverse perspectives in AI development, not directly on transparency and security.`
- [ ] reliability and safety ❌: `This is incorrect because reliability and safety focus on ensuring consistent performance and preventing harm, not directly on transparency and security.` 
- [X] privacy and security ✅: `This is correct because privacy and security focus on protecting user data, which is essential for ensuring secure results.`

## Q: Automating Invoice Processing

> Your company receives numerous invoices in English and wants to automate the process of extracting key information such as invoice number, date, and total amount. The solution should require minimal development effort and be able to handle various invoice formats.
> Which Azure service should you use?

**Options:**
- [ ] **A. Custom Vision** ❌: `This is incorrect because Custom Vision is used for image classification and object detection, not for extracting text from documents.`
- [X] **B. Form Recognizer** ✅: `This is correct because Form Recognizer is designed to extract key information from documents, such as invoices, with minimal development effort.`
- [ ] **C Computer Vision** ❌: `This is incorrect because Computer Vision is used for analyzing images and extracting text, but it is not specialized for extracting structured information from documents like invoices.`
- [ ] **D. Personalizer** ❌: `This is incorrect because Personalizer is used for creating personalized user experiences, not for extracting information from documents.`

## Q: Deploying a Language Understanding Application to a Container

> You plan to use a Language Understanding application named `app19467` that is deployed to a container `container27362`. The application was developed using a Language Understanding authoring resource named `lu17392n`. The application has the following versions:

| Version | Trained Date | Published Date |
|---------|--------------|----------------|
| V1.3    | None   | None |
| V1.2    | 2020-10-01   | None           |
| V1.1    | 2020-09-10   | 2020-09-15     |

> You need to create a container that uses the latest deployed version of `app19467`. What steps should you take to achieve this? Pick the actions in the correct sequence.

**Actions:**

- [ ] **Run a container that has version set as an environment variable.** ❌ `This action is not necessary for deploying the model.`
- [ ] **Export the model by using the Export as JSON option.** ❌ `This option is not suitable for container deployment.`
- [ ] **Select v1.2 of `app1`.** ❌ `This version has not been published yet.`
- [X] **Run a container and mount the model file.** ✅ `This action deploys the model to the container using the exported file.`
- [X] **Select v1.1 of `app1`.** ✅ `Given that v1.2 is not an option, v1.1 is the latest published version.`
- [X] **Export the model by using the Export for containers (GZIP) option.** ✅ `This prepares the model for deployment in a container.`

Answer:

| **Action** | **Explanation**                                                                                   |
|------------|---------------------------------------------------------------------------------------------------|
| `Select v1.1 of app1` | This is correct because v1.1 is the latest published version of the application.        |
| `Export the model by using the Export for containers (GZIP) option` | This prepares the model for deployment in a container. |
| `Run a container and mount the model file` | This deploys the model to the container using the exported file. |

<div align="center">
  <h3 style="color: #4CAF50;">Total Visitors</h3>
  <img src="https://profile-counter.glitch.me/brown9804/count.svg" alt="Visitor Count" style="border: 2px solid #4CAF50; border-radius: 5px; padding: 5px;"/>
</div>
