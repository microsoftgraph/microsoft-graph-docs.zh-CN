---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fba91d598916c6e854f826dcff46c8adb5fc7547
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2019
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