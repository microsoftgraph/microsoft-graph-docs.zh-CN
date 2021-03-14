---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8def2b961032b6c6c130e1376e776c5aae196bcb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792565"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "{id}"
};

await graphClient.Groups["{group-id}"].Owners.References
    .Request()
    .AddAsync(directoryObject);

```