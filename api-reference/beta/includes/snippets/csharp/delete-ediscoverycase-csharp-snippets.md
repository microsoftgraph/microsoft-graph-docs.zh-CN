---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a689c0ba4f5b5ba653ae1c94642e6c49899b1cff
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095982"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"]
    .Request()
    .DeleteAsync();

```