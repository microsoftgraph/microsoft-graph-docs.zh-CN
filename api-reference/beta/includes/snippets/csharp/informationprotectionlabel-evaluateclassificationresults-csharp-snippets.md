---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7cea47fc1c64717beb8de103613bcd7562fd33e
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37995619"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contentInfo = new ContentInfo
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"state@odata.type","#microsoft.graph.contentState"},
        {"format@odata.type","#microsoft.graph.contentFormat"}
    },
    Format = ContentFormat.Default,
    Identifier = null,
    State = ContentState.Rest
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

await graphClient.Informationprotection.Policy.Labels
    .EvaluateClassificationResults(contentInfo,classificationResults)
    .Request()
    .PostAsync();

```