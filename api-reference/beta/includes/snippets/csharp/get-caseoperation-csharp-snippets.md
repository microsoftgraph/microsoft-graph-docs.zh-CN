---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a71ff4efe68acf2651a61470d0b7432a9a050e7
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096094"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var caseOperation = await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Operations["{security.caseOperation-id}"]
    .Request()
    .GetAsync();

```