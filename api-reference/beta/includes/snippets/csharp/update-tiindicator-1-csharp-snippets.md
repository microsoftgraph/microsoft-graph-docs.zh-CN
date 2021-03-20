---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 860f76bf13651cf49018f8d239613b1dd72f8f7d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942167"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tiIndicator = new TiIndicator
{
    Description = "description-updated"
};

await graphClient.Security.TiIndicators["{tiIndicator-id}"]
    .Request()
    .UpdateAsync(tiIndicator);

```