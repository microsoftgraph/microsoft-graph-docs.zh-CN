---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c68fc0d4bbccbc686cfa7038c6ad076875f0dd4eb305712abaf77b9790e5cf9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278582"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "15c1a2d5-9101-44b2-83ab-885db8a647ca"
};

await graphClient.DirectoryRoles["{directoryRole-id}"].Members.References
    .Request()
    .AddAsync(directoryObject);

```