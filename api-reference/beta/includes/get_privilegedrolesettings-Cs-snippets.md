---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b5b4312c65a8a42db6c33d9728a1bf84f7e99bc6
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447276"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoleSettings = await graphClient.PrivilegedRoles["{id}"].Settings
    .Request()
    .GetAsync();

```