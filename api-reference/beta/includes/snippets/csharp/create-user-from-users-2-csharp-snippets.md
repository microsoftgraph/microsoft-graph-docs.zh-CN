---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d95c0ac686243ea6a8691d1ca4e2b20f4a48f24ab0aebcbebb846d00ea9d94b9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333068"
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