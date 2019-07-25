---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e62cd3e02f128f998a75b9e8dac5ecd92780283a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732617"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Events["{id}"]
    .Request()
    .DeleteAsync();

```