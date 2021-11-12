---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23f76d40ba52404ed9006acb1eedb49c7c2e660d4590473c7d38263066af4165
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162953"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = new User
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/v1.0/users/{userId}"}
    }
};

await graphClient.Print.Shares["{printerShare-id}"].AllowedUsers.References
    .Request()
    .AddAsync(user);

```