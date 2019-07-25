---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8059aeed7494206979579fdcff022e146efe9ed6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884749"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id","https://graph.microsoft.com/v1.0/users/{id}"}
    }
};

await graphClient.Groups["{id}"].Owners.References
    .Request()
    .AddAsync(directoryObject);

```