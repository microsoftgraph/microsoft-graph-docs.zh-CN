---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7731eb062019c01b32d91ee3efe93781ffcc2b6
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092931"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"]
    .Reopen()
    .Request()
    .PostAsync();

```