---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fba91d598916c6e854f826dcff46c8adb5fc7547
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892183"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("If-Match", "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\""));

PlannerAssignedToTaskBoardTaskFormat plannerAssignedToTaskBoardTaskFormat = new PlannerAssignedToTaskBoardTaskFormat();
PlannerOrderHintsByAssignee orderHintsByAssignee = new PlannerOrderHintsByAssignee();
orderHintsByAssignee.aaa27244-1db4-476a-a5cb-004607466324 = "8566473P 957764Jk!";
plannerAssignedToTaskBoardTaskFormat.orderHintsByAssignee = orderHintsByAssignee;

graphClient.planner().tasks("{task-id}").assignedToTaskBoardFormat()
    .buildRequest( requestOptions )
    .patch(plannerAssignedToTaskBoardTaskFormat);

```