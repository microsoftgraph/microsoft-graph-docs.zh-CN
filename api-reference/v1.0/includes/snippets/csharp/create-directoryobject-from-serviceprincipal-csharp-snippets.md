---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1aad641f1367e205034cb73a6df7d67418773459
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334806"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "{id}"
};

await graphClient.ServicePrincipals["{id}"].Owners.References
    .Request()
    .AddAsync(directoryObject);

```