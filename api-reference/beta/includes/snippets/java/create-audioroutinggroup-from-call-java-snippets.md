---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 823a3156c62430eee67b929ab60f68341601616d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969954"
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
audioRoutingGroup.receivers = receiversList;

graphClient.communications().calls("{id}").audioRoutingGroups()
    .buildRequest()
    .post(audioRoutingGroup);

```