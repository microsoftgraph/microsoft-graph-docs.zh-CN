---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bed8f5319bc136ec577941491a2284c0c6425efd91cced0560c39ec3d1bc5669
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334078"
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