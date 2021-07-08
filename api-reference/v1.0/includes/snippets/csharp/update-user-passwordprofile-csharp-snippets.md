---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b6c9d0207a7acbccd51ebd672305905728a0d534
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316517"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = new User
{
    PasswordProfile = new PasswordProfile
    {
        ForceChangePasswordNextSignIn = false,
        Password = "xWwvJ]6NMw+bWH-d"
    }
};

await graphClient.Users["{user-id}"]
    .Request()
    .UpdateAsync(user);

```