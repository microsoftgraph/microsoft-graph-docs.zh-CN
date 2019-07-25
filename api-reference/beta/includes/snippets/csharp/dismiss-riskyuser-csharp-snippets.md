---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 31a56258c6964991777e226a89c67118eee244bc
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725679"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userIds = new List<String>()
{
    "04487ee0-f4f6-4e7f-8999-facc5a30e232",
    "13387ee0-f4f6-4e7f-8999-facc5120e345"
};

await graphClient.RiskyUsers
    .Dismiss(userIds)
    .Request()
    .PostAsync();

```