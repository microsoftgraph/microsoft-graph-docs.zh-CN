---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8891cacc2cdc18492656e97a9635278c039a4441c3457d3889f6fac09e9b118
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278587"
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