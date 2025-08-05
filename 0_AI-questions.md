# Planning and Managing Azure AI Solutions: Sample Questions and Answers 

Costa Rica

[![GitHub](https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff)](https://github.com/)
[brown9804](https://github.com/brown9804)

Last updated: 2025-08-05

----------

> [!NOTE]
> The questions and answers provided in this study guide are for practice purposes only and are not official practice questions.
> They are intended to help you prepare for the [AI-102 Microsoft certification exam](https://learn.microsoft.com/en-us/credentials/certifications/azure-ai-engineer/?practice-assessment-type=certification).
> For additional preparation materials and the most up-to-date information, please refer to the [official Microsoft documentation](https://learn.microsoft.com/en-us/credentials/certifications/azure-ai-engineer/?practice-assessment-type=certification#certification-prepare-for-the-exam).

> - Plan and manage an Azure AI solution <br/>
> - Implement content moderation solutions <br/>
> - Implement knowledge mining and document intelligence solutions <br/>
> - Implement generative AI solutions

<details>
<summary><b>List of References </b> (Click to expand)</summary>

- [Microsoft Certified: Azure AI Engineer Associate](https://learn.microsoft.com/en-us/credentials/certifications/azure-ai-fundamentals/) - Overview of the AI-102 certification, including skills measured and exam details.
- [Study Guide for Exam AI-102: Designing and Implementing an Azure AI Solution](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/ai-900) - Detailed study guide with topics covered in the exam and links to additional resources.
- [Course AI-102T00-A: Designing and Implementing an Azure AI Solution](https://learn.microsoft.com/en-us/training/courses/ai-900t00) - Training course that covers designing and implementing AI solutions using Azure AI services.

</details>

<details>
<summary><b>List of questions/answers </b> (Click to expand)</summary>

- [Q1: Configuring Index Attributes for Azure AI Search](#q1-configuring-index-attributes-for-azure-ai-search)
- [Q2: Configuring Azure AI Services for Text Translation](#q2-configuring-azure-ai-services-for-text-translation)
- [Q3: Configuring an Enrichment Pipeline for OCR and Text Analytics](#q3-configuring-an-enrichment-pipeline-for-ocr-and-text-analytics)
- [Q4: Managing Query Throttling in Azure AI Search](#q4-managing-query-throttling-in-azure-ai-search)
- [Q5: Choosing the Right Azure Service for Predictive Maintenance](#q5-choosing-the-right-azure-service-for-predictive-maintenance)
- [Q6: Configuring Private Endpoint for Azure AI Search](#q6-configuring-private-endpoint-for-azure-ai-search)
- [Q7: Ensuring Fairness in a Sales System](#q7-ensuring-fairness-in-a-sales-system)
- [Q8: Deploying Anomaly Detector API Containers](#q8-deploying-anomaly-detector-api-containers)
- [Q9: Ensuring Direct Connectivity for Azure AI Search](#q9-ensuring-direct-connectivity-for-azure-ai-search)
- [Q10: Ensuring Inclusiveness in an Azure Bot](#q10-ensuring-inclusiveness-in-an-azure-bot)
- [Q11: Ensuring Transparency and Privacy in a Sales System](#q11-ensuring-transparency-and-privacy-in-a-sales-system)
- [Q12: Automating Invoice Processing](#q12-automating-invoice-processing)
- [Q13: Reducing Throttling in Azure AI Search](#q13-reducing-throttling-in-azure-ai-search)
- [Q14: Ensuring Direct Connectivity for Azure AI Search](#q14-ensuring-direct-connectivity-for-azure-ai-search)
- [Q15: Deploying a Language Understanding Application to a Container](#q15-deploying-a-language-understanding-application-to-a-container)
- [Q16: Enabling Server-Side Encryption with Customer-Managed Keys in Azure AI Search](#q16-enabling-server-side-encryption-with-customer-managed-keys-in-azure-ai-search)
- [Q17: Ensuring Responsible AI Principles in Sentiment Analysis for Bonuses](#q17-ensuring-responsible-ai-principles-in-sentiment-analysis-for-bonuses)
- [Q18: Directing Messages to Language Support Teams](#q18-directing-messages-to-language-support-teams)
- [Q19: Configuring IP Firewall Rules for Azure AI Search](#q19-configuring-ip-firewall-rules-for-azure-ai-search)
- [Q20: Converting Speech to Text for Streaming MP3 Data](#q20-converting-speech-to-text-for-streaming-mp3-data)
- [Q21: Developing an Automated Call Handling System](#q21-developing-an-automated-call-handling-system)
- [Q22: Extracting Data from Receipts Using Form Recognizer](#q22-extracting-data-from-receipts-using-form-recognizer)
    - [Tip Reference](#tip-reference)
- [Q23: Reducing Throttling in Azure AI Search](#q23-reducing-throttling-in-azure-ai-search)
- [Q24: Analyzing Extracted Information from Purchase Orders Using Power BI](#q24-analyzing-extracted-information-from-purchase-orders-using-power-bi)
- [Q25: Securing an Azure AI Search Resource](#q25-securing-an-azure-ai-search-resource)
- [Q26: Building a Monitoring Solution for PPE Compliance](#q26-building-a-monitoring-solution-for-ppe-compliance)
- [Q27: Building an App for Anomaly Detection and Incident Alerts](#q27-building-an-app-for-anomaly-detection-and-incident-alerts)
- [Q28: Hosting an Azure AI Services Model with Limited Connectivity](#q28-hosting-an-azure-ai-services-model-with-limited-connectivity)
- [Q29: Detecting Anomalies in Real-Time Sensor Data](#q29-detecting-anomalies-in-real-time-sensor-data)
- [Q30: Ensuring Confidential Documents Remain On-Premises with Azure AI Services](#q30-ensuring-confidential-documents-remain-on-premises-with-azure-ai-services)
- [Q31: Authenticating to the Speech Service Using Azure AD](#q31-authenticating-to-the-speech-service-using-azure-ad)
- [Q32: Implementing Real-Time Translation in a Multilingual Chat Application](#q32-implementing-real-time-translation-in-a-multilingual-chat-application)
- [Q33: Hosting an Anomaly Detector Instance on a Docker Host](#q33-hosting-an-anomaly-detector-instance-on-a-docker-host)
- [Q34: Configuring Capacity for an Azure OpenAI Resource](#q34-configuring-capacity-for-an-azure-openai-resource)
- [Q35: Detecting Negative Comments Using Sentiment Analysis API](#q35-detecting-negative-comments-using-sentiment-analysis-api)
- [Q36: Providing Access to Azure OpenAI Resource and Connecting to Deployments](#q36-providing-access-to-azure-openai-resource-and-connecting-to-deployments)
- [Q37: Configuring App1 to Connect to Azure OpenAI Model AI1](#q37-configuring-app1-to-connect-to-azure-openai-model-ai1)
- [Q38: Monitoring Temperature Data and Generating Alerts](#q38-monitoring-temperature-data-and-generating-alerts)
- [Q39: Implementing Predictive Maintenance with Azure Services](#q39-implementing-predictive-maintenance-with-azure-services)
- [Q40: Indexing a Large Video File Using Azure Video Indexer](#q40-indexing-a-large-video-file-using-azure-video-indexer)
- [Q41: Securing Access to Azure AI Service Resource](#q41-securing-access-to-azure-ai-service-resource)
- [Q42: Monitoring a Video Stream and Detecting Questions](#q42-monitoring-a-video-stream-and-detecting-questions)
- [Q43: Identifying the Created Azure AI Services Account in Azure DevOps Pipeline](#q43-identifying-the-created-azure-ai-services-account-in-azure-devops-pipeline)
- [Q44: Extracting Data from Hand-Written Survey Responses Using Azure AI Document Intelligence](#q44-extracting-data-from-hand-written-survey-responses-using-azure-ai-document-intelligence)

</details>

> [!TIP]
> **Azure AI Service Deployment Patterns:**

| Pattern | Use Case | Benefits |
|---------|----------|----------|
| **Multi-Service Resource** | Multiple AI capabilities needed | Cost-effective, single endpoint management |
| **Single-Service Resource** | Specific service requirements | Granular control, dedicated resources |
| **Containerized Deployment** | On-premises or edge scenarios | Data sovereignty, reduced latency |
| **Hybrid Deployment** | Mixed cloud/on-premises needs | Flexibility, compliance requirements |

> [!TIP]
> **Azure OpenAI Resource Planning:**

| Consideration | Standard Tier | Provisioned Tier |
|---------------|---------------|------------------|
| **Capacity Units** | Pay-per-use | Reserved capacity |
| **Request Limits** | 60 RPM per unit | Guaranteed throughput |
| **Cost Model** | Variable | Fixed monthly |
| **Use Case** | Development, testing | Production, high-volume |

> [!TIP]
> **Container Deployment Best Practices:**

| Requirement | Solution | Configuration |
|-------------|----------|---------------|
| **Billing Parameter** | Required for all containers | `Billing={ENDPOINT_URI}` |
| **API Key** | Authentication | `ApiKey={API_KEY}` |
| **EULA Acceptance** | Legal requirement | `Eula=accept` |
| **Resource Limits** | Performance optimization | `--memory 4g --cpus 1` |

> [!TIP]
> **Azure AI Search Index Optimization:**

| Attribute | Purpose | Impact on Performance |
|-----------|---------|---------------------|
| **searchable** | Enable text search | Increases index size |
| **filterable** | Enable filtering | Faster query performance |
| **facetable** | Enable drill-down navigation | Enhanced user experience |
| **retrievable** | Return in results | Required for display |
| **sortable** | Enable sorting | Additional processing overhead |

> [!TIP]
> **Responsible AI Implementation Checklist:**

| Principle | Implementation | Validation Method |
|-----------|----------------|-------------------|
| **Fairness** | Diverse training data, bias testing | Regular model audits |
| **Reliability** | Error handling, fallback mechanisms | Comprehensive testing |
| **Safety** | Content filtering, output validation | Continuous monitoring |
| **Privacy** | Data encryption, access controls | Security assessments |
| **Inclusiveness** | Multi-modal interfaces, accessibility | User feedback analysis |
| **Transparency** | Model explainability, documentation | Clear communication |
| **Accountability** | Human oversight, audit trails | Review processes |

> [!TIP]
> **Azure AI Services Throttling Management:**

| Service Tier | Requests/Second | Mitigation Strategy |
|--------------|----------------|-------------------|
| **Free (F0)** | Limited | Use for development only |
| **Standard (S0)** | Higher limits | Scale up for production |
| **Premium** | Highest limits | Add replicas, optimize queries |
| **Custom** | Negotiated | Enterprise agreements |

> [!TIP]
> **Network Security Configuration:**

| Security Level | Configuration | Use Case |
|----------------|---------------|----------|
| **Public Access** | Default endpoints | Development, testing |
| **IP Restrictions** | Firewall rules | Basic access control |
| **Service Endpoints** | VNet integration | Azure-to-Azure communication |
| **Private Endpoints** | Private connectivity | Maximum security |

> [!TIP]
> **Authentication Methods Comparison:**

| Method | Security Level | Implementation Complexity | Cost |
|--------|----------------|--------------------------|------|
| **API Keys** | Basic | Low | None |
| **Azure AD** | High | Medium | None |
| **Managed Identity** | Highest | Low (for Azure resources) | None |
| **Service Principal** | High | High | None |

> [!TIP]
> **Cost Optimization Strategies:**

| Strategy | Implementation | Savings Potential |
|----------|----------------|-------------------|
| **Right-sizing** | Match tier to workload | 20-40% |
| **Reserved Instances** | Long-term commitments | 20-50% |
| **Auto-scaling** | Dynamic resource allocation | 15-30% |
| **Container Deployment** | On-premises hosting | Variable |
| **Multi-service Resources** | Consolidated billing | 10-20% |

> [!TIP]
> **Monitoring and Diagnostics Setup:**

| Monitoring Type | Tool | Key Metrics |
|----------------|------|-------------|
| **Performance** | Azure Monitor | Response time, throughput |
| **Availability** | Application Insights | Uptime, error rates |
| **Usage** | Cost Management | Request volume, costs |
| **Security** | Azure Security Center | Access patterns, threats |

> [!TIP]
> **Development Environment Setup:**

| Environment | Configuration | Purpose |
|-------------|---------------|---------|
| **Development** | Free/Basic tier, public access | Initial development |
| **Testing** | Standard tier, limited access | Integration testing |
| **Staging** | Production-like, private access | Pre-production validation |
| **Production** | High-tier, secured access | Live workloads |

> [!TIP]
> **Data Residency and Compliance:**

| Requirement | Implementation | Services Affected |
|-------------|----------------|-------------------|
| **GDPR** | EU data centers, encryption | All AI services |
| **HIPAA** | BAA agreements, secure transmission | Text Analytics, Speech |
| **SOC 2** | Audit compliance, access controls | All AI services |
| **FedRAMP** | Government cloud deployment | Limited services |

> [!TIP]
> **Service Integration Patterns:**

| Pattern | Use Case | Implementation |
|---------|----------|----------------|
| **Pipeline Integration** | Sequential processing | AI Search + Form Recognizer |
| **Event-Driven** | Real-time processing | Event Grid + Functions |
| **Batch Processing** | Large-scale analysis | Logic Apps + AI Services |
| **API Gateway** | Centralized access | API Management + AI Services |

> [!TIP]
> **Performance Optimization:**

| Optimization | Technique | Benefit |
|--------------|-----------|---------|
| **Caching** | Redis Cache for results | Reduced API calls |
| **Batching** | Multiple requests together | Improved throughput |
| **Async Processing** | Non-blocking operations | Better scalability |
| **Load Balancing** | Distribute requests | Higher availability |

> [!TIP]
> **Disaster Recovery Planning:**

| Component | Strategy | Recovery Time |
|-----------|----------|---------------|
| **AI Models** | Cross-region deployment | < 5 minutes |
| **Training Data** | Geo-redundant storage | < 30 minutes |
| **Configuration** | ARM templates | < 15 minutes |
| **Custom Code** | CI/CD pipelines | < 10 minutes |

> [!TIP]
> **Capacity Planning Guidelines:**

| Service | Metric | Planning Factor |
|---------|--------|----------------|
| **Computer Vision** | Images/hour | Peak usage × 1.5 |
| **Text Analytics** | Documents/minute | Average × burst factor |
| **Speech Services** | Concurrent connections | Expected users × 0.3 |
| **Custom Vision** | Predictions/second | Historical data + growth |

> [!TIP]
> **Security Best Practices:**

| Security Layer | Implementation | Tools |
|----------------|----------------|-------|
| **Network** | Private endpoints, NSGs | Azure Firewall |
| **Identity** | Azure AD, RBAC | Conditional Access |
| **Data** | Encryption at rest/transit | Key Vault |
| **Application** | Input validation, rate limiting | App Gateway |

> [!TIP]
> **Troubleshooting Common Issues:**

| Issue | Symptoms | Resolution |
|-------|----------|------------|
| **Rate Limiting** | 429 errors | Scale tier, add replicas |
| **Authentication** | 401/403 errors | Check keys, permissions |
| **Timeout** | Request timeouts | Optimize queries, increase limits |
| **Quality** | Poor results | Retrain models, validate data |

> [!TIP]
> **Migration Strategies:**

| Migration Type | Approach | Considerations |
|----------------|----------|----------------|
| **Service Upgrade** | Blue-green deployment | Zero downtime |
| **Region Change** | Parallel deployment | Data transfer costs |
| **Tier Change** | In-place upgrade | Brief downtime |
| **Architecture** | Phased migration | Gradual transition |

> [!TIP]
> Planning Phase
1. **Assess Requirements**: Understand performance, security, and compliance needs
2. **Choose Architecture**: Select appropriate deployment patterns
3. **Design for Scale**: Plan for future growth and peak loads
4. **Security First**: Implement defense in depth from the start

> [!TIP]
> Implementation Phase:
1. **Start Small**: Begin with development/test environments
2. **Automate Deployment**: Use Infrastructure as Code (IaC)
3. **Monitor Everything**: Set up comprehensive monitoring
4. **Test Thoroughly**: Validate performance and security

> [!TIP]
> Operations Phase:
1. **Monitor Continuously**: Track performance and costs
2. **Optimize Regularly**: Review and adjust configurations
3. **Plan Capacity**: Anticipate growth and scaling needs
4. **Maintain Security**: Keep up with security updates

> [!TIP]
> Governance:
1. **Document Everything**: Maintain architectural decisions
2. **Establish Policies**: Define usage and security guidelines
3. **Review Regularly**: Conduct periodic architecture reviews
4. **Train Teams**: Ensure knowledge transfer and best practices

## Q1: Configuring Index Attributes for Azure AI Search

> You have an Azure AI Search solution and a collection of blog posts that include a category field. You need to index the posts. The solution must meet the following requirements: <br/>
> - Include the category field in the search results. <br/>
> - Ensure that users can search for words in the category field. <br/>
> - Ensure that users can perform drill down filtering based on category. <br/>
> Which index attributes should you configure for the category field?

- [ ] searchable, sortable, and retrievable ❌: `This is incorrect because while these attributes allow searching and sorting, they do not support drill down filtering.`
- [ ] retrievable, filterable, and sortable ❌: `This is incorrect because while these attributes allow filtering and sorting, they do not support searching for words in the category field.`
- [ ] retrievable, facetable, and key ❌: `This is incorrect because the 'key' attribute is used for unique identifiers, not for enabling search or filtering capabilities.`
- [ ] searchable, facetable, and retrievable ✅: `This is correct because these attributes allow the category field to be included in search results, support searching for words in the category field, and enable drill down filtering based on category.`

## Q2: Configuring Azure AI Services for Text Translation

> You are developing a multilingual application that needs to translate text between multiple languages. You plan to use Azure AI Services to achieve this. Which Azure AI Service should you use for each requirement? 

To translate text from one language to another: ___________________________

- [ ] Translator Text ✅: `This is correct because the Translator Text service is specifically designed for translating text between multiple languages.`
- [ ] Text Analytics ❌: `This is incorrect because Text Analytics is used for analyzing text data, not for translating text.`
- [ ] Speech ❌: `This is incorrect because the Speech service is used for processing and recognizing speech, not for translating text.`

To detect the language of the input text: ___________________________

- [ ] Translator Text ✅: `This is correct because the Translator Text service includes language detection capabilities to identify the language of the input text.`
- [ ] Text Analytics ✅: `This is correct because the Text Analytics service also provides language detection capabilities.`
- [ ] Speech ❌: `This is incorrect because the Speech service is used for processing and recognizing speech, not for detecting the language of text.`

To provide real-time translation of spoken language:___________________________

- [ ] Translator Text ❌: `This is incorrect because Translator Text is used for translating written text, not for real-time spoken language translation.`
- [ ] Speech ✅: `This is correct because the Speech service provides real-time translation of spoken language.`
- [ ] Text Analytics ❌: `This is incorrect because Text Analytics is used for analyzing text data, not for real-time spoken language translation.`


## Q3: Configuring an Enrichment Pipeline for OCR and Text Analytics

> You have a collection of 50,000 scanned documents that contain text. You plan to make the text available through Azure AI Search. You need to configure an enrichment pipeline to perform optical character recognition (OCR) and text analytics. The solution must minimize costs. What should you attach to the skillset?

- [ ] a new Computer Vision resource ❌: `This is incorrect because while the Computer Vision service can perform OCR, it does not provide text analytics capabilities.`
- [ ] a free (limited enrichments) AI Services resource ❌: `This is incorrect because a multiservice account does not support the free tier (F0), and the free tier is not suitable for processing a large volume of documents like 50,000.`
- [ ] an Azure Machine Learning Designer pipeline ❌: `This is incorrect because an Azure Machine Learning Designer pipeline is not required for OCR and text analytics in this scenario.`
- [ ] a new AI Services resource that uses the S0 pricing tier ✅: `This is correct because a multiservice AI Services resource using the S0 pricing tier can provide both OCR and text analytics capabilities, and it is suitable for processing a large volume of documents.`

## Q4: Managing Query Throttling in Azure AI Search

> You have an Azure AI Search service. During the past 12 months, query volume steadily increased. You discover that some search query requests to the AI Search service are being throttled. You need to reduce the likelihood that search query requests are throttled. Which solution should you implement?

- [ ] Configure a AI Search service that uses a higher tier. ✅: `This is correct because using a higher tier provides more resources and can handle a higher query volume, reducing the likelihood of throttling.`
- [ ] Add more replicas to the AI Search service. ✅: `This is correct because adding more replicas can distribute the query load and reduce the likelihood of throttling.`
- [ ] Enable query caching in the AI Search service. ❌: `This is incorrect because query caching is not a feature of Azure AI Search and does not address throttling issues.`
- [ ] Increase the timeout setting for search queries. ❌: `This is incorrect because increasing the timeout setting does not reduce throttling; it only allows queries to run longer before timing out.`

## Q5: Choosing the Right Azure Service for Predictive Maintenance

> You plan to perform predictive maintenance. You collect IoT sensor data from 1000 industrial machines for a year. Each machine has 50 different sensors that generate data at one-minute intervals. In total, you have 50,000 time series datasets. You need to identify unusual values in each time series to help predict machinery failures. Which Azure service should you use?

- [ ] Azure Machine Learning ❌: `This is incorrect because while Azure Machine Learning can be used for predictive maintenance, it requires more setup and customization compared to a specialized service like Anomaly Detector.`
- [ ] Azure Stream Analytics ❌: `This is incorrect because Azure Stream Analytics is designed for real-time data processing and analytics, not specifically for detecting anomalies in time series data.`
- [ ] Azure Time Series Insights ❌: `This is incorrect because Azure Time Series Insights is used for visualizing and exploring time series data, not specifically for detecting anomalies.`
- [ ] Anomaly Detector ✅: `This is correct because Anomaly Detector is specifically designed to identify unusual values in time series data, making it ideal for predictive maintenance.`

## Q6: Configuring Private Endpoint for Azure AI Search

> You create a web app named `app1` that runs on an Azure virtual machine named `vm1`. `vm1` is on an Azure virtual network named `vnet1`. You plan to create a new Azure AI Search service named `service1`. You need to ensure that `app1` can connect directly to `service1` without routing traffic over the public internet. Which solution should you implement?

- [ ] Deploy `service1` with a private endpoint in `vnet1` and configure Azure Private Link. ✅: `This is correct because deploying `service1` with a private endpoint in the same virtual network and configuring Azure Private Link ensures that traffic between `app1` and `service1` does not traverse the public internet.`
- [ ] Deploy `service1` with a public endpoint and configure a VPN connection between `vnet1` and the public endpoint. ❌: `This is incorrect because using a public endpoint and VPN connection does not prevent traffic from traversing the public internet.`
- [ ] Deploy `service1` with a public endpoint and configure a service endpoint in `vnet1`. ❌: `This is incorrect because service endpoints do not provide the same level of security as private endpoints and still allow traffic to traverse the public internet.`
- [ ] Deploy `service1` with a private endpoint in a different virtual network and configure Azure Private Link. ❌: `This is incorrect because deploying `service1` in a different virtual network would require additional configuration and does not ensure direct connectivity without traversing the public internet.`

## Q7: Ensuring Fairness in a Sales System

> You are developing a new sales system that will process video and text from a public-facing website. To ensure fairness, you plan to implement measures that prevent bias in the system's recommendations and decisions. Which two actions should you take to ensure fairness? 

- [ ] Conduct regular bias assessments on the system's algorithms. ✅: `This is correct because conducting regular bias assessments helps identify and mitigate any biases in the system's algorithms, ensuring fair outcomes.`
- [ ] Ensure transparency in how the system makes decisions. ❌: `This is incorrect because while transparency is important, it does not directly address the prevention of bias in recommendations and decisions.`
- [ ] Include diverse data sets during the training phase. ✅: `This is correct because including diverse data sets helps ensure that the system's algorithms are trained on a wide range of scenarios, reducing the risk of bias.`
- [ ] Implement strict data privacy measures. ❌: `This is incorrect because data privacy measures focus on protecting user data, not directly on ensuring fairness in recommendations and decisions.`
- [ ] Use only historical data for training the system. ❌: `This is incorrect because relying solely on historical data can perpetuate existing biases, rather than ensuring fairness.`

## Q8: Deploying Anomaly Detector API Containers

> You plan to use containerized versions of the Anomaly Detector API on cloud devices for testing and in on-premises datacenters. You need to ensure that containerized deployments meet the following requirements:
> - Prevent billing and API information from being stored in the command-line histories of the devices that run the container. <br/>
> - Control access to the container images by using Azure role-based access control (Azure RBAC). <br/>
> Which four actions should you perform in sequence? 

- [ ] Create a custom Dockerfile. 1️⃣ `This is correct because creating a custom Dockerfile is the first step in defining the container environment.`
- [ ] Pull the Anomaly Detector container image. 2️⃣ `This is correct because pulling the Anomaly Detector container image is necessary to get the base image for your custom Dockerfile.`
- [ ] Build the image. 3️⃣ `This is correct because building the image compiles the Dockerfile and creates the container image.`
- [ ] Push the image to an Azure container registry. 4️⃣ `This is correct because pushing the image to an Azure container registry allows you to control access using Azure RBAC.`
- [ ] Distribute a docker run script. ❌ `This is incorrect because distributing a docker run script is not necessary for controlling access or preventing billing and API information from being stored in command-line histories.`
- [ ] Push the image to Docker Hub. ❌ `This is incorrect because pushing the image to Docker Hub does not meet the requirement of controlling access using Azure RBAC.`

## Q9: Ensuring Direct Connectivity for Azure AI Search

> You create a web app named `app1` that runs on an Azure virtual machine named `vm1`. `vm1` is on an Azure virtual network named `vnet1`. You plan to create a new Azure AI Search service named `service1`. You need to ensure that `app1` can connect directly to `service1` without routing traffic over the public internet. <br/>
> **Solution: You deploy `service1` and a private endpoint to `vnet1`.** Does this meet the goal?

- [ ] Yes ✅: `This is correct because deploying `service1` with a private endpoint in `vnet1` ensures that traffic between `app1` and `service1` does not traverse the public internet, providing a secure and direct connection.`
- [ ] No ❌: `This is incorrect because deploying `service1` with a private endpoint in `vnet1` does meet the goal of ensuring direct connectivity without using the public internet.`

## Q10: Ensuring Inclusiveness in an Azure Bot

> You have a Language Understanding resource named `lu1`. You build and deploy an Azure bot named `bot1` that uses `lu1`. You need to ensure that `bot1` adheres to the Microsoft responsible AI principle of inclusiveness. How should you extend `bot1`?

- [ ] Implement authentication for `bot1` ❌: `This is incorrect because implementing authentication does not directly address the principle of inclusiveness.`
- [ ] Enable active learning for `lu1` ❌: `This is incorrect because enabling active learning improves the model's accuracy over time but does not directly address inclusiveness.`
- [ ] Host `lu1` in a container ❌: `This is incorrect because hosting `lu1` in a container does not directly address the principle of inclusiveness.`
- [ ] Add Direct Line Speech to `bot1` ✅: `This is correct because adding Direct Line Speech allows the bot to support speech interactions, making it more accessible and inclusive for users who may have difficulty typing or reading.`

## Q11: Ensuring Transparency and Privacy in a Sales System

> You are developing a new sales system that will process video and text from a public-facing website. You plan to monitor the sales system to ensure that it provides transparent and secure results. Which two responsible AI principles provide guidance to meet the monitoring requirements? 

- [ ] transparency ✅: `This is correct because transparency ensures that AI systems are understandable and explainable, which is crucial for monitoring and providing transparent results.`
- [ ] fairness ❌: `This is incorrect because fairness focuses on providing unbiased outcomes, not directly on transparency and security.`
- [ ] inclusiveness ❌: `This is incorrect because inclusiveness focuses on ensuring diverse perspectives in AI development, not directly on transparency and security.`
- [ ] reliability and safety ❌: `This is incorrect because reliability and safety focus on ensuring consistent performance and preventing harm, not directly on transparency and security.` 
- [ ] privacy and security ✅: `This is correct because privacy and security focus on protecting user data, which is essential for ensuring secure results.`

## Q12: Automating Invoice Processing

> Your company receives numerous invoices in English and wants to automate the process of extracting key information such as invoice number, date, and total amount. The solution should require minimal development effort and be able to handle various invoice formats. Which Azure service should you use?


- [ ] **Custom Vision** ❌: `This is incorrect because Custom Vision is used for image classification and object detection, not for extracting text from documents.`
- [ ] **Form Recognizer** ✅: `This is correct because Form Recognizer is designed to extract key information from documents, such as invoices, with minimal development effort.`
- [ ] **Computer Vision** ❌: `This is incorrect because Computer Vision is used for analyzing images and extracting text, but it is not specialized for extracting structured information from documents like invoices.`
- [ ] **Personalizer** ❌: `This is incorrect because Personalizer is used for creating personalized user experiences, not for extracting information from documents.`

## Q13: Reducing Throttling in Azure AI Search

> You have an Azure AI Search service. During the past 12 months, query volume steadily increased. You discover that some search query requests to the AI Search service are being throttled. You need to reduce the likelihood that search query requests are throttled. **Solution: You enable customer-managed key (CMK) encryption.** Does this meet the goal?

- [ ] Yes ❌: `This is incorrect because enabling customer-managed key (CMK) encryption does not address the issue of throttling caused by high query volume. Throttling is typically related to service capacity, not encryption settings.`
- [ ] No ✅: `This is correct because enabling customer-managed key (CMK) encryption does not reduce throttling. To reduce throttling, you should consider increasing the service tier, adding more replicas, or optimizing query performance.`

## Q14: Ensuring Direct Connectivity for Azure AI Search

> You create a web app named `app1` that runs on an Azure virtual machine named `vm1`. `vm1` is on an Azure virtual network named `vnet1`. You plan to create a new Azure AI Search service named `service1`. You need to ensure that `app1` can connect directly to `service1` without routing traffic over the public internet. <br/>
> Solution: You deploy `service1` with a public endpoint and configure a network security group (NSG) for `vnet1`. Does this meet the goal?

- [ ] Yes ❌
- [ ] No ✅. The correct answer is **No**. Configuring a network security group (NSG) for `vnet1` does not prevent traffic from routing over the public internet. To ensure direct connectivity without using the public internet, you should deploy `service1` with a private endpoint and configure Azure Private Link.

## Q15: Deploying a Language Understanding Application to a Container

> You plan to use a Language Understanding application named `app19467` that is deployed to a container `container27362`. The application was developed using a Language Understanding authoring resource named `lu17392n`. The application has the following versions:

| Version | Trained Date | Published Date |
|---------|--------------|----------------|
| V1.3    | None   | None |
| V1.2    | 2020-10-01   | None           |
| V1.1    | 2020-09-10   | 2020-09-15     |

> You need to create a container that uses the latest deployed version of `app19467`. What steps should you take to achieve this?

- [ ] **Run a container that has version set as an environment variable.** ❌ `This action is not necessary for deploying the model.`
- [ ] **Export the model by using the Export as JSON option.** ❌ `This option is not suitable for container deployment.`
- [ ] **Select v1.2 of `app1`.** ❌ `This version has not been published yet.`
- [ ] **Run a container and mount the model file.** ✅ `This action deploys the model to the container using the exported file.`
- [ ] **Select v1.1 of `app1`.** ✅ `Given that v1.2 is not an option, v1.1 is the latest published version.`
- [ ] **Export the model by using the Export for containers (GZIP) option.** ✅ `This prepares the model for deployment in a container.`

| **Action** | **Explanation**                                                                                   |
|------------|---------------------------------------------------------------------------------------------------|
| `Select v1.1 of app1` | This is correct because v1.1 is the latest published version of the application.        |
| `Export the model by using the Export for containers (GZIP) option` | This prepares the model for deployment in a container. |
| `Run a container and mount the model file` | This deploys the model to the container using the exported file. |

## Q16: Enabling Server-Side Encryption with Customer-Managed Keys in Azure AI Search

> A customer is currently using Azure AI Search to manage and query their indexed data. To enhance security, they plan to enable server-side encryption and use customer-managed keys (CMK) stored in Azure Key Vault. This change aims to provide an additional layer of protection for their sensitive data. However, they need to understand the potential impacts of this change on their search service. What are three implications of enabling server-side encryption with CMK in Azure AI Search? 

- [ ] Azure Key Vault is required. ✅: `This is correct because Azure Key Vault is used to store and manage the customer-managed keys.`
- [ ] A self-signed X.509 certificate is required. ❌: `This is incorrect because Azure Key Vault manages the keys, and a self-signed certificate is not required.`
- [ ] The index size will increase. ✅: `This is correct because enabling server-side encryption with CMK typically results in some overhead, causing the index size to increase due to the encryption metadata.`
- [ ] The index size will decrease. ❌: `This is incorrect because enabling server-side encryption with CMK does not reduce the index size.`
- [ ] Query times will increase. ✅: `This is correct because using customer-managed keys can introduce additional latency due to the encryption and decryption processes.`
- [ ] Query times will decrease. ❌: `This is incorrect because using customer-managed keys can introduce additional latency, not reduce it.`

## Q17: Ensuring Responsible AI Principles in Sentiment Analysis for Bonuses

> You are building an AI solution that will use Sentiment Analysis results from surveys to calculate bonuses for customer service staff. You need to ensure that the solution meets the Microsoft responsible AI principles. What should you do?

- [ ] Include the Sentiment Analysis results when surveys return a low confidence score. ❌: `This is incorrect because including results with low confidence scores can lead to unreliable and unfair decisions, which does not align with responsible AI principles.`
- [ ] Use all the surveys, including surveys by customers who requested that their account be deleted and their data be removed. ❌: `This is incorrect because using data from customers who requested deletion violates privacy and security principles.`
- [ ] Publish the raw survey data to a central location and provide the staff with access to the location. ❌: `This is incorrect because publishing raw data can compromise privacy and security, and may not ensure fairness or accountability.`
- [ ] Add a human review and approval step before making decisions that affect the staff's financial situation. ✅: `This is correct because adding a human review and approval step ensures accountability and fairness, preventing automated decisions from negatively impacting staff without oversight.`

## Q18: Directing Messages to Language Support Teams

> You are building an app that will process incoming email and direct messages to either French or English language support teams. Which Azure AI Services API should you use? <br/>
> Answer: {Value1}{Value2} 

**Value1 Options:**

- [ ] api.AI.microsoft.com ❌: `This is incorrect because it is not the correct format for the endpoint.`
- [ ] eastus.api.AI.microsoft.com ✅: `This is correct because it follows the correct format for the endpoint, specifying the region (eastus).`
- [ ] portal.azure.com ❌: `This is incorrect because this is the URL for the Azure portal, not an API endpoint for language detection.`

**Value2 Options:**

- [ ] /text/analytics/v3.1/entities/recognition/general ❌: `This is incorrect because this endpoint is used for recognizing entities in text, not for detecting the language.`
- [ ] /text/analytics/v3.1/languages ✅: `This is correct because this endpoint is used for detecting the language of the input text.`
- [ ] /translator/text/v3.0/translate?to=en ❌: `This is incorrect because this endpoint is used for translating text to English, not for detecting the language.`
- [ ] /translator/text/v3.0/translate?to=fr ❌: `This is incorrect because this endpoint is used for translating text to French, not for detecting the language.`

## Q19: Configuring IP Firewall Rules for Azure AI Search

> You create a web app named `app1` that runs on an Azure virtual machine named `vm1`. `vm1` is on an Azure virtual network named `vnet1`. You plan to create a new Azure AI Search service named `service1`. You need to ensure that `app1` can connect directly to `service1` without routing traffic over the public internet. Which solution should you implement?

- [ ] Deploy `service1` with a private endpoint in `vnet1` and configure Azure Private Link. ✅: `This is correct because deploying `service1` with a private endpoint in the same virtual network and configuring Azure Private Link ensures that traffic between `app1` and `service1` does not traverse the public internet.`
- [ ] Deploy `service1` with a public endpoint and configure an IP firewall rule. ❌: `This is incorrect because using a public endpoint and IP firewall rule does not prevent traffic from traversing the public internet.`
- [ ] Deploy `service1` with a public endpoint and configure a VPN connection between `vnet1` and the public endpoint. ❌: `This is incorrect because using a public endpoint and VPN connection does not prevent traffic from traversing the public internet.`
- [ ] Deploy `service1` with a private endpoint in a different virtual network and configure Azure Private Link. ❌: `This is incorrect because deploying `service1` in a different virtual network would require additional configuration and does not ensure direct connectivity without traversing the public internet.`

## Q20: Converting Speech to Text for Streaming MP3 Data

> You need to develop a method to convert speech to text for streaming MP3 data. How should you complete the code?

```csharp
var audioFormat = ___________________________ (audioStream.ContainsFormat.MP3);

var audioConfig = AudioConfig.FromSubscription(pushStream, audioFormat);

using (var recognizer = ___________________________ (speechConfig, audioConfig))
{
    var result = await recognizer.RecognizeOnceAsync();
    var text = result.Text;
}
```

**Options for the first blank:**

- [ ] AudioConfig.SetProperty ❌: `This is incorrect because SetProperty is used to set properties on the audio configuration, not to get the audio format.`
- [ ] AudioConfig.GetCompressedFormat ✅: `This is correct because GetCompressedFormat is used to get the audio format for compressed audio streams like MP3.`
- [ ] AudioConfig.GetWaveFormatPCM ❌: `This is incorrect because GetWaveFormatPCM is used for uncompressed PCM audio, not for MP3.`
- [ ] PullAudioInputStream ❌: `This is incorrect because PullAudioInputStream is used to pull audio data from a stream, not to get the audio format.`

**Options for the second blank:**

- [ ] KeywordRecognizer ❌: `This is incorrect because KeywordRecognizer is used for recognizing specific keywords, not for general speech-to-text conversion.`
- [ ] SpeakerRecognizer ❌: `This is incorrect because SpeakerRecognizer is used for speaker identification and verification, not for general speech-to-text conversion.`
- [ ] SpeechRecognizer ✅: `This is correct because SpeechRecognizer is used for converting speech to text.`
- [ ] SpeechSynthesizer ❌: `This is incorrect because SpeechSynthesizer is used for converting text to speech, not for speech-to-text conversion.`

## Q21: Developing an Automated Call Handling System

> You need to develop an automated call handling system that can respond to callers in their own language. The system will support only French and English. Which Azure AI Services service should you use to meet each requirement? 

1. Detect the incoming language: ___________________________

- [ ] Speaker Recognition ❌: `This is incorrect because Speaker Recognition is used for identifying and verifying speakers, not for detecting the language of the incoming call.`
- [ ] Speech to Text ❌: `This is incorrect because Speech to Text converts spoken language into text but does not detect the language.`
- [ ] Text Analytics ✅: `This is correct because the Text Analytics service provides language detection capabilities to identify the language of the input text.`
- [ ] Text to Speech ❌: `This is incorrect because Text to Speech converts text into spoken language but does not detect the language.`
- [ ] Translator ✅: `This is correct because the Translator service can detect the language of the incoming call.`

2. Respond in the callers' own language: ___________________________

- [ ] Speaker Recognition ❌: `This is incorrect because Speaker Recognition is used for identifying and verifying speakers, not for responding in the caller's language.`
- [ ] Speech to Text ❌: `This is incorrect because Speech to Text converts spoken language into text but does not generate spoken responses.`
- [ ] Text Analytics ❌: `This is incorrect because Text Analytics is used for analyzing text data, not for generating spoken responses.`
- [ ] Text to Speech ✅: `This is correct because Text to Speech converts text into spoken language, allowing the system to respond in the caller's language.`
- [ ] Translator ❌: `This is incorrect because while Translator can translate text, it does not generate spoken responses.`

## Q22: Extracting Data from Receipts Using Form Recognizer

> You have receipts that are accessible from a URL. You need to extract data from the receipts by using Form Recognizer and the SDK. The solution must use a prebuilt model. Which client and method should you use?

- [ ] the FormRecognizerClient client and the StartRecognizeContentFromUri method ❌: `This is incorrect because the StartRecognizeContentFromUri method is used for recognizing content in general documents, not specifically for receipts.`
- [ ] the FormTrainingClient client and the StartRecognizeContentFromUri method ❌: `This is incorrect because the FormTrainingClient is used for training custom models, not for using prebuilt models.`
- [ ] the FormTrainingClient client and the StartRecognizeReceiptsFromUri method ❌: `This is incorrect because the FormTrainingClient is used for training custom models, not for using prebuilt models.`
- [ ] the FormRecognizerClient client and the StartRecognizeReceiptsFromUri method ✅: `This is correct because the FormRecognizerClient client and the StartRecognizeReceiptsFromUri method are used to extract data from receipts using the prebuilt receipt model.`

### Tip (Reference)
> [!TIP]
> Find below a quick reference:

| Service                  | Client                  | Method                                      | Description|
|--------------------------|-------------------------|---------------------------------------------|-----------------------------------------------------------------------------|
| Form Recognizer          | FormRecognizerClient    | StartRecognizeContentFromUri                | Recognizes content from a document using a prebuilt model.|
| Form Recognizer          | FormRecognizerClient    | StartRecognizeReceiptsFromUri               | Recognizes data from receipts using a prebuilt receipt model.|
| Form Recognizer          | FormTrainingClient      | StartTraining                               | Trains a custom model using labeled data.|
| Text Analytics           | TextAnalyticsClient     | AnalyzeSentiment                            | Analyzes the sentiment of the input text.|
| Text Analytics           | TextAnalyticsClient     | ExtractKeyPhrases                           | Extracts key phrases from the input text.|
| Text Analytics           | TextAnalyticsClient     | DetectLanguage                              | Detects the language of the input text.|
| Translator               | TranslatorClient        | TranslateText                               | Translates text from one language to another.|
| Speech                   | SpeechRecognizer        | RecognizeOnceAsync                          | Recognizes speech from an audio stream and converts it to text.|
| Speech                   | SpeechSynthesizer       | SpeakTextAsync                              | Converts text to speech.|
| Speech                   | SpeechRecognizer        | StartContinuousRecognitionAsync             | Starts continuous speech recognition.|
| Computer Vision          | ComputerVisionClient    | AnalyzeImage                                | Analyzes visual content in an image.|
| Computer Vision          | ComputerVisionClient    | DescribeImage                               | Generates a description of the content in an image.|
| Computer Vision          | ComputerVisionClient    | RecognizePrintedText                        | Recognizes printed text in an image.|
| Face                     | FaceClient              | DetectWithStreamAsync                       | Detects faces in an image stream.|
| Face                     | FaceClient              | IdentifyAsync                               | Identifies faces in a group of detected faces.|
| Face                     | FaceClient              | VerifyAsync                                 | Verifies whether two faces belong to the same person.|
| Custom Vision            | CustomVisionTrainingClient | CreateImageFromDataAsync                  | Creates an image from data for training a custom model.|
| Custom Vision            | CustomVisionPredictionClient | ClassifyImageAsync                       | Classifies an image using a custom model.|

## Q23: Reducing Throttling in Azure AI Search

> You have an Azure AI Search service. During the past 12 months, query volume steadily increased. You discover that some search query requests to the AI Search service are being throttled. You need to reduce the likelihood that search query requests are throttled. **Solution: You add indexes.** Does this meet the goal?

- [ ] Yes ❌: `This is incorrect because adding indexes does not directly address the issue of throttling caused by high query volume. Throttling is typically related to service capacity, not the number of indexes.`
- [ ] No ✅: `This is correct because adding indexes does not reduce throttling. To reduce throttling, you should consider increasing the service tier, adding more replicas, or optimizing query performance.`

## Q24: Analyzing Extracted Information from Purchase Orders Using Power BI

> You have an Azure AI Search instance that indexes purchase orders by using Form Recognizer. You need to analyze the extracted information by using Microsoft Power BI. The solution must minimize development effort. What should you add to the indexer?

- [ ] a projection group ❌: `This is incorrect because a projection group is not specifically used for integrating with Power BI.`
- [ ] a file projection ❌: `This is incorrect because a file projection is used for handling file data, not for structuring data for Power BI analysis.`
- [ ] an object projection ❌: `This is incorrect because an object projection is used for handling complex objects, not for structuring data for Power BI analysis.`
- [ ] a table projection ✅: `This is correct because a table projection organizes the extracted data into a tabular format, which can be easily consumed by Power BI for analysis.`

## Q25: Securing an Azure AI Search Resource

> You have an Azure AI Search resource named Search1 that is used by multiple apps. You need to secure Search1. The solution must meet the following requirements: <br/>
> - Prevent access to Search1 from the internet. <br/>
> - Limit the access of each app to specific queries. <br/>
> What should you do? 

**To prevent access from the internet:** ___________________________

- [ ] Configure an IP firewall. ❌: `This is incorrect because while configuring an IP firewall can restrict access to specific IP addresses, it does not fully prevent access from the internet.`
- [ ] Create a private endpoint. ✅: `This is correct because creating a private endpoint ensures that the Azure AI Search resource is only accessible within a virtual network, preventing access from the public internet.`
- [ ] Use Azure roles. ❌: `This is incorrect because Azure roles are used for managing permissions and access control, not for preventing access from the internet.`

**To limit access to queries:** ___________________________

- [ ] Create a private endpoint. ❌: `This is incorrect because creating a private endpoint is used to prevent access from the internet, not for limiting access to specific queries.`
- [ ] Use Azure roles. ✅: `This is correct because using Azure roles allows you to manage permissions and limit access to specific queries based on the roles assigned to each app.`
- [ ] Use key authentication. ❌: `This is incorrect because key authentication is used for authenticating requests, not for limiting access to specific queries.`

## Q26: Building a Monitoring Solution for PPE Compliance

> You have a factory that produces food products. You need to build a monitoring solution for staff compliance with personal protective equipment (PPE) requirements. The solution must meet the following requirements:  <br/>
> - Identify staff who have removed masks or safety glasses.  <br/>
> - Perform a compliance check every 15 minutes.  <br/>
> - Minimize development effort.  <br/>
> - Minimize costs. <br/>
> Which service should you use?

- [ ] Face ❌: `This is incorrect because while the Face service can detect and analyze facial features, including the presence of objects like masks and safety glasses, it is primarily used for facial recognition and verification. It may not be the most efficient solution for frequent compliance checks in a video stream.`
- [ ] Computer Vision ❌: `This is incorrect because while Computer Vision can analyze images, it may not be the most efficient solution for frequent compliance checks in a video stream.`
- [ ] Azure Video Analyzer for Media (formerly Video Indexer) ✅: `This is correct because Azure Video Analyzer for Media is designed to analyze video content and can be used to identify specific scenarios, such as whether individuals in a video are wearing masks or safety glasses. It supports a range of video analytics capabilities, including object detection, which can be leveraged to monitor PPE compliance. Using Azure Video Analyzer for Media can minimize development effort by providing built-in models for analyzing video content and can be set up to perform compliance checks at specified intervals, such as every 15 minutes.`

## Q27: Building an App for Anomaly Detection and Incident Alerts

> You have an Azure IoT hub that receives sensor data from machinery. You need to build an app that will perform the following actions: <br/>
> - Perform anomaly detection across multiple correlated sensors. <br/>
> - Identify the root cause of process stops. <br/>
> - Send incident alerts. <br/>
> - The solution must minimize development time. <br/>
> Which Azure service should you use?

- [ ] Azure Metrics Advisor ❌: `This is incorrect because Azure Metrics Advisor is primarily used for monitoring and diagnosing anomalies in time series data, but it may not be the best choice for identifying root causes and sending incident alerts.`
- [ ] Form Recognizer ❌: `This is incorrect because Form Recognizer is used for extracting text and data from forms and documents, not for anomaly detection or incident alerts.`
- [ ] Azure Machine Learning ❌: `This is incorrect because while Azure Machine Learning can be used for anomaly detection and root cause analysis, it requires more development effort compared to a specialized service like Anomaly Detector.`
- [ ] Anomaly Detector ✅: `This is correct because Anomaly Detector is designed to perform anomaly detection across multiple correlated sensors, identify the root cause of anomalies, and can be integrated with other services to send incident alerts. It minimizes development time by providing built-in models and APIs for anomaly detection.`

## Q28: Hosting an Azure AI Services Model with Limited Connectivity

> You have an app named App1 that uses an Azure AI Services model to identify anomalies in a time series data stream. You need to run App1 in a location that has limited connectivity. The solution must minimize costs. What should you use to host the model?

- [ ] a Kubernetes cluster hosted in an Azure Stack Hub integrated system ❌: `This is incorrect because while it allows running Kubernetes clusters on-premises, it may not be the most cost-effective solution compared to using the Docker Engine.`
- [ ] Azure Kubernetes Service (AKS) ❌: `This is incorrect because AKS is a managed Kubernetes service that requires a stable internet connection for management and scaling.`
- [ ] Azure Container Instances ❌: `This is incorrect because Azure Container Instances are designed for running containers in the cloud and require internet connectivity.`
- [ ] the Docker Engine ✅: `This is correct because the Docker Engine can run containers on-premises without requiring internet connectivity, making it a cost-effective solution for hosting the model in a location with limited connectivity.`

## Q29: Detecting Anomalies in Real-Time Sensor Data

> You are building a solution that will detect anomalies in sensor data from the previous 24 hours. You need to ensure that the solution detects anomalies in real-time as the data is being generated. Which type of detection should you use?

- [ ] batch ❌: `This is incorrect because batch detection processes data in large chunks at specific intervals, not in real-time.`
- [ ] streaming ✅: `This is correct because streaming detection processes data in real-time as it is being generated, allowing for immediate anomaly detection.`
- [ ] change points ❌: `This is incorrect because change point detection identifies points in time where the statistical properties of a time series change, but it is not specifically designed for real-time anomaly detection.`

## Q30: Ensuring Confidential Documents Remain On-Premises with Azure AI Services

> You are building an app that will scan confidential documents and use the Language service to analyze the contents. You provision an Azure AI Services resource. You need to ensure that the app can make requests to the Language service endpoint. The solution must ensure that confidential documents remain on-premises. Which three actions should you perform in sequence?

- [ ] Run the container and specify an App ID and Client Secret. ❌: `This is incorrect because specifying an App ID and Client Secret is not the first step in ensuring that confidential documents remain on-premises.`
- [ ] Provision an on-premises Kubernetes cluster that is located under your desk. ❌: `This is incorrect because provisioning a Kubernetes cluster under your desk is not a practical or scalable solution for ensuring that confidential documents remain on-premises.`
- [ ] Provision an on-premises Kubernetes cluster that has internet connectivity. 1️⃣: `This is correct because provisioning an on-premises Kubernetes cluster with internet connectivity is the first step to host the containerized Language service while ensuring that confidential documents remain on-premises.`
- [ ] Pull an image from Microsoft Container Registry (MCR). 2️⃣: `This is correct because pulling an image from Microsoft Container Registry (MCR) is necessary to get the container image for the Language service.`
- [ ] Run the container and specify an App ID and then inject URI of AI Services. 3️⃣: `This is correct because running the container and specifying an App ID and injecting the URI of AI Services is necessary to configure the container to communicate with the Language service endpoint.`
- [ ] Pull an image from Docker Hub. ❌: `This is incorrect because pulling an image from Docker Hub is not the recommended source for the Language service container image.`
- [ ] Provision a Kubernetes Service (AKS) resource. ❌: `This is incorrect because provisioning a Kubernetes Service (AKS) resource does not ensure that confidential documents remain on-premises.`

## Q31: Authenticating to the Speech Service Using Azure AD

> You are building an app that will use the Speech service. You need to ensure that the app can authenticate to the service by using a Microsoft Azure Active Directory (Azure AD), part of Microsoft Entra, token. Which two actions should you perform? 

- [ ] Enable a virtual network service endpoint. ❌: `This is incorrect because enabling a virtual network service endpoint is not required for Azure AD authentication.`
- [ ] Configure a custom subdomain. 1️⃣ `This is correct because configuring a custom subdomain is necessary for setting up Azure AD authentication with the Speech service.`
- [ ] Request an X.509 certificate. ❌: `This is incorrect because requesting an X.509 certificate is not required for Azure AD authentication.`
- [ ] Create a private endpoint. 2️⃣ `This is correct because creating a private endpoint ensures secure communication between the app and the Speech service, preventing traffic from traversing the public internet.`
- [ ] Assign Azure roles to the application. ❌: `This is incorrect because while assigning Azure roles is important for managing permissions, it is not specifically required for Azure AD authentication with the Speech service.`

## Q32: Implementing Real-Time Translation in a Multilingual Chat Application

> You are developing a multilingual chat application that needs to translate messages between multiple languages in real-time. The application must support translation for text messages and provide language detection capabilities. Which Azure AI Service should you use for each requirement?

To translate text messages between multiple languages: ___________________________

- [ ] Text Analytics ❌: `This is incorrect because Text Analytics is used for analyzing text data, not for translating text.`
- [ ] Translator Text ✅: `This is correct because the Translator Text service is specifically designed for translating text between multiple languages.`
- [ ] Speech to Text ❌: `This is incorrect because Speech to Text converts spoken language into text but does not translate text.`

To detect the language of the input text: ___________________________

- [ ] Text Analytics ✅: `This is correct because the Text Analytics service provides language detection capabilities to identify the language of the input text.`
- [ ] Translator Text ❌: `This is incorrect because while Translator Text includes language detection capabilities, the primary service for language detection is Text Analytics.`
- [ ] Speech to Text ❌: `This is incorrect because Speech to Text converts spoken language into text but does not detect the language of text.`

## Q33: Hosting an Anomaly Detector Instance on a Docker Host

> You have an Azure subscription that contains an Anomaly Detector resource. You deploy a Docker host server named Server1 to the on-premises network. You need to host an instance of the Anomaly Detector service on Server1. Which parameter should you include in the docker run command?

- [ ] Fluentd ❌: `This is incorrect because Fluentd is used for logging and does not relate to hosting the Anomaly Detector service.`
- [ ] Http Proxy ❌: `This is incorrect because Http Proxy is used for configuring proxy settings and is not required for hosting the Anomaly Detector service.`
- [ ] Mounts ❌: `This is incorrect because Mounts are used for mounting volumes and directories, not for specifying billing information.`
- [ ] Billing ✅: `This is correct because the Billing parameter specifies the endpoint URI for billing purposes, which is required to run the Anomaly Detector container.`

> [!TIP]
> This command ensures that the Anomaly Detector service runs in a Docker container on Server1, with the necessary configurations for memory, CPU, and network settings:

```bash
docker run --rm -it -p 5000:5000 --memory 4g --cpus 1 \
mcr.microsoft.com/azure-AI-services/decision/anomaly-detector:latest \
Eula=accept \
Billing={ENDPOINT_URI} \
ApiKey={API_KEY}
```

- **docker run**: This command starts a new container.
- **--rm**: Automatically removes the container when it exits.
- **-it**: Runs the container in interactive mode with a terminal.
- **-p 5000:5000**: Maps port 5000 on the host to port 5000 in the container.
- **--memory 4g**: Allocates 4 GB of memory to the container.
- **--cpus 1**: Allocates 1 CPU to the container.
- **mcr.microsoft.com/azure-AI-services/decision/anomaly-detector:latest**: Specifies the container image to use.
- **Eula=accept**: Accepts the End User License Agreement.
- **Billing={ENDPOINT_URI}**: Specifies the endpoint URI for billing purposes.
- **ApiKey={API_KEY}**: Specifies the API key for authentication.

## Q34: Configuring Capacity for an Azure OpenAI Resource

> You plan to deploy an Azure OpenAI resource by using an Azure Resource Manager (ARM) template. The resource must be capable of handling 600 requests per minute. How should you complete the template?

```json
{
    "type": "Microsoft.AIServices/accounts/deployments",
    "apiVersion": "2023-05-01",
    "name": "[parameters('arm-aaoai-sample-resource/arm-je-std-deployment')]",
    "dependsOn": [
        "[resourceId('Microsoft.AIServices/accounts', 'arm-aaoai-sample-resource')]"
    ],
    "sku": {
        "name": "Standard",
        "capacity": "_________________"
    },
    "properties": {
        "model": {
            "format": "OpenAI",
            "name": "GPT-4"
        }
    }
}
```

- [ ] 1 Capacity Unit ❌: `This is incorrect because 1 capacity unit is not sufficient to handle 600 requests per minute.`
- [ ] 10 Capacity Units ✅: `This is correct because 10 capacity units are required to handle 600 requests per minute, as each capacity unit supports 60 requests per minute.`
- [ ] 100 Capacity Units ❌: `This is incorrect because 100 capacity units exceed the requirement and would incur unnecessary costs.`

## Q35: Detecting Negative Comments Using Sentiment Analysis API

> You need to ensure that the app can detect negative comments by using the Sentiment Analysis API in Azure AI Language. The solution must ensure that the managed feedback remains on your company's internal network. Which three actions should you perform in sequence? 

- [ ] Identify the Language service endpoint URL and key. ❌: `This is incorrect because identifying the endpoint URL and key is not the first step in setting up the Sentiment Analysis API.`
- [ ] Provision the Language service resource in Azure. 1️⃣ ✅: `This is correct because provisioning the Language service resource is the first step to set up the Sentiment Analysis API.`
- [ ] Run the container and query a prediction endpoint. 3️⃣ ✅: `This is correct because running the container and querying the prediction endpoint allows you to use the Sentiment Analysis API while keeping the data on-premises.`
- [ ] Deploy a Docker container to an on-premises server. 2️⃣ ✅: `This is correct because deploying a Docker container on an on-premises server ensures that the managed feedback remains on your company’s internal network.`
- [ ] Deploy a Docker container to an Azure container instance. ❌: `This is incorrect because deploying to an Azure container instance does not ensure that the data remains on-premises.`

## Q36: Providing Access to Azure OpenAI Resource and Connecting to Deployments

> You have an Azure OpenAI resource named AI1 that hosts three deployments of the GPT 3.5 model. Each deployment is optimized for a unique workload. You plan to deploy three apps. Each app will access AI1 by using the REST API and will use the deployment that was optimized for the app’s intended workload. You need to provide each app with access to AI1 and the appropriate deployment. The solution must ensure that only the apps can access AI1. What should you use to provide access to AI1, and what should each app use to connect to its appropriate deployment? 

**Provide access to AI1 by using:** ___________________________

- [ ] An API key ✅: `This is correct because an API key provides secure access to the Azure OpenAI resource and ensures that only authorized apps can access AI1.`
- [ ] A bearer token ❌: `This is incorrect because a bearer token is typically used for OAuth 2.0 authentication, not for accessing Azure OpenAI resources.`
- [ ] A shared access signature (SAS) token ❌: `This is incorrect because SAS tokens are used for granting limited access to Azure Storage resources, not for Azure OpenAI resources.`

**Connect to the deployment by using:** ___________________________

- [ ] An API key ❌: `This is incorrect because an API key is used for authentication, not for specifying the deployment.`
- [ ] A deployment endpoint ✅: `This is correct because each app should use the specific deployment endpoint to connect to the deployment optimized for its workload.`
- [ ] A deployment name ❌: `This is incorrect because the deployment name alone does not provide the necessary connection details.`
- [ ] A deployment type ❌: `This is incorrect because the deployment type does not specify the connection details for the deployment.`


## Q37: Configuring App1 to Connect to Azure OpenAI Model AI1

> You have an Azure OpenAI model named AI1. You are building a web app named App1 by using the Azure OpenAI SDK. You need to configure App1 to connect to AI1. What information must you provide?

- [ ] the endpoint, key, and model name ❌: `This is incorrect because the model name alone is not sufficient to connect to the specific deployment.`
- [ ] the deployment name, key, and model name ❌: `This is incorrect because the model name alone is not sufficient to connect to the specific deployment.`
- [ ] the endpoint, key, and model type ❌: `This is incorrect because the model type alone is not sufficient to connect to the specific deployment.`
- [ ] the deployment name, endpoint, and key ✅: `This is correct because you need the deployment name to specify which deployment to use, the endpoint to connect to the Azure OpenAI resource, and the key for authentication.`

## Q38: Monitoring Temperature Data and Generating Alerts

> You are developing a system for monitoring temperature data from a data stream. The system must generate an alert in response to atypical values and minimize development effort. What should you include in the solution?

- [ ] Multivariate Anomaly Detection ❌: `This is incorrect because Multivariate Anomaly Detection is used for detecting anomalies across multiple correlated variables, but it may not be the simplest solution for monitoring a single data stream.`
- [ ] Azure Stream Analytics ✅: `This is correct because Azure Stream Analytics can process real-time data streams and generate alerts based on predefined conditions, minimizing development effort.`
- [ ] metric alerts in Azure Monitor ❌: `This is incorrect because metric alerts in Azure Monitor are used for monitoring metrics and generating alerts, but they may not be the most efficient solution for processing real-time data streams.`
- [ ] Univariate Anomaly Detection ❌: `This is incorrect because Univariate Anomaly Detection is used for detecting anomalies in a single time series, but it may not provide the necessary alerting capabilities.`

## Q39: Implementing Predictive Maintenance with Azure Services

> You plan to perform predictive maintenance. You collect IoT sensor data from 100 industrial machines for a year. Each machine has 500 different sensors that generate data at one-minute intervals. In total, you have 50,000 time series datasets. You need to identify unusual values in each time series to help predict machinery failures. Which Azure service should you use?

- [ ] Azure AI Computer Vision ❌: `This is incorrect because Computer Vision is used for analyzing visual content in images and videos, not for detecting anomalies in time series data.`
- [ ] Cognitive Search ❌: `This is incorrect because Cognitive Search is used for indexing and searching text and documents, not for detecting anomalies in time series data.`
- [ ] Azure AI Document Intelligence ❌: `This is incorrect because Document Intelligence is used for extracting information from documents, not for detecting anomalies in time series data.`
- [ ] Azure AI Anomaly Detector ✅: `This is correct because Anomaly Detector is specifically designed to identify unusual values in time series data, making it ideal for predictive maintenance.`

## Q40: Indexing a Large Video File Using Azure Video Indexer

> You have a Microsoft OneDrive folder that contains a 20-GB video file named File1.avi. You need to index File1.avi by using the Azure Video Indexer website. What should you do?

- [ ] Upload File1.avi to the www.youtube.com webpage, and then copy the URL of the video to the Azure AI Video Indexer website. ❌: `This is incorrect because URLs from streaming services like YouTube are not supported by Azure Video Indexer for indexing.`
- [ ] Download File1.avi to a local computer, and then upload the file to the Azure AI Video Indexer website. ❌: `This is incorrect because downloading and re-uploading a large file is not efficient and may not be necessary.`
- [ ] From OneDrive, create a download link, and then copy the link to the Azure AI Video Indexer website. ❌: `This is incorrect because a download link does not provide the necessary access for Azure Video Indexer to index the file.`
- [ ] From OneDrive, create a sharing link for File1.avi, and then copy the link to the Azure AI Video Indexer website. ✅: `This is correct because creating a sharing link from OneDrive provides a publicly accessible URL that Azure Video Indexer can use to index the video file.`

## Q41: Securing Access to Azure AI Service Resource

> You have an Azure subscription that contains an Azure AI Service resource named AIServiceAccount and a virtual network named VNet1. AIServiceAccount is connected to VNet1. You need to ensure that only specific resources can access AIServiceAccount. The solution must meet the following requirements: <br/>
> - Prevent external access to AIServiceAccount.  <br/>
> - Minimize administrative effort.  <br/>
> Which two actions should you perform? Each correct answer presents part of the solution.

- [ ] In VNet1, enable a service endpoint for AIServiceAccount. ✅: `This is correct because enabling a service endpoint allows you to secure your Azure service resources to the virtual network, ensuring that only resources within VNet1 can access AIServiceAccount.`
- [ ] In AIServiceAccount, configure the Access control (IAM) settings. ❌: `This is incorrect because configuring IAM settings alone does not prevent external access.`
- [ ] In VNet1, modify the virtual network settings. ❌: `This is incorrect because modifying virtual network settings alone does not fully prevent external access.`
- [ ] In VNet1, create a subnet. ❌: `This is incorrect because creating a subnet alone does not prevent external access.`
- [ ] In AIServiceAccount, modify the virtual network settings. ✅: `This is correct because modifying the virtual network settings in AIServiceAccount allows you to configure it to accept connections only from the virtual network VNet1, effectively preventing external access.`

## Q42: Monitoring a Video Stream and Detecting Questions

> You are building an internet-based training solution. The solution requires that a user's camera and microphone remain enabled. You need to monitor a video stream of the user and detect when the user asks an instructor a question. The solution must minimize development effort. What should you include in the solution?

- [ ] language detection in Azure AI Language Service ❌: `This is incorrect because language detection identifies the language of the text but does not detect when a user asks a question.`
- [ ] the Face service in Azure AI Vision ❌: `This is incorrect because the Face service is used for facial recognition and analysis, not for detecting spoken questions.`
- [ ] object detection in Azure AI Custom Vision ❌: `This is incorrect because object detection identifies objects in images or videos, not for detecting spoken questions.`
- [ ] speech-to-text in the Azure AI Speech service ✅: `This is correct because speech-to-text can convert spoken questions into text, allowing the system to detect when a user asks a question.`

## Q43: Identifying the Created Azure AI Services Account in Azure DevOps Pipeline

> You have an Azure DevOps pipeline named Pipeline1 that is used to deploy an app. Pipeline1 includes a step that will create an Azure AI services account. You need to add a step to Pipeline1 that will identify the created Azure AI services account. The solution must minimize development effort. Which Azure Command-Line Interface (CLI) command should you run?

- [ ] az resource link ❌: `This is incorrect because az resource link is used to link resources, not to identify a created Azure AI services account.`
- [ ] az cognitiveservices account network-rule ❌: `This is incorrect because az cognitiveservices account network-rule is used to manage network rules for a Cognitive Services account, not to identify the account.`
- [ ] az account list ❌: `This is incorrect because az account list lists all Azure accounts, not specific details about a created Azure AI services account.`
- [ ] az cognitiveservices account show ✅: `This is correct because az cognitiveservices account show retrieves information about a specific Cognitive Services account, allowing you to identify the created account.`

## Q44: Extracting Data from Hand-Written Survey Responses Using Azure AI Document Intelligence

> You have 10,000 scanned images of hand-written survey responses. The surveys do NOT have a consistent layout. You need an Azure subscription that contains an Azure AI Document Intelligence resource named Aldoc1. You open Document Intelligence Studio and create a new project. You need to extract data from the survey responses. The solution must minimize development effort. Where should you upload the images, and which type of model should you use? 

**Upload to:** ___________________________

- [ ] An Azure Cosmos DB account ❌: `This is incorrect because Azure Cosmos DB is used for globally distributed databases, not for storing and processing images for Document Intelligence.`
- [ ] An Azure Files share ❌: `This is incorrect because Azure Files is used for file shares, not for storing and processing images for Document Intelligence.`
- [ ] An Azure Storage account ✅: `This is correct because Azure Storage is used to store the images, which can then be accessed by Document Intelligence for processing.`

**Model type:** ___________________________

- [ ] Custom neural ✅: `This is correct because a custom neural model is suitable for extracting data from documents with inconsistent layouts, such as hand-written survey responses.`
- [ ] Custom template ❌: `This is incorrect because custom template models are better suited for documents with consistent layouts.`
- [ ] Identity document (ID) ❌: `This is incorrect because identity document models are specifically designed for processing identity documents, not survey responses.`

<!-- START BADGE -->
<div align="center">
  <img src="https://img.shields.io/badge/Total%20views-1436-limegreen" alt="Total views">
  <p>Refresh Date: 2025-08-05</p>
</div>
<!-- END BADGE -->
