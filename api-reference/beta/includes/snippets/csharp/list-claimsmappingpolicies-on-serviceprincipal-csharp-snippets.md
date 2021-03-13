---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d72ca9c9ceb7a1fd81469f05c84ad125f501fa20
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801186"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var claimsMappingPolicies = await graphClient.ServicePrincipals["{servicePrincipal-id}"].ClaimsMappingPolicies
    .Request()
    .GetAsync();

```