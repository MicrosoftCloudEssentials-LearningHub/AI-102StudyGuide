# Computer Vision & Natural Languange Processing: Sample Questions and Answers 

Costa Rica

[![GitHub](https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff)](https://github.com/)
[brown9804](https://github.com/brown9804)

Last updated: 2025-01-16

----------

> [!NOTE]
> The questions and answers provided in this study guide are for practice purposes only and are not official practice questions.
> They are intended to help you prepare for the [AI-102 Microsoft certification exam](https://learn.microsoft.com/en-us/credentials/certifications/azure-ai-engineer/?practice-assessment-type=certification).
> For additional preparation materials and the most up-to-date information, please refer to the [official Microsoft documentation](https://learn.microsoft.com/en-us/credentials/certifications/azure-ai-engineer/?practice-assessment-type=certification#certification-prepare-for-the-exam).

> - Implement computer vision solutions <br/> 
> - Implement natural language processing solutions

<details>
<summary><b>List of References </b> (Click to expand)</summary>

- [Microsoft Certified: Azure AI Engineer Associate](https://learn.microsoft.com/en-us/credentials/certifications/azure-ai-fundamentals/) - Overview of the AI-102 certification, including skills measured and exam details.
- [Study Guide for Exam AI-102: Designing and Implementing an Azure AI Solution](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/ai-900) - Detailed study guide with topics covered in the exam and links to additional resources.
- [Course AI-102T00-A: Designing and Implementing an Azure AI Solution](https://learn.microsoft.com/en-us/training/courses/ai-900t00) - Training course that covers designing and implementing AI solutions using Azure AI services.

</details>

<details>
<summary><b>List of questions/answers </b> (Click to expand)</summary>

</details>

## Q: Training a Custom Form Recognizer Model

> You build a custom Form Recognizer model. You receive sample files to use for training the model as shown in the following table.

| Name  | Type | Size  |
|-------|------|-------|
| File1 | PDF  | 30 MB |
| File2 | MP4  | 150 MB|
| File3 | JPG  | 40 MB |
| File4 | PDF  | 170 MB|
| File5 | GIF  | 15 MB |
| File6 | JPG  | 30 MB |

> Which three files can you use to train the model? Each correct answer presents a complete solution.

**Options:**

- [ ]  File1 ✅: `This is correct because it is a PDF file within the size limit for training, which is 50 MB for PDF files.`
- [ ] File2 ❌: `This is incorrect because MP4 files are not supported for training a Form Recognizer model`
- [ ]  File3 ✅: `This is correct because it is a JPG file within the size limit for training, which is 50 MB for image files.`
- [ ] File4 ❌: `This is incorrect because it is a PDF file that exceeds the size limit for training, which is 50 MB for PDF files.`
- [ ] File5 ❌: `This is incorrect because GIF files are not supported for training a Form Recognizer model`
- [ ]  File6 ✅: `This is correct because it is a JPG file within the size limit for training, which is 50 MB for image files.`

## Q: Regenerating an API Key

> You successfully run the following HTTP request.

```http
POST https://management.azure.com/subscriptions/18e51a87-3a69-47a8-aedc-a5474517f08a/resourceGroups/RGI/providers/Microsoft.CognitiveServices/accounts/conosci1/regenerateKey?api-version=2017-04-18

Body {"keyName": "Key2"}
```

> What is the result of the request?

**Options:**

- [ ] `A new query key was generated.` ❌: `This is incorrect because the request regenerates a subscription key, not a query key.`
- [ ] `A key for Azure Cognitive Services was generated in Azure Key Vault.` ❌: `This is incorrect because the request regenerates a key for the Cognitive Services account, not in Azure Key Vault.`
- [ ] `The primary subscription key and the secondary subscription key were rotated.` ❌: `This is incorrect because the request regenerates only one key, not both.`
- [ ]  `The secondary subscription key was reset.` ✅: `This is correct because the request regenerates the secondary subscription key specified by "Key2".`

## Q: Creating a Text Analytics Resource

> You have the following C# method for creating Azure Cognitive Services resources programmatically.

```csharp
static void create_resource(CognitiveServicesManagementClient client, string resource_name, string kind, string account_tier, string location) 
{
    CognitiveServicesAccount parameters = new CognitiveServicesAccount(null, null, kind, location, resource_name,
        new CognitiveServicesAccountProperties(), new Sku(account_tier));
    client.CognitiveServicesAccounts.create(resource_group_name, account_tier,
        parameters);
}
```

> You need to call the method to create a Text Analytics resource in the West US Azure region. The resource will be used for sentiment analysis. Which choice should you make?

**Options:**

- [ ]  `create_resource(client, "test", "TextAnalytics", "S0", "westus")` ✅: `This is correct because it specifies the Text Analytics resource kind, which is used for sentiment analysis.`
- [ ] `create_resource(client, "test", "ComputerVision", "F0", "westus")` ❌: `This is incorrect because it specifies the Computer Vision resource kind, not the Text Analytics resource kind.`
- [ ] `create_resource(client, "test", "CustomVision.Training", "S0", "westus")` ❌: `This is incorrect because it specifies the Custom Vision Training resource kind, not the Text Analytics resource kind.`
- [ ] `create_resource(client, "test", "CustomVision.Prediction", "S0", "westus")` ❌: `This is incorrect because it specifies the Custom Vision Prediction resource kind, not the Text Analytics resource kind.`

## Q: Deploying Text Analytics API Container

> You plan to deploy a containerized version of an Azure Cognitive Services service that will be used for text analysis. You configure `https://contoso.cognitiveservices.azure.com` as the endpoint URL for the service, and you pull the latest version of the Text Analytics API container image. You need to run the container on an Azure virtual machine by using Docker. You configure the command to `/text/answer`, select the appropriate options in the answer area.

```bash
docker run --rm -it -p 5000:5000 --memory 8g --cpus 1 \
__________________________ \
-e Eula=accept \
-e Billing=________________ \
-e ApiKey=xxxxxxxxxxxxxxxxxxxxxx
```

**Options for the Container Image:**

- [ ] mcr.microsoft.com/azure-cognitive-services/textanalytics/keyphrase ❌: `This is incorrect because it specifies the container image for the keyphrase extraction feature, not the sentiment analysis feature.`
- [ ]  mcr.microsoft.com/azure-cognitive-services/textanalytics/sentiment ✅: `This is correct because it specifies the container image for the sentiment analysis feature.`

**Options for Billing:**

- [ ] http://contoso.blob.core.windows.net ❌: `This is incorrect because it specifies a general Azure Blob Storage endpoint, not the specific billing endpoint for the service.`
- [ ]  https://contoso.cognitiveservices.azure.com ✅: `This is correct because it specifies the endpoint URL for the Cognitive Services, which can be used as the billing endpoint.`

## Q: Updating a Computer Vision Resource

> Your company has an existing Azure Computer Vision resource that needs to be updated to include a new feature for analyzing handwritten text. The solution must:
> - Apply partial updates to the existing resource. <br/> 
> - Ensure the resource remains in the same region.  <br/> 
> - Use the appropriate HTTP method for partial updates.  <br/> 
> How should you complete the HTTP request to update the resource? Select the appropriate options in the answer area.

```http
__________ https://management.azure.com/subscriptions/xxxxxxxx-xxxx-xxxx-xxxx/resourceGroups/RG3/providers/Microsoft.CognitiveServices/accounts/CV1?api-version=2017-04-18

{
  "properties": {
    "features": [
      "__________"
    ]
  }
}
```

**Options:**

- [ ] POST ❌: `This is incorrect because POST is typically used to create a new resource without specifying the resource identifier.`
- [ ] PUT ❌: `This is incorrect because PUT is used to create or update a resource at a specified URI, ensuring idempotency.`
- [ ] CognitiveServices ❌: `This is incorrect because it specifies the general Azure Cognitive Services resource, rather than the specific Computer Vision service.`
- [ ] TextAnalytics ❌: `This is incorrect because it specifies a different service within Azure Cognitive Services, not related to computer vision.`
- [ ]  PATCH ✅: `This is correct because PATCH is used to apply partial updates to an existing resource.`
- [ ]  ComputerVision ✅: `This is correct because it specifies the specific Azure Cognitive Services resource for computer vision tasks.`

```http
PATCH https://management.azure.com/subscriptions/xxxxxxxx-xxxx-xxxx-xxxx/resourceGroups/RG3/providers/Microsoft.CognitiveServices/accounts/CV1?api-version=2017-04-18

{
  "properties": {
    "features": [
      "ComputerVision"
    ]
  }
}
```
## Q: Language Understanding Model

> You've got 4659 chatbots, each with its own Language Understanding model.
> Often, you need to add the same phrases to all the models.
> You need to update the Language Understanding models programmatically to include these phrases.
> How should you complete the code? 
 
```csharp
var result = await client.Features.<value>(
    appId, versionId, new <value>
    {
        EnabledForAllModels = false,
        IsExchangeable = true,
        Name = "PL1",
        Phrases = "item1,item2,item3,item4,item5"
    });
```

Pick the right values for the correct targets. Each value may be used once, more than once, or not at all.

- [ ] **Phraselist** ❌: `This is incorrect because it is not an action. Represents a collection of phrases used in a language understanding model.`
- [ ] **Phrases** ❌: `This is incorrect because it refers to the content, not an action or method. The actual phrases included in the phrase list.`
- [ ] **SavePhraselistAsync** ❌: `This is incorrect because it is not relevant to the code snippet. Saves the phrase list asynchronously to the language understanding model.`
- [ ] **UploadPhraseListAsync** ❌: `This is incorrect because it is not relevant to the code snippet. Uploads a phrase list asynchronously to the language understanding model.`
- [ ]  **PhraseListCreateObject** ✅: `This is correct because it represents an object for creating a phrase list.`
- [ ]  **AddPhraseListAsync** ✅: `This is correct because it adds a phrase list asynchronously.`

Answer:

```csharp
var result = await client.Features.AddPhraseListAsync(
    appId, versionId, new PhraseListCreateObject 
    {
        EnabledForAllModels = false,
        IsExchangeable = true,
        Name = "PL1",
        Phrases = "item1,item2,item3,item4,item5"
    });
```

## Q: Building a Multilingual Chatbot with Sentiment Analysis

> You are tasked with building a chatbot that must: <br/>
> - Handle chit-chat, knowledge base queries, and support multiple languages <br/> 
> - Analyze user messages to determine their emotional tone (sentiment analysis) <br/>
> - Automatically choose the most appropriate language model <br/>
> Which services should you integrate into the chatbot?

**Options:**
- [ ] **Translator, Speech, and Dispatch** ❌: `This is incorrect because it does not include chit-chat or knowledge base support.`
- [ ] **QnA Maker, Language Understanding, and Dispatch** ❌: `This is incorrect because it does not include sentiment analysis.` 
- [ ] **Text Analytics, Translator, and Dispatch** ❌: `This is incorrect because it does not include chit-chat or knowledge base support.`
- [ ]  **Language Understanding, Text Analytics, and QnA Maker** ✅: `This is correct because it supports chit-chat, knowledge base, multilingual models, and performs sentiment analysis.`

<div align="center">
  <h3 style="color: #4CAF50;">Total Visitors</h3>
  <img src="https://profile-counter.glitch.me/brown9804/count.svg" alt="Visitor Count" style="border: 2px solid #4CAF50; border-radius: 5px; padding: 5px;"/>
</div>

