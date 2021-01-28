---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 308dbc950335951dd0181e059f60d4a6bdd97e68
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015288"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "{id}"
};

await graphClient.Devices["{id}"].RegisteredOwners.References
    .Request()
    .AddAsync(directoryObject);

```