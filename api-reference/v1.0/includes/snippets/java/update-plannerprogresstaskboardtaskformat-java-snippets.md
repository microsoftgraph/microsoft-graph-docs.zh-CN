---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8aebf0bd9a04096e30db7ae3e23df96734b83686
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975894"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("If-Match", "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\""));

PlannerProgressTaskBoardTaskFormat plannerProgressTaskBoardTaskFormat = new PlannerProgressTaskBoardTaskFormat();
plannerProgressTaskBoardTaskFormat.orderHint = "A6673H Ejkl!";

graphClient.planner().tasks("{task-id}").progressTaskBoardFormat()
    .buildRequest( requestOptions )
    .patch(plannerProgressTaskBoardTaskFormat);

```