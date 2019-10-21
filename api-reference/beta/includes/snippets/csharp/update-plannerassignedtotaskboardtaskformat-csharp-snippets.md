---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2db058af1ddf6b16cbbc25b41dafb0c53f5b7814
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2019
ms.locfileid: "35720633"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerAssignedToTaskBoardTaskFormat = new PlannerAssignedToTaskBoardTaskFormat
{
    OrderHintsByAssignee = new PlannerOrderHintsByAssignee
    {
        Aaa27244-1db4-476a-a5cb-004607466324 = "8566473P 957764Jk!"
    }
};

await graphClient.Planner.Tasks["01gzSlKkIUSUl6DF_EilrmQAKDhh"].AssignedToTaskBoardFormat
    .Request()
    .Header("If-Match","W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"")
    .UpdateAsync(plannerAssignedToTaskBoardTaskFormat);

```