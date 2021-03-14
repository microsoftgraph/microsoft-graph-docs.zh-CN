---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24ae6c229de82aa9479e6e93660e779dd415037f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792545"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var oauth2PermissionGrants = await graphClient.ServicePrincipals["{servicePrincipal-id}"].Oauth2PermissionGrants
    .Request()
    .GetAsync();

```