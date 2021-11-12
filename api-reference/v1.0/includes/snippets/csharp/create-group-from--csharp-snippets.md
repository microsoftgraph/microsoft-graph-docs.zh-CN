---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c407f706487b37b5dd22f4530b945856c1259354462505f9c1f68ab49749e764
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378722"
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