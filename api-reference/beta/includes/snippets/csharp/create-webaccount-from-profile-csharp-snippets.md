---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 764582a34b59cf90dc1f8b17bc613e514abfb9be9e1ea76353430ebc2b82ffee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218903"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var webAccount = new WebAccount
{
    Description = "My Github contributions!",
    UserId = "innocenty.popov",
    Service = new ServiceInformation
    {
        Name = "GitHub",
        WebUrl = "https://github.com"
    }
};

await graphClient.Me.Profile.WebAccounts
    .Request()
    .AddAsync(webAccount);

```