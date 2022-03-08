---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26890bd8af41a5af71fe0c7ad2cea1b535b28a95
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63351201"
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
        SensitiveTypeId = "cb353f78-2b72-4c3c-8827-92ebe4f69fdf",
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