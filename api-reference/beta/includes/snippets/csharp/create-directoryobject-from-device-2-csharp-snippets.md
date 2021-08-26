---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c3bdae788ec1ce77bd9f89aa6819a01f19520d1626e57beb9001bff8487bd250
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278313"
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