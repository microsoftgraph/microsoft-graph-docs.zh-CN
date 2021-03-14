---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 04cee301e9ae6964f454513a2d61955bd094a612
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796617"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "{id}"
};

await graphClient.Devices["{device-id}"].RegisteredOwners.References
    .Request()
    .AddAsync(directoryObject);

```