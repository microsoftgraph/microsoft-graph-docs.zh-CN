---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a5b8382f5b51fe26bfc79c6b2da4d3e77ad8faf
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/20/2019
ms.locfileid: "38747806"
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

await graphClient.ServicePrincipals["{id}"]
    .UpdatePasswordSingleSignOnCredentials(id,credentials)
    .Request()
    .PostAsync();

```