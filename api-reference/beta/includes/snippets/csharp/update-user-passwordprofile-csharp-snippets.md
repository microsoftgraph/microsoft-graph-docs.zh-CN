---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9477b084c142e3bd2db2a455212da299545530f7b0039d1869bff60394bbc7cb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333374"
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