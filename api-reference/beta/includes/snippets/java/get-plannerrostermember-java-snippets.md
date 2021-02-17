---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c1785248c4d5e07191784f6d21ce89b9cc8280b
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272350"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerRosterMember plannerRosterMember = graphClient.planner().rosters("523a9d5a-f9d5-45c1-929f-b8525393515c").members("5ba84f7a-aa11-4a51-a298-9f2c7ec6bb38")
    .buildRequest()
    .get();

```