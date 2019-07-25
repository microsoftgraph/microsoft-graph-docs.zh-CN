---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b467821ffef4ed10b75674bb20838b06d067ddc5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870869"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SchedulingGroup schedulingGroup = new SchedulingGroup();
schedulingGroup.displayName = "Cashiers";
schedulingGroup.isActive = true;
LinkedList<String> userIdsList = new LinkedList<String>();
userIdsList.add("c5d0c76b-80c4-481c-be50-923cd8d680a1");
userIdsList.add("2a4296b3-a28a-44ba-bc66-0274b9b95851");
schedulingGroup.userIds = userIdsList;

graphClient.teams("{teamId}").schedule().schedulingGroups()
    .buildRequest()
    .post(schedulingGroup);

```