---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6225dc4d9447f34457d73f5a4744c5069676c807
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942164"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tiIndicator = new TiIndicator
{
    AdditionalInformation = "additionalInformation-after-update",
    Confidence = 42,
    Description = "description-after-update"
};

await graphClient.Security.TiIndicators["{tiIndicator-id}"]
    .Request()
    .Header("Prefer","return=representation")
    .UpdateAsync(tiIndicator);

```