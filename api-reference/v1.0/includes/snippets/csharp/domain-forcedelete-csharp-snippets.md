---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0e5c597c2af5f5a78120a3b5bb2b51acbf97b411
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733527"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var disableUserAccounts = true;

await graphClient.Domains["{id}"]
    .ForceDelete(disableUserAccounts)
    .Request()
    .PostAsync();

```