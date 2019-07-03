---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b5b4312c65a8a42db6c33d9728a1bf84f7e99bc6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479473"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoleSettings = await graphClient.PrivilegedRoles["{id}"].Settings
    .Request()
    .GetAsync();

```