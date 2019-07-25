---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 385289f24b04dd604f1793de393b9d940f5f622e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891059"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id","https://graph.microsoft.com/v1.0/directoryObjects/{id}"}
    }
};

await graphClient.DirectoryRoles["{id}"].Members.References
    .Request()
    .AddAsync(directoryObject);

```