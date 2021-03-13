---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 923846079c499091cadda49f77398701f2137dcc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776184"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignments = await graphClient.Users["{user-id}"].AppRoleAssignments
    .Request()
    .Filter("resourceId eq 8e881353-1735-45af-af21-ee1344582a4d")
    .GetAsync();

```