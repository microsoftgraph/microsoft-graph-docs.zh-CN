---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 042749413cf168bb9a58260db84b819c1ae6aa7c
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095702"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userSources = await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Custodians["{security.ediscoveryCustodian-id}"].UserSources
    .Request()
    .GetAsync();

```