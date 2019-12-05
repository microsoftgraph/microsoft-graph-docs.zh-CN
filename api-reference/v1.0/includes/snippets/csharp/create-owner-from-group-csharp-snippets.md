---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 587b87fa4afbf782b514402f97704b9176898c9f
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37544217"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "{id}"
};

await graphClient.Groups["{id}"].Owners.References
    .Request()
    .AddAsync(directoryObject);

```