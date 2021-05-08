---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e7ce59c0ef27ca64b23d6bdc8261a894330977c
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240829"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var settings = new Microsoft.Graph.Ediscovery.Settings
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
    .UpdateAsync(settings);

```