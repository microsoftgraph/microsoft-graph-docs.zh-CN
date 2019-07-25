---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 37dd6350563c2449bfe71fa7fb05baadcd77d9c0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734822"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerProgressTaskBoardTaskFormat = await graphClient.Planner.Tasks["{task-id}"].ProgressTaskBoardFormat
    .Request()
    .GetAsync();

```