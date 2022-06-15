---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d4c398ecfcfdcb0e718af66699cdaab2cb3024a
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093993"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Searches["{security.ediscoverySearch-id}"]
    .Estimatestatistics()
    .Request()
    .PostAsync();

```