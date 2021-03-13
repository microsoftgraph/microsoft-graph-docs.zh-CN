---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6eddf740aa676ff5702cf9aa4b6b619215383951
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778155"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "{id}"
};

await graphClient.Applications["{application-id}"].Owners.References
    .Request()
    .AddAsync(directoryObject);

```