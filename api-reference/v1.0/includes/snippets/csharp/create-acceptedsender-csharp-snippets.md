---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f00418ee7a8192345569a4bb0d7d3da0df170650
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888151"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id","https://graph.microsoft.com/v1.0/users/alexd@contoso.com"}
    }
};

await graphClient.Groups["{id}"].AcceptedSenders.References
    .Request()
    .AddAsync(directoryObject);

```