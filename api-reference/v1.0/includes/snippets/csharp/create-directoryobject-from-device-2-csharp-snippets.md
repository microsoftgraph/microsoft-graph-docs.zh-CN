---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b1ecd8a98a56de213ba413d1f5ed9f3bf5179c5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959892"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "{id}"
};

await graphClient.Devices["{device-id}"].RegisteredUsers.References
    .Request()
    .AddAsync(directoryObject);

```