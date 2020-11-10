---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 463307cacf6d48d9622667cea7b7bbf95c01aed9
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978390"
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