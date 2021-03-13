---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b10fb5e14a3c3ac9a9a435317a08f71b5c5f4cf
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805061"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var transitiveMemberOf = await graphClient.ServicePrincipals["{servicePrincipal-id}"].TransitiveMemberOf
    .Request()
    .GetAsync();

```