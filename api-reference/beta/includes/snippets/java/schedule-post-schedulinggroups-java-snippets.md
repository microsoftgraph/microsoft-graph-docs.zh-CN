---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0059d379c06c339fcbf27c090c4abf428f9e14cd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980738"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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