---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce71fc69015c7785f32235dfa27d2bfaca594586
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683744"
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

await graphClient.Informationprotection.Policy.Labels
    .EvaluateClassificationResults(contentInfo,classificationResults)
    .Request()
    .Header("User-Agent","ContosoLOBApp/1.0")
    .PostAsync();

```