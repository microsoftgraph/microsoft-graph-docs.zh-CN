---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e3b93521c9bf80f807e90f8cd2abf91fe2dd5c2f
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092136"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tags = await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Tags
    .Request()
    .GetAsync();

```