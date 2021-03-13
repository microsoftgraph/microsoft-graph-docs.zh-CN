---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f41be5c09c950372795905f9e5dcc72d043983e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779914"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var memberOf = await graphClient.ServicePrincipals["{servicePrincipal-id}"].MemberOf
    .Request()
    .GetAsync();

```