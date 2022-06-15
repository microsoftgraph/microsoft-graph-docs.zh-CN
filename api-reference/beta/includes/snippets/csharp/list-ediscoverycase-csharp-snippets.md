---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a7028ee089f3c48c4fa7d6bfb790cce7d172a6a0
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092493"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ediscoveryCases = await graphClient.Security.Cases.EdiscoveryCases
    .Request()
    .GetAsync();

```