---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6292fcf20ba6f4142da69c8970a1a07eb8a37fb8
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334749"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var servicePrincipalIds = new List<String>()
{
    "9089a539-a539-9089-39a5-899039a58990"
};

await graphClient.IdentityProtection.RiskyServicePrincipals
    .ConfirmCompromised(servicePrincipalIds)
    .Request()
    .PostAsync();

```