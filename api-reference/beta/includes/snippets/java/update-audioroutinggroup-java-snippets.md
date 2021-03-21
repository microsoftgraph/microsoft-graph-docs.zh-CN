---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9cb46f395e6554bb6512fee18345d909ae8bca70
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982283"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AudioRoutingGroup audioRoutingGroup = new AudioRoutingGroup();
audioRoutingGroup.id = "oneToOne";
audioRoutingGroup.routingMode = RoutingMode.ONE_TO_ONE;
LinkedList<String> sourcesList = new LinkedList<String>();
sourcesList.add("632899f8-2ea1-4604-8413-27bd2892079f");
audioRoutingGroup.sources = sourcesList;
LinkedList<String> receiversList = new LinkedList<String>();
receiversList.add("550fae72-d251-43ec-868c-373732c2704f");
receiversList.add("72f988bf-86f1-41af-91ab-2d7cd011db47");
audioRoutingGroup.receivers = receiversList;

graphClient.communications().calls("{id}").audioRoutingGroups("{id}")
    .buildRequest()
    .patch(audioRoutingGroup);

```