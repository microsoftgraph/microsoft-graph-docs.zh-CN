---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c8769ff563d6da859708eb1b95974ff0a4b9bd78
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466770"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerBucketTaskBoardTaskFormat = await graphClient.Planner.Tasks["{task-id}"].BucketTaskBoardFormat
    .Request()
    .GetAsync();

```