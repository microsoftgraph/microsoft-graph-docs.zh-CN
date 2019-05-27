---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e6aa7ae895baade00992d77d1abe0efb7721deb4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447255"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoleSummary = await graphClient.PrivilegedRoles["{id}"].Summary
    .Request()
    .GetAsync();

```