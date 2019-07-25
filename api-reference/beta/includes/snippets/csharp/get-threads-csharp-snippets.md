---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3b1035bb4fdff81b1eab92f59750532e2bee1f41
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35707243"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var threads = await graphClient.Groups["{id}"].Conversations["{id}"].Threads
    .Request()
    .GetAsync();

```