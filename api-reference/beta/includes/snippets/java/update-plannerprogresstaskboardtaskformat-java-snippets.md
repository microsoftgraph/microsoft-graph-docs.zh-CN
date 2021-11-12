---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a625abc472bb6f2ce39ae498df16ac6ccb6420d705c0308fe8d3899557052940
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273974"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "return=representation"));
requestOptions.add(new HeaderOption("If-Match", "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\""));

PlannerProgressTaskBoardTaskFormat plannerProgressTaskBoardTaskFormat = new PlannerProgressTaskBoardTaskFormat();
plannerProgressTaskBoardTaskFormat.orderHint = "A6673H Ejkl!";

graphClient.planner().tasks("{id}").progressTaskBoardFormat()
    .buildRequest( requestOptions )
    .patch(plannerProgressTaskBoardTaskFormat);

```