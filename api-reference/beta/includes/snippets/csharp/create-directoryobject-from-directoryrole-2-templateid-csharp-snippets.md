---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d98eb55baba22038434e0873007ea77157da4974
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52990770"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "bb165b45-151c-4cf6-9911-cd7188912848"
};

await graphClient.DirectoryRoles["{directoryRole-id}"].Members.References
    .Request()
    .AddAsync(directoryObject);

```