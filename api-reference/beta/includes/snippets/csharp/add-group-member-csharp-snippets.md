---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e1d1084a185aab4856951ab9fa67b1d7736a5e53
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37544164"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "{id}"
};

await graphClient.Groups["{id}"].Members.References
    .Request()
    .AddAsync(directoryObject);

```