---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c20bbcba66fbaf04f18f333a8720c6a556f809b
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096167"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ediscoveryCase = await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"]
    .Request()
    .GetAsync();

```