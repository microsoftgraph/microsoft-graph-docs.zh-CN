---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b467821ffef4ed10b75674bb20838b06d067ddc5
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44218393"
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