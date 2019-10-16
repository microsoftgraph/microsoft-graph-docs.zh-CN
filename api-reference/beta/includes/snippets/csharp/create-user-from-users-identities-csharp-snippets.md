---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 66487d83b5ff08c6d394383448310eb131852af7
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538422"
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
            SignInType = "federated",
            Issuer = "facebook.com",
            IssuerAssignedId = "5eecb0cd"
        }
    },
    PasswordProfile = new PasswordProfile
    {
        ForceChangePasswordNextSignIn = true,
        Password = "password-value"
    }
};

await graphClient.Users
    .Request()
    .AddAsync(user);

```