---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c03162e84f7f46e6ec304ab856c555246692566a
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094736"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var additionalSources = await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Searches["{security.ediscoverySearch-id}"].AdditionalSources
    .Request()
    .GetAsync();

```