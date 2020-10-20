---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a918586b0cb62135430dabd89766a665f154723d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608636"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ids = new List<String>()
{
    "84b80893-8749-40a3-97b7-68513b600544",
    "5d6059b6-368d-45f8-91e1-8e07d485f1d0"
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