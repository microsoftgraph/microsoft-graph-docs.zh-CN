---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5cc4c400b5b168ebd1c910fc97fe4fa4746e0f1e
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48610320"
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