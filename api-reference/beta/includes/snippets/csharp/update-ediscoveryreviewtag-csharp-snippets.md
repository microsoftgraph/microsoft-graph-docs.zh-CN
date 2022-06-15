---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: acfc6dc2a7af9e47f7b53c8f25f3d9fb5bc203e8
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093695"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ediscoveryReviewTag = new Microsoft.Graph.Security.EdiscoveryReviewTag
{
    DisplayName = "My tag API 2",
    Description = "Use Graph API to create tags (updated)"
};

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Tags["{security.ediscoveryReviewTag-id}"]
    .Request()
    .UpdateAsync(ediscoveryReviewTag);

```