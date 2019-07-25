---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a7b4cd52b1be8d65b3a2346d20f218e528e183ce
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887117"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("If-Match", "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\""));

PlannerPlan plannerPlan = new PlannerPlan();
plannerPlan.title = "title-value";

graphClient.planner().plans("{plan-id}")
    .buildRequest( requestOptions )
    .patch(plannerPlan);

```