---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 83473236e23ebb0150d924d7f01eda77327c9dcd
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272433"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerRosterMember plannerRosterMember = new PlannerRosterMember();
plannerRosterMember.userId = "String";

graphClient.planner().rosters("6519868f-868f-6519-8f86-19658f861965").members()
    .buildRequest()
    .post(plannerRosterMember);

```