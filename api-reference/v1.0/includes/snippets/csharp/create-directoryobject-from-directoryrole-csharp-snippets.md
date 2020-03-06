---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c75a1eb10e31d84b5f01f4fa1acda4dc390bd69
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37544214"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "{id}"
};

await graphClient.DirectoryRoles["{id}"].Members.References
    .Request()
    .AddAsync(directoryObject);

```