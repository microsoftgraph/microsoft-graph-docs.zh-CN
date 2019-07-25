---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 64d9d3c7de23a851ddf73b6a44bc61722720eb56
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720591"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerBucketTaskBoardTaskFormat = new PlannerBucketTaskBoardTaskFormat
{
    OrderHint = "A6673H Ejkl!"
};

await graphClient.Planner.Tasks["hsOf2dhOJkqyYYZEtdzDe2QAIUCR"].BucketTaskBoardFormat
    .Request()
    .Header("If-Match","W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"")
    .UpdateAsync(plannerBucketTaskBoardTaskFormat);

```