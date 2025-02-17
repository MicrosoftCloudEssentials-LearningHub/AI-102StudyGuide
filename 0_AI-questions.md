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
