---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 55ed45972aefd5b7f774568aac111905f6b8e7e9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791775"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var passwordCredential = new PasswordCredential
{
    DisplayName = "Password friendly name"
};

await graphClient.ServicePrincipals["{servicePrincipal-id}"]
    .AddPassword(passwordCredential)
    .Request()
    .PostAsync();

```