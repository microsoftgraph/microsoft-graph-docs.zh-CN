---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24186dcba90b691a64a941e87529745ae13c7490
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095219"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Custodians["{security.ediscoveryCustodian-id}"]
    .UpdateIndex()
    .Request()
    .PostAsync();

```