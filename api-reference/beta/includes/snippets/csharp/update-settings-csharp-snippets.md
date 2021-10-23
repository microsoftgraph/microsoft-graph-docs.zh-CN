---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca25aacb1bf4d0d6418e7fd86905bd68d6a35d3c
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60559717"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var caseSettings = new Microsoft.Graph.Ediscovery.CaseSettings
{
    RedundancyDetection = new Microsoft.Graph.Ediscovery.RedundancyDetectionSettings
    {
        IsEnabled = false,
        SimilarityThreshold = 70,
        MinWords = 12,
        MaxWords = 400000
    },
    TopicModeling = new Microsoft.Graph.Ediscovery.TopicModelingSettings
    {
        IsEnabled = false,
        IgnoreNumbers = false,
        TopicCount = 50,
        DynamicallyAdjustTopicCount = false
    },
    Ocr = new Microsoft.Graph.Ediscovery.OcrSettings
    {
        IsEnabled = true,
        MaxImageSize = 12000
    }
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Settings
    .Request()
    .UpdateAsync(caseSettings);

```