---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c5840f1dd77ac94c0b7bb4a26c56806d4938e327
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858173"
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

await graphClient.Groups["{id}"].AcceptedSenders.References
    .Request()
    .AddAsync(directoryObject);

```