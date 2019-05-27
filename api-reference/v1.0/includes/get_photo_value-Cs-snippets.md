---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fcde4b8ff38a06313b1e8adfe9ac0c199bb1d416
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34451298"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var Stream = await graphClient.Users["{id|userPrincipalName}"].Photo.Content
    .Request()
    .GetAsync();

```