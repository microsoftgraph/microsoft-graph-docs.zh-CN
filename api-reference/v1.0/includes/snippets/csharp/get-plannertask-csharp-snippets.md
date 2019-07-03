---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 333d9558b2680644aa52cc95e50ce5272d2a4d88
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466764"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerTask = await graphClient.Planner.Tasks["{task-id}"]
    .Request()
    .GetAsync();

```