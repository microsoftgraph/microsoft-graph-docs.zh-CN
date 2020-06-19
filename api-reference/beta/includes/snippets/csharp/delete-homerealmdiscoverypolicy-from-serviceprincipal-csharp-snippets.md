---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f91e98dc8665064aee5ffce925192f3e2cfdcf60
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44794489"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{servicePrincipalId}"].HomeRealmDiscoveryPolicies["{policyId}"].Reference
    .Request()
    .DeleteAsync();

```