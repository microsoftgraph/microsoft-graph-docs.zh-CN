---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d45ae06d323a74773c91cfde291ae1be22b81ee6368bec8cdfda08d5e141426
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902900"
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