---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2adbaad4372904f88b57772ab1ffb71b8adfbc06
ms.sourcegitcommit: d09d720b56ed6f1fad556e2a3730c2e850db355f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/02/2020
ms.locfileid: "49556156"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = new User
{
    AccountEnabled = true,
    DisplayName = "Adele Vance",
    MailNickname = "AdeleV",
    UserPrincipalName = "AdeleV@contoso.onmicrosoft.com",
    PasswordProfile = new PasswordProfile
    {
        ForceChangePasswordNextSignIn = true,
        Password = "xWwvJ]6NMw+bWH-d"
    }
};

await graphClient.Users
    .Request()
    .AddAsync(user);

```