---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d206f6d83859abb89e8a5c1a8a5b5d935e873cb6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779274"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = new Group
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/beta/groups/{id}"}
    }
};

await graphClient.Print.Shares["{printerShare-id}"].AllowedGroups.References
    .Request()
    .AddAsync(group);

```