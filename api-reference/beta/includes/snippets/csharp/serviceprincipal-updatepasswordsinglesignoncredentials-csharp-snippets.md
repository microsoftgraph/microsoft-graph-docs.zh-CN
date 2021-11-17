---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d02c4c719cc01aa12655b031f577235761c24679d415c4d9f6b512ab01593873
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163778"
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
    .UpdatePasswordSingleSignOnCredentials(id,credentials)
    .Request()
    .PostAsync();

```