---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a42bdcece138678326e5cdfd5d443ad84ceab171
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972363"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerPlanDetails plannerPlanDetails = graphClient.planner().plans("{plan-id}").details()
    .buildRequest()
    .get();

```