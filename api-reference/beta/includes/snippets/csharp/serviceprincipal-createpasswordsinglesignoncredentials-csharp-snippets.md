---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0689efce420ef640b3e1597b610d1c2a3601592
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786725"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var id = "5793aa3b-cca9-4794-679a240f8b58";

var credentials = new List<Credential>()
{
    new Credential
    {
        FieldId = "param_username",
        Value = "myusername",
        Type = "username"
    },
    new Credential
    {
        FieldId = "param_password",
        Value = "pa$$w0rd",
        Type = "password"
    }
};

await graphClient.ServicePrincipals["{servicePrincipal-id}"]
    .CreatePasswordSingleSignOnCredentials(id,credentials)
    .Request()
    .PostAsync();

```