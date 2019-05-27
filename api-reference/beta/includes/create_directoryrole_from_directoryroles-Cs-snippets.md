---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 88deacf3d76679a76da39083f345dc7e794d7064
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34481042"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryRole = new DirectoryRole
{
    Description = "description-value",
    DisplayName = "displayName-value",
    RoleTemplateId = "roleTemplateId-value"
};

await graphClient.DirectoryRoles
    .Request()
    .AddAsync(directoryRole);

```