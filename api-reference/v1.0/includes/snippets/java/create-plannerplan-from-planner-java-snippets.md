---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 463307cacf6d48d9622667cea7b7bbf95c01aed9
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2019
ms.locfileid: "35881257"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerPlan plannerPlan = new PlannerPlan();
plannerPlan.owner = "ebf3b108-5234-4e22-b93d-656d7dae5874";
plannerPlan.title = "title-value";

graphClient.planner().plans()
    .buildRequest()
    .post(plannerPlan);

```