---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2cd11e7a6298a836a215f2589d4e6c61e0595a44
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520162"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
};

await graphClient.Users["{id}"].Manager.Reference
    .Request()
    .PutAsync(directoryObject);

```