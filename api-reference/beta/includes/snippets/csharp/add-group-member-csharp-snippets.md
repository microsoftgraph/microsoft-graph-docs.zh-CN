---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fa6ab643e9175090e85855a588b7cccba957e710
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858087"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id","https://graph.microsoft.com/beta/directoryObjects/{id}"}
    }
};

await graphClient.Groups["{id}"].Members.References
    .Request()
    .AddAsync(directoryObject);

```