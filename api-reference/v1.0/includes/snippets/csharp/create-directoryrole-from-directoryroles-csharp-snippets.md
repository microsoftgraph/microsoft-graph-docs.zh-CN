---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb0da9b4fa704250345d8d3466028c8c65448a35
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "53005907"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryRole = new DirectoryRole
{
    RoleTemplateId = "fe930be7-5e62-47db-91af-98c3a49a38b1"
};

await graphClient.DirectoryRoles
    .Request()
    .AddAsync(directoryRole);

```