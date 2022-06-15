---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f44af6943d2d892e1c559d5702ec90fbca48a6d
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095440"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queries = await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].ReviewSets["{security.ediscoveryReviewSet-id}"].Queries
    .Request()
    .GetAsync();

```