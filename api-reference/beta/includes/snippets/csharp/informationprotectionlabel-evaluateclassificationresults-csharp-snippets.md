---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20183c448f280994e23997154f6300f5500d6aebc656cd4b5bd3178882898edb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220507"
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