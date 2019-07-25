---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6fb5a38aca0dc3423580abe54651fc14518b3de4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857968"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id","https://graph.microsoft.com/beta/users/alexd@contoso.com"}
    }
};

await graphClient.Groups["{id}"].RejectedSenders.References
    .Request()
    .AddAsync(directoryObject);

```