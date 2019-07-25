---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 94298f47467788d3846313b4fe98267f5e734473
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876286"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("If-Match", "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\""));

PlannerProgressTaskBoardTaskFormat plannerProgressTaskBoardTaskFormat = new PlannerProgressTaskBoardTaskFormat();
plannerProgressTaskBoardTaskFormat.orderHint = "A6673H Ejkl!";

graphClient.planner().tasks("'id'").progressTaskBoardFormat()
    .buildRequest( requestOptions )
    .patch(plannerProgressTaskBoardTaskFormat);

```