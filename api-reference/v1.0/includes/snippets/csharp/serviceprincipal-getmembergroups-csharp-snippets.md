---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d1ddeb04b6093d705d5229872783b0e852a9edd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788381"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = true;

await graphClient.ServicePrincipals["{servicePrincipal-id}"]
    .GetMemberGroups(securityEnabledOnly)
    .Request()
    .PostAsync();

```