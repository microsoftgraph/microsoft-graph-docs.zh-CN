---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b61d190dec63c0c63a81fe3070d9710f36ea71a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790053"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{servicePrincipal-id}"].ClaimsMappingPolicies["{claimsMappingPolicy-id}"].Reference
    .Request()
    .DeleteAsync();

```