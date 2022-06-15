---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b7816d83731466337c122a838be2468fc605882
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095394"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Searches["{security.ediscoverySearch-id}"]
    .PurgeData()
    .Request()
    .PostAsync();

```