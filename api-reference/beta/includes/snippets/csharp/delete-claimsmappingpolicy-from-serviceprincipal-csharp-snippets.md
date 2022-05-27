---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d9cf2d79d8641f2421e9676108b3536a35c90a7dc2831c4ee23aa1dda8117eb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903306"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{servicePrincipal-id}"].ClaimsMappingPolicies["{claimsMappingPolicy-id}"].Reference
    .Request()
    .DeleteAsync();

```