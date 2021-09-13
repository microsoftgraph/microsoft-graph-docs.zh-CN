---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 78e4dbd313efcc836d115d13e44b617fba0a6ef473e4a32817f264d9495ab09e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105349"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerPlan plannerPlan = new PlannerPlan();
plannerPlan.owner = "ebf3b108-5234-4e22-b93d-656d7dae5874";
plannerPlan.title = "title-value";

graphClient.planner().plans()
    .buildRequest()
    .post(plannerPlan);

```