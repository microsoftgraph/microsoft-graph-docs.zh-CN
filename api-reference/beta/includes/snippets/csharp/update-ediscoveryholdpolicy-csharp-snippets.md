---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6309c4915fbfdf6fad177602da06b486304b0c4d
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093926"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ediscoveryHoldPolicy = new Microsoft.Graph.Security.EdiscoveryHoldPolicy
{
    Description = "updated description",
    ContentQuery = "bazooka bazooka"
};

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].LegalHolds["{security.ediscoveryHoldPolicy-id}"]
    .Request()
    .UpdateAsync(ediscoveryHoldPolicy);

```