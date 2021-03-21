---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ec0a94b35c23932f9b87e0119425620c56f19d3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970631"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("If-Match", "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\""));

PlannerPlan plannerPlan = new PlannerPlan();
plannerPlan.title = "title-value";

graphClient.planner().plans("{plan-id}")
    .buildRequest( requestOptions )
    .patch(plannerPlan);

```