---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9687732e8ece5b298e7223f8856111e0b9ecfc3c
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093806"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reviewSets = await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].ReviewSets
    .Request()
    .GetAsync();

```