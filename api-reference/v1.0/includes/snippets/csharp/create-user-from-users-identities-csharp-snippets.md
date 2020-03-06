---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76326bd35c5f0013596c423a58942a92f8af9792
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41558810"
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
        Password = "password-value"
    },
    PasswordPolicies = "DisablePasswordExpiration"
};

await graphClient.Users
    .Request()
    .AddAsync(user);

```