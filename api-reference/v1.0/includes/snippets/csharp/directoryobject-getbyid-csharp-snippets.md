---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5cc4c400b5b168ebd1c910fc97fe4fa4746e0f1e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467063"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ids = new List<String>()
{
    "84b80893874940a3-97b7-68513b600544",
    "5d6059b6368d-45f8-91e18e07d485f1d0"
};

var types = new List<String>()
{
    "user"
};

await graphClient.DirectoryObjects
    .GetByIds(ids,types)
    .Request()
    .PostAsync();

```