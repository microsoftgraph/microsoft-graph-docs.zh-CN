---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3174772c6bb355843808cb15c109d4158af3ee42
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093097"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ediscoverySearch = await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Searches["{security.ediscoverySearch-id}"]
    .Request()
    .GetAsync();

```