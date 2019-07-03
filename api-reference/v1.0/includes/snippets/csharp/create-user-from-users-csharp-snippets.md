---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 776789492f83c5898520cc7c1e4ac9f20838f3c2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35510147"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = new User
{
    AccountEnabled = true,
    DisplayName = "displayName-value",
    MailNickname = "mailNickname-value",
    UserPrincipalName = "upn-value@tenant-value.onmicrosoft.com",
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