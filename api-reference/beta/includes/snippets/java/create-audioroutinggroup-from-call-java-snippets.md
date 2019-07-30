---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5b7c6acf80c32b368af972dad97b735bb90cd10b
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933823"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AudioRoutingGroup audioRoutingGroup = new AudioRoutingGroup();
audioRoutingGroup.id = "oneToOne";
audioRoutingGroup.routingMode = RoutingMode.ONE_TO_ONE;
LinkedList<String> sourcesList = new LinkedList<String>();
sourcesList.add("632899f8-2ea1-4604-8413-27bd2892079f");
audioRoutingGroup.sources = sourcesList;
LinkedList<String> receiversList = new LinkedList<String>();
receiversList.add("550fae72-d251-43ec-868c-373732c2704f");
audioRoutingGroup.receivers = receiversList;

graphClient.app().calls("{id}").audioRoutingGroups()
    .buildRequest()
    .post(audioRoutingGroup);

```