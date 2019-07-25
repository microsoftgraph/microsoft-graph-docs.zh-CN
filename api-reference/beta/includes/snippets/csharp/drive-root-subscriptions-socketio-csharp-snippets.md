---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 21ab5b4454c31f3299eb676dfbfe6d96c066309b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713067"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subscription = await graphClient.Me.Drive.Root.Subscriptions["socketIo"]
    .Request()
    .GetAsync();

```