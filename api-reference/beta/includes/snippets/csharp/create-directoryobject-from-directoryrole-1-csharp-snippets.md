---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5477e2b2056d2ea5cdcbffe331269f21fd2220326437bacbbb86c03030fa4e4e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105222"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "0f933635-5b77-4cf4-a577-f78a5eb090a2"
};

await graphClient.DirectoryRoles["{directoryRole-id}"].Members.References
    .Request()
    .AddAsync(directoryObject);

```