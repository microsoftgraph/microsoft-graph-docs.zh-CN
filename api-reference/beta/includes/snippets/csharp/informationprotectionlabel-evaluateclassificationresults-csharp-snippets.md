---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c0f0ecced6bfc3d2f238721952672bb7bbf43722
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41494656"
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
    .Header("User-Agent","ContosoLOBApp/1.0")
    .PostAsync();

```