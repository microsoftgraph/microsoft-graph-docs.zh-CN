---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31dfb9ae32f02d5e4c8808498ab4c293858eafa3
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093001"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ediscoveryFile = await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].ReviewSets["{security.ediscoveryReviewSet-id}"].Files["{security.ediscoveryFile-id}"]
    .Request()
    .GetAsync();

```