---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3fffc41c99db18e1f4205c58287b1850d6788e9e
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "37637861"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Planner.Buckets["{task-id}"].Tasks
    .Request()
    .GetAsync();

```