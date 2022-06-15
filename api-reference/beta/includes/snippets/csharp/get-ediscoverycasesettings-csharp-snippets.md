---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2237f20a327b5f1a5fa775805e15a32a1914af57
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094442"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ediscoveryCaseSettings = await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Settings
    .Request()
    .GetAsync();

```