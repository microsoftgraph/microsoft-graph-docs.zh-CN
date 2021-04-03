---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1050e57a598967a1a9cfe5cee1e685bef83a354f
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573182"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "return=representation"));
requestOptions.add(new HeaderOption("If-Match", "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\""));

PlannerPlan plannerPlan = new PlannerPlan();
plannerPlan.title = "title-value";

graphClient.planner().plans("{plan-id}")
    .buildRequest( requestOptions )
    .patch(plannerPlan);

```