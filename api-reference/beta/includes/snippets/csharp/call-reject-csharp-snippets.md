---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a6d695c7d6c77ffdf70761d2c57e1c5dd9a9b810
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708787"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reason = RejectReason.None;

await graphClient.App.Calls["{id}"]
    .Reject(reason)
    .Request()
    .PostAsync();

```