---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b61603649a9cff237767e94ca2f25c14b7a4df4f42604070a2e113acec5f70f5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215775"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var claimsMappingPolicies = await graphClient.ServicePrincipals["{servicePrincipal-id}"].ClaimsMappingPolicies
    .Request()
    .GetAsync();

```