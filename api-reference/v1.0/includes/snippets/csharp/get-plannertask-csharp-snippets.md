---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 333d9558b2680644aa52cc95e50ce5272d2a4d88
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608537"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerTask = await graphClient.Planner.Tasks["{task-id}"]
    .Request()
    .GetAsync();

```