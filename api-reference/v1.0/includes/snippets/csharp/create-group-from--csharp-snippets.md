---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b412efd4c5fd6ff11a14b1df8ff4275410015403
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771461"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = new Group
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/v1.0/groups/{groupId}"}
    }
};

await graphClient.Print.Shares["{printerShare-id}"].AllowedGroups.References
    .Request()
    .AddAsync(group);

```