---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 60b4207cb5c830cc3202d14432a909e726852cf4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803899"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignedTo = await graphClient.ServicePrincipals["{servicePrincipal-id}"].AppRoleAssignedTo
    .Request()
    .GetAsync();

```