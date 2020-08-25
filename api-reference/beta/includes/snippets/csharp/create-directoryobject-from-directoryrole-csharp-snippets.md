---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 162f4e4483529002d80f289853b78bf45e717fb4
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46872672"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "2c891f12-928d-4da2-8d83-7d2434a0d8dc"
};

await graphClient.DirectoryRoles["0afed502-2456-4fd4-988e-3c21924c28a7"].Members.References
    .Request()
    .AddAsync(directoryObject);

```