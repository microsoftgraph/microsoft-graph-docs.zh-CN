---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a7fe4630bd0f0ad884d621b866cd13b0299f2c35
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50274710"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPlannerPlanCollectionPage plans = graphClient.groups("ebf3b108-5234-4e22-b93d-656d7dae5874").planner().plans()
    .buildRequest()
    .get();

```