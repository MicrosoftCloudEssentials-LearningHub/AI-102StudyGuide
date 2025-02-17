# Computer Vision & Natural Languange Processing: Sample Questions and Answers 

Costa Rica

[![GitHub](https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff)](https://github.com/)
[brown9804](https://github.com/brown9804)

Last updated: 2025-01-16

----------

> Implement computer vision solutions
> Implement natural language processing solutions

> [!NOTE]
> The questions and answers provided in this study guide are for practice purposes only and are not official practice questions.
> They are intended to help you prepare for the [AI-102 Microsoft certification exam](https://learn.microsoft.com/en-us/credentials/certifications/azure-ai-engineer/?practice-assessment-type=certification).
> For additional preparation materials and the most up-to-date information, please refer to the [official Microsoft documentation](https://learn.microsoft.com/en-us/credentials/certifications/azure-ai-engineer/?practice-assessment-type=certification#certification-prepare-for-the-exam).

<details>
<summary><b>List of References </b> (Click to expand)</summary>

- [Microsoft Certified: Azure AI Engineer Associate](https://learn.microsoft.com/en-us/credentials/certifications/azure-ai-fundamentals/) - Overview of the AI-102 certification, including skills measured and exam details.
- [Study Guide for Exam AI-102: Designing and Implementing an Azure AI Solution](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/ai-900) - Detailed study guide with topics covered in the exam and links to additional resources.
- [Course AI-102T00-A: Designing and Implementing an Azure AI Solution](https://learn.microsoft.com/en-us/training/courses/ai-900t00) - Training course that covers designing and implementing AI solutions using Azure AI services.

</details>

<details>
<summary><b>List of questions/answers </b> (Click to expand)</summary>

</details>

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
- [X] **PhraseListCreateObject** ✅: `This is correct because it represents an object for creating a phrase list.`
- [X] **AddPhraseListAsync** ✅: `This is correct because it adds a phrase list asynchronously.`

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
- [ ] **A. QnA Maker, Language Understanding, and Dispatch** ❌: `This is incorrect because it does not include sentiment analysis.` 
- [ ] **B. Translator, Speech, and Dispatch** ❌: `This is incorrect because it does not include chit-chat or knowledge base support.`
- [X] **C. Language Understanding, Text Analytics, and QnA Maker** ✅: `This is correct because it supports chit-chat, knowledge base, multilingual models, and performs sentiment analysis.`
- [ ] **D. Text Analytics, Translator, and Dispatch** ❌: `This is incorrect because it does not include chit-chat or knowledge base support.`

<div align="center">
  <h3 style="color: #4CAF50;">Total Visitors</h3>
  <img src="https://profile-counter.glitch.me/brown9804/count.svg" alt="Visitor Count" style="border: 2px solid #4CAF50; border-radius: 5px; padding: 5px;"/>
</div>

