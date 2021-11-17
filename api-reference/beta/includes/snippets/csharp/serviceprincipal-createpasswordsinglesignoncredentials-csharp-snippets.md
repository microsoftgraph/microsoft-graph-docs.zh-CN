---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c19446477a811940e6d74d363b8b70abdb7d54e06da55cea979d72eeeec108a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220487"
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