---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d032b0ba316c57697b837ef40094ad4b7db72c4d474fd915030470fd9040f0a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902451"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = new User
{
    DisplayName = "John Smith",
    Identities = new List<ObjectIdentity>()
    {
        new ObjectIdentity
        {
            SignInType = "userName",
            Issuer = "contoso.onmicrosoft.com",
            IssuerAssignedId = "johnsmith"
        },
        new ObjectIdentity
        {
            SignInType = "emailAddress",
            Issuer = "contoso.onmicrosoft.com",
            IssuerAssignedId = "jsmith@yahoo.com"
        },
        new ObjectIdentity
        {
            SignInType = "federated",
            Issuer = "facebook.com",
            IssuerAssignedId = "5eecb0cd"
        }
    },
    PasswordProfile = new PasswordProfile
    {
        Password = "password-value",
        ForceChangePasswordNextSignIn = false
    },
    PasswordPolicies = "DisablePasswordExpiration"
};

await graphClient.Users
    .Request()
    .AddAsync(user);

```