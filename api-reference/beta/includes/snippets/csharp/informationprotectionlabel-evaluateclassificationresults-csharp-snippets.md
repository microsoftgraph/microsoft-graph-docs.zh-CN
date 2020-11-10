---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 11af8f23109b05e6396eeb187ab9bb067f7e2a85
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952918"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contentInfo = new ContentInfo
{
    Format = ContentFormat.Default,
    Identifier = null,
    State = ContentState.Rest,
    AdditionalData = new Dictionary<string, object>()
    {
        {"format@odata.type", "#microsoft.graph.contentFormat"},
        {"state@odata.type", "#microsoft.graph.contentState"}
    }
};

var classificationResults = new List<ClassificationResult>()
{
    new ClassificationResult
    {
        SensitiveTypeId = Guid.Parse("cb353f78-2b72-4c3c-8827-92ebe4f69fdf"),
        Count = 4,
        ConfidenceLevel = 75
    }
};

await graphClient.InformationProtection.Policy.Labels
    .EvaluateClassificationResults(contentInfo,classificationResults)
    .Request()
    .Header("User-Agent","ContosoLOBApp/1.0")
    .PostAsync();

```