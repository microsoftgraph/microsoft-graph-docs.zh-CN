---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 53e8e5d3e131f2cadcc9596056170a5c0fd6bf38
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093601"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var files = await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].ReviewSets["{security.ediscoveryReviewSet-id}"].Files
    .Request()
    .Top(5)
    .GetAsync();

```