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

</details>

## Q: Configuring Index Attributes for Azure AI Search

> You have an Azure AI Search solution and a collection of blog posts that include a category field. You need to index the posts. The solution must meet the following requirements: <br/>
> - Include the category field in the search results. <br/>
> - Ensure that users can search for words in the category field. <br/>
> - Ensure that users can perform drill down filtering based on category. <br/>
> Which index attributes should you configure for the category field?

**Options:**

- [ ] A. searchable, sortable, and retrievable ❌: `This is incorrect because while these attributes allow searching and sorting, they do not support drill down filtering.`
- [ ] retrievable, filterable, and sortable ❌: `This is incorrect because while these attributes allow filtering and sorting, they do not support searching for words in the category field.`
- [ ] retrievable, facetable, and key ❌: `This is incorrect because the 'key' attribute is used for unique identifiers, not for enabling search or filtering capabilities.`
- [ ] searchable, facetable, and retrievable ✅: `This is correct because these attributes allow the category field to be included in search results, support searching for words in the category field, and enable drill down filtering based on category.`

## Q: Configuring Azure AI Services for Text Translation

> You are developing a multilingual application that needs to translate text between multiple languages. You plan to use Azure AI Services to achieve this. Which Azure AI Service should you use for each requirement? 

**Answer:**

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


## Q: Managing Access in Language Understanding (LUIS)

> You are building a language model by using a Language Understanding (classic) service. You create a new Language Understanding (classic) resource. You need to add more contributors. What should you use?

**Options:**

- [ ] a conditional access policy in Azure Active Directory (Azure AD) ❌: `This is incorrect because a conditional access policy is used to control access to resources based on conditions, not for adding contributors.`
- [ ] the Access control (IAM) page for the authoring resources in the Azure portal ✅: `This is correct because the Access control (IAM) page for the authoring resources is where you can manage roles and add contributors to the Language Understanding (classic) resource.`
- [ ] the Access control (IAM) page for the prediction resources in the Azure portal ❌: `This is incorrect because the Access control (IAM) page for the prediction resources is used for managing access to prediction resources, not for adding contributors to the authoring resources.`

## Q: Configuring an Enrichment Pipeline for OCR and Text Analytics

> You have a collection of 50,000 scanned documents that contain text. You plan to make the text available through Azure AI Search. You need to configure an enrichment pipeline to perform optical character recognition (OCR) and text analytics. The solution must minimize costs. What should you attach to the skillset?

**Options:**

- [ ] A. a new Computer Vision resource ❌: `This is incorrect because while the Computer Vision service can perform OCR, it does not provide text analytics capabilities.`
- [ ] B. a free (limited enrichments) AI Services resource ❌: `This is incorrect because a multiservice account does not support the free tier (F0), and the free tier is not suitable for processing a large volume of documents like 50,000.`
- [ ] C. an Azure Machine Learning Designer pipeline ❌: `This is incorrect because an Azure Machine Learning Designer pipeline is not required for OCR and text analytics in this scenario.`
- [ ] D. a new AI Services resource that uses the S0 pricing tier ✅: `This is correct because a multiservice AI Services resource using the S0 pricing tier can provide both OCR and text analytics capabilities, and it is suitable for processing a large volume of documents.`

## Q: Managing Query Throttling in Azure AI Search

> You have an Azure AI Search service. During the past 12 months, query volume steadily increased. You discover that some search query requests to the AI Search service are being throttled. You need to reduce the likelihood that search query requests are throttled. Which solution should you implement?

**Options:**

- [ ] Configure a AI Search service that uses a higher tier. ✅: `This is correct because using a higher tier provides more resources and can handle a higher query volume, reducing the likelihood of throttling.`
- [ ] Add more replicas to the AI Search service. ✅: `This is correct because adding more replicas can distribute the query load and reduce the likelihood of throttling.`
- [ ] Enable query caching in the AI Search service. ❌: `This is incorrect because query caching is not a feature of Azure AI Search and does not address throttling issues.`
- [ ] Increase the timeout setting for search queries. ❌: `This is incorrect because increasing the timeout setting does not reduce throttling; it only allows queries to run longer before timing out.`

## Q: Choosing the Right Azure Service for Predictive Maintenance

> You plan to perform predictive maintenance. You collect IoT sensor data from 1000 industrial machines for a year. Each machine has 50 different sensors that generate data at one-minute intervals. In total, you have 50,000 time series datasets. You need to identify unusual values in each time series to help predict machinery failures. Which Azure service should you use?

**Options:**

- [ ] Azure Machine Learning ❌: `This is incorrect because while Azure Machine Learning can be used for predictive maintenance, it requires more setup and customization compared to a specialized service like Anomaly Detector.`
- [ ] Azure Stream Analytics ❌: `This is incorrect because Azure Stream Analytics is designed for real-time data processing and analytics, not specifically for detecting anomalies in time series data.`
- [ ] Azure Time Series Insights ❌: `This is incorrect because Azure Time Series Insights is used for visualizing and exploring time series data, not specifically for detecting anomalies.`
- [ ] Anomaly Detector ✅: `This is correct because Anomaly Detector is specifically designed to identify unusual values in time series data, making it ideal for predictive maintenance.`

## Q: Configuring Private Endpoint for Azure AI Search

> You create a web app named `app1` that runs on an Azure virtual machine named `vm1`. `vm1` is on an Azure virtual network named `vnet1`. You plan to create a new Azure AI Search service named `service1`. You need to ensure that `app1` can connect directly to `service1` without routing traffic over the public internet. Which solution should you implement?

**Options:**

- [ ] Deploy `service1` with a private endpoint in `vnet1` and configure Azure Private Link. ✅: `This is correct because deploying `service1` with a private endpoint in the same virtual network and configuring Azure Private Link ensures that traffic between `app1` and `service1` does not traverse the public internet.`
- [ ] Deploy `service1` with a public endpoint and configure a VPN connection between `vnet1` and the public endpoint. ❌: `This is incorrect because using a public endpoint and VPN connection does not prevent traffic from traversing the public internet.`
- [ ] Deploy `service1` with a public endpoint and configure a service endpoint in `vnet1`. ❌: `This is incorrect because service endpoints do not provide the same level of security as private endpoints and still allow traffic to traverse the public internet.`
- [ ] Deploy `service1` with a private endpoint in a different virtual network and configure Azure Private Link. ❌: `This is incorrect because deploying `service1` in a different virtual network would require additional configuration and does not ensure direct connectivity without traversing the public internet.`


## Q: Ensuring Fairness in a Sales System

> You are developing a new sales system that will process video and text from a public-facing website. To ensure fairness, you plan to implement measures that prevent bias in the system's recommendations and decisions. Which two actions should you take to ensure fairness? 
**Options:**

- [ ] Conduct regular bias assessments on the system's algorithms. ✅: `This is correct because conducting regular bias assessments helps identify and mitigate any biases in the system's algorithms, ensuring fair outcomes.`
- [ ] Ensure transparency in how the system makes decisions. ❌: `This is incorrect because while transparency is important, it does not directly address the prevention of bias in recommendations and decisions.`
- [ ] Include diverse data sets during the training phase. ✅: `This is correct because including diverse data sets helps ensure that the system's algorithms are trained on a wide range of scenarios, reducing the risk of bias.`
- [ ] Implement strict data privacy measures. ❌: `This is incorrect because data privacy measures focus on protecting user data, not directly on ensuring fairness in recommendations and decisions.`
- [ ] Use only historical data for training the system. ❌: `This is incorrect because relying solely on historical data can perpetuate existing biases, rather than ensuring fairness.`

## Q: Deploying Anomaly Detector API Containers

> You plan to use containerized versions of the Anomaly Detector API on cloud devices for testing and in on-premises datacenters. You need to ensure that containerized deployments meet the following requirements:
> - Prevent billing and API information from being stored in the command-line histories of the devices that run the container. <br/>
> - Control access to the container images by using Azure role-based access control (Azure RBAC). <br/>
> Which four actions should you perform in sequence? To answer, move the appropriate actions from the list of actions to the answer area and arrange them in the correct order.

**Actions:**

- [ ] Create a custom Dockerfile. 1️⃣ `This is correct because creating a custom Dockerfile is the first step in defining the container environment.`
- [ ] Pull the Anomaly Detector container image. 2️⃣ `This is correct because pulling the Anomaly Detector container image is necessary to get the base image for your custom Dockerfile.`
- [ ] Build the image. 3️⃣ `This is correct because building the image compiles the Dockerfile and creates the container image.`
- [ ] Push the image to an Azure container registry. 4️⃣ `This is correct because pushing the image to an Azure container registry allows you to control access using Azure RBAC.`
- [ ] Distribute a docker run script. ❌ `This is incorrect because distributing a docker run script is not necessary for controlling access or preventing billing and API information from being stored in command-line histories.`
- [ ] Push the image to Docker Hub. ❌ `This is incorrect because pushing the image to Docker Hub does not meet the requirement of controlling access using Azure RBAC.`


## Q: Ensuring Direct Connectivity for Azure AI Search

> You create a web app named `app1` that runs on an Azure virtual machine named `vm1`. `vm1` is on an Azure virtual network named `vnet1`. You plan to create a new Azure AI Search service named `service1`. You need to ensure that `app1` can connect directly to `service1` without routing traffic over the public internet. <br/>
> **Solution: You deploy `service1` and a private endpoint to `vnet1`.** Does this meet the goal?

**Options:**

- [ ] Yes ✅: `This is correct because deploying `service1` with a private endpoint in `vnet1` ensures that traffic between `app1` and `service1` does not traverse the public internet, providing a secure and direct connection.`
- [ ] No ❌: `This is incorrect because deploying `service1` with a private endpoint in `vnet1` does meet the goal of ensuring direct connectivity without using the public internet.`

## Q: Ensuring Inclusiveness in an Azure Bot

> You have a Language Understanding resource named `lu1`. You build and deploy an Azure bot named `bot1` that uses `lu1`. You need to ensure that `bot1` adheres to the Microsoft responsible AI principle of inclusiveness. How should you extend `bot1`?

**Options:**

- [ ] A. Implement authentication for `bot1` ❌: `This is incorrect because implementing authentication does not directly address the principle of inclusiveness.`
- [ ] B. Enable active learning for `lu1` ❌: `This is incorrect because enabling active learning improves the model's accuracy over time but does not directly address inclusiveness.`
- [ ] C. Host `lu1` in a container ❌: `This is incorrect because hosting `lu1` in a container does not directly address the principle of inclusiveness.`
- [ ] D. Add Direct Line Speech to `bot1` ✅: `This is correct because adding Direct Line Speech allows the bot to support speech interactions, making it more accessible and inclusive for users who may have difficulty typing or reading.`

## Q: Ensuring Transparency and Privacy in a Sales System

> You are developing a new sales system that will process video and text from a public-facing website. You plan to monitor the sales system to ensure that it provides transparent and secure results. Which two responsible AI principles provide guidance to meet the monitoring requirements? 

**Options:**

- [ ] transparency ✅: `This is correct because transparency ensures that AI systems are understandable and explainable, which is crucial for monitoring and providing transparent results.`
- [ ] fairness ❌: `This is incorrect because fairness focuses on providing unbiased outcomes, not directly on transparency and security.`
- [ ] inclusiveness ❌: `This is incorrect because inclusiveness focuses on ensuring diverse perspectives in AI development, not directly on transparency and security.`
- [ ] reliability and safety ❌: `This is incorrect because reliability and safety focus on ensuring consistent performance and preventing harm, not directly on transparency and security.` 
- [ ] privacy and security ✅: `This is correct because privacy and security focus on protecting user data, which is essential for ensuring secure results.`

## Q: Automating Invoice Processing

> Your company receives numerous invoices in English and wants to automate the process of extracting key information such as invoice number, date, and total amount. The solution should require minimal development effort and be able to handle various invoice formats. Which Azure service should you use?

**Options:**
- [ ] **A. Custom Vision** ❌: `This is incorrect because Custom Vision is used for image classification and object detection, not for extracting text from documents.`
- [ ] **B. Form Recognizer** ✅: `This is correct because Form Recognizer is designed to extract key information from documents, such as invoices, with minimal development effort.`
- [ ] **C Computer Vision** ❌: `This is incorrect because Computer Vision is used for analyzing images and extracting text, but it is not specialized for extracting structured information from documents like invoices.`
- [ ] **D. Personalizer** ❌: `This is incorrect because Personalizer is used for creating personalized user experiences, not for extracting information from documents.`

## Q: Reducing Throttling in Azure AI Search

> You have an Azure AI Search service. During the past 12 months, query volume steadily increased. You discover that some search query requests to the AI Search service are being throttled. You need to reduce the likelihood that search query requests are throttled. **Solution: You enable customer-managed key (CMK) encryption.** Does this meet the goal?

**Options:**

- [ ] Yes ❌: `This is incorrect because enabling customer-managed key (CMK) encryption does not address the issue of throttling caused by high query volume. Throttling is typically related to service capacity, not encryption settings.`
- [ ] No ✅: `This is correct because enabling customer-managed key (CMK) encryption does not reduce throttling. To reduce throttling, you should consider increasing the service tier, adding more replicas, or optimizing query performance.`

## Q: Ensuring Direct Connectivity for Azure AI Search

> You create a web app named `app1` that runs on an Azure virtual machine named `vm1`. `vm1` is on an Azure virtual network named `vnet1`. You plan to create a new Azure AI Search service named `service1`. You need to ensure that `app1` can connect directly to `service1` without routing traffic over the public internet. <br/>
> Solution: You deploy `service1` with a public endpoint and configure a network security group (NSG) for `vnet1`. Does this meet the goal?

- [ ] Yes ❌
- [ ] No ✅. The correct answer is **No**. Configuring a network security group (NSG) for `vnet1` does not prevent traffic from routing over the public internet. To ensure direct connectivity without using the public internet, you should deploy `service1` with a private endpoint and configure Azure Private Link.

## Q: Deploying a Language Understanding Application to a Container

> You plan to use a Language Understanding application named `app19467` that is deployed to a container `container27362`. The application was developed using a Language Understanding authoring resource named `lu17392n`. The application has the following versions:

| Version | Trained Date | Published Date |
|---------|--------------|----------------|
| V1.3    | None   | None |
| V1.2    | 2020-10-01   | None           |
| V1.1    | 2020-09-10   | 2020-09-15     |

> You need to create a container that uses the latest deployed version of `app19467`. What steps should you take to achieve this?

**Actions:**

- [ ] **Run a container that has version set as an environment variable.** ❌ `This action is not necessary for deploying the model.`
- [ ] **Export the model by using the Export as JSON option.** ❌ `This option is not suitable for container deployment.`
- [ ] **Select v1.2 of `app1`.** ❌ `This version has not been published yet.`
- [ ] **Run a container and mount the model file.** ✅ `This action deploys the model to the container using the exported file.`
- [ ] **Select v1.1 of `app1`.** ✅ `Given that v1.2 is not an option, v1.1 is the latest published version.`
- [ ] **Export the model by using the Export for containers (GZIP) option.** ✅ `This prepares the model for deployment in a container.`

Answer:

| **Action** | **Explanation**                                                                                   |
|------------|---------------------------------------------------------------------------------------------------|
| `Select v1.1 of app1` | This is correct because v1.1 is the latest published version of the application.        |
| `Export the model by using the Export for containers (GZIP) option` | This prepares the model for deployment in a container. |
| `Run a container and mount the model file` | This deploys the model to the container using the exported file. |

## Q: Enabling Server-Side Encryption with Customer-Managed Keys in Azure AI Search

> A customer is currently using Azure AI Search to manage and query their indexed data. To enhance security, they plan to enable server-side encryption and use customer-managed keys (CMK) stored in Azure Key Vault. This change aims to provide an additional layer of protection for their sensitive data. However, they need to understand the potential impacts of this change on their search service. What are three implications of enabling server-side encryption with CMK in Azure AI Search? 

**Options:**

- [ ] Azure Key Vault is required. ✅: `This is correct because Azure Key Vault is used to store and manage the customer-managed keys.`
- [ ] A self-signed X.509 certificate is required. ❌: `This is incorrect because Azure Key Vault manages the keys, and a self-signed certificate is not required.`
- [ ] The index size will increase. ✅: `This is correct because enabling server-side encryption with CMK typically results in some overhead, causing the index size to increase due to the encryption metadata.`
- [ ] The index size will decrease. ❌: `This is incorrect because enabling server-side encryption with CMK does not reduce the index size.`
- [ ] Query times will increase. ✅: `This is correct because using customer-managed keys can introduce additional latency due to the encryption and decryption processes.`
- [ ] Query times will decrease. ❌: `This is incorrect because using customer-managed keys can introduce additional latency, not reduce it.`


## Q: Directing Messages to Language Support Teams

> You are building an app that will process incoming email and direct messages to either French or English language support teams. Which Azure AI Services API should you use? <br/>
> **Answer:** {Value1}{Value2} 

**Value1 Options:**

- [ ] api.AI.microsoft.com ❌: `This is incorrect because it is not the correct format for the endpoint.`
- [ ] eastus.api.AI.microsoft.com ✅: `This is correct because it follows the correct format for the endpoint, specifying the region (eastus).`
- [ ] portal.azure.com ❌: `This is incorrect because this is the URL for the Azure portal, not an API endpoint for language detection.`

**Value2 Options:**

- [ ] /text/analytics/v3.1/entities/recognition/general ❌: `This is incorrect because this endpoint is used for recognizing entities in text, not for detecting the language.`
- [ ] /text/analytics/v3.1/languages ✅: `This is correct because this endpoint is used for detecting the language of the input text.`
- [ ] /translator/text/v3.0/translate?to=en ❌: `This is incorrect because this endpoint is used for translating text to English, not for detecting the language.`
- [ ] /translator/text/v3.0/translate?to=fr ❌: `This is incorrect because this endpoint is used for translating text to French, not for detecting the language.`

## Q: Configuring IP Firewall Rules for Azure AI Search

> You create a web app named `app1` that runs on an Azure virtual machine named `vm1`. `vm1` is on an Azure virtual network named `vnet1`. You plan to create a new Azure AI Search service named `service1`. You need to ensure that `app1` can connect directly to `service1` without routing traffic over the public internet. Which solution should you implement?

**Options:**

- [ ] Deploy `service1` with a private endpoint in `vnet1` and configure Azure Private Link. ✅: `This is correct because deploying `service1` with a private endpoint in the same virtual network and configuring Azure Private Link ensures that traffic between `app1` and `service1` does not traverse the public internet.`
- [ ] Deploy `service1` with a public endpoint and configure an IP firewall rule. ❌: `This is incorrect because using a public endpoint and IP firewall rule does not prevent traffic from traversing the public internet.`
- [ ] Deploy `service1` with a public endpoint and configure a VPN connection between `vnet1` and the public endpoint. ❌: `This is incorrect because using a public endpoint and VPN connection does not prevent traffic from traversing the public internet.`
- [ ] Deploy `service1` with a private endpoint in a different virtual network and configure Azure Private Link. ❌: `This is incorrect because deploying `service1` in a different virtual network would require additional configuration and does not ensure direct connectivity without traversing the public internet.`

## Q: Converting Speech to Text for Streaming MP3 Data

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

## Q: Developing an Automated Call Handling System

> You need to develop an automated call handling system that can respond to callers in their own language. The system will support only French and English. Which Azure AI Services service should you use to meet each requirement? 

**Answer:**

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

## Q: Extracting Data from Receipts Using Form Recognizer

> You have receipts that are accessible from a URL. You need to extract data from the receipts by using Form Recognizer and the SDK. The solution must use a prebuilt model. Which client and method should you use?

**Options:**

- [ ] the FormRecognizerClient client and the StartRecognizeContentFromUri method ❌: `This is incorrect because the StartRecognizeContentFromUri method is used for recognizing content in general documents, not specifically for receipts.`
- [ ] the FormTrainingClient client and the StartRecognizeContentFromUri method ❌: `This is incorrect because the FormTrainingClient is used for training custom models, not for using prebuilt models.`
- [ ] the FormTrainingClient client and the StartRecognizeReceiptsFromUri method ❌: `This is incorrect because the FormTrainingClient is used for training custom models, not for using prebuilt models.`
- [ ] the FormRecognizerClient client and the StartRecognizeReceiptsFromUri method ✅: `This is correct because the FormRecognizerClient client and the StartRecognizeReceiptsFromUri method are used to extract data from receipts using the prebuilt receipt model.`

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

## Q: Reducing Throttling in Azure AI Search

> You have an Azure AI Search service. During the past 12 months, query volume steadily increased. You discover that some search query requests to the AI Search service are being throttled. You need to reduce the likelihood that search query requests are throttled. **Solution: You add indexes.** Does this meet the goal?

**Options:**

- [ ] Yes ❌: `This is incorrect because adding indexes does not directly address the issue of throttling caused by high query volume. Throttling is typically related to service capacity, not the number of indexes.`
- [ ] No ✅: `This is correct because adding indexes does not reduce throttling. To reduce throttling, you should consider increasing the service tier, adding more replicas, or optimizing query performance.`

## Q: Analyzing Extracted Information from Purchase Orders Using Power BI

> You have an Azure AI Search instance that indexes purchase orders by using Form Recognizer. You need to analyze the extracted information by using Microsoft Power BI. The solution must minimize development effort. What should you add to the indexer?

**Options:**

- [ ] a projection group ❌: `This is incorrect because a projection group is not specifically used for integrating with Power BI.`
- [ ] a file projection ❌: `This is incorrect because a file projection is used for handling file data, not for structuring data for Power BI analysis.`
- [ ] an object projection ❌: `This is incorrect because an object projection is used for handling complex objects, not for structuring data for Power BI analysis.`
- [ ] a table projection ✅: `This is correct because a table projection organizes the extracted data into a tabular format, which can be easily consumed by Power BI for analysis.`

## Q: Building a Monitoring Solution for PPE Compliance

> You have a factory that produces food products. You need to build a monitoring solution for staff compliance with personal protective equipment (PPE) requirements. The solution must meet the following requirements:  <br/>
> - Identify staff who have removed masks or safety glasses.  <br/>
> - Perform a compliance check every 15 minutes.  <br/>
> - Minimize development effort.  <br/>
> - Minimize costs. <br/>
> Which service should you use?

**Options:**

- [ ] Face ❌: `This is incorrect because while the Face service can detect and analyze facial features, including the presence of objects like masks and safety glasses, it is primarily used for facial recognition and verification. It may not be the most efficient solution for frequent compliance checks in a video stream.`
- [ ] Computer Vision ❌: `This is incorrect because while Computer Vision can analyze images, it may not be the most efficient solution for frequent compliance checks in a video stream.`
- [ ] Azure Video Analyzer for Media (formerly Video Indexer) ✅: `This is correct because Azure Video Analyzer for Media is designed to analyze video content and can be used to identify specific scenarios, such as whether individuals in a video are wearing masks or safety glasses. It supports a range of video analytics capabilities, including object detection, which can be leveraged to monitor PPE compliance. Using Azure Video Analyzer for Media can minimize development effort by providing built-in models for analyzing video content and can be set up to perform compliance checks at specified intervals, such as every 15 minutes.`

## Q: Building an App for Anomaly Detection and Incident Alerts

> You have an Azure IoT hub that receives sensor data from machinery. You need to build an app that will perform the following actions: <br/>
> - Perform anomaly detection across multiple correlated sensors. <br/>
> - Identify the root cause of process stops. <br/>
> - Send incident alerts. <br/>
> - The solution must minimize development time. <br/>
> Which Azure service should you use?

**Options:**

- [ ] Azure Metrics Advisor ❌: `This is incorrect because Azure Metrics Advisor is primarily used for monitoring and diagnosing anomalies in time series data, but it may not be the best choice for identifying root causes and sending incident alerts.`
- [ ] Form Recognizer ❌: `This is incorrect because Form Recognizer is used for extracting text and data from forms and documents, not for anomaly detection or incident alerts.`
- [ ] Azure Machine Learning ❌: `This is incorrect because while Azure Machine Learning can be used for anomaly detection and root cause analysis, it requires more development effort compared to a specialized service like Anomaly Detector.`
- [ ] Anomaly Detector ✅: `This is correct because Anomaly Detector is designed to perform anomaly detection across multiple correlated sensors, identify the root cause of anomalies, and can be integrated with other services to send incident alerts. It minimizes development time by providing built-in models and APIs for anomaly detection.`


<div align="center">
  <h3 style="color: #4CAF50;">Total Visitors</h3>
  <img src="https://profile-counter.glitch.me/brown9804/count.svg" alt="Visitor Count" style="border: 2px solid #4CAF50; border-radius: 5px; padding: 5px;"/>
</div>
