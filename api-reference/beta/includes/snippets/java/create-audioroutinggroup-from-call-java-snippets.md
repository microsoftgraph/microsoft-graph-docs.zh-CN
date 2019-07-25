---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 84220c187d73b5e6071fdc032ab8dced40d93dc0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864708"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AudioRoutingGroup AudioRoutingGroup = new AudioRoutingGroup();
AudioRoutingGroup.id = "oneToOne";
AudioRoutingGroup.routingMode = RoutingMode.ONE_TO_ONE;
LinkedList<String> sourcesList = new LinkedList<String>();
sourcesList.add("632899f8-2ea1-4604-8413-27bd2892079f");
AudioRoutingGroup.sources = sourcesList;
LinkedList<String> receiversList = new LinkedList<String>();
receiversList.add("550fae72-d251-43ec-868c-373732c2704f");
AudioRoutingGroup.receivers = receiversList;

graphClient.app().calls("{id}").audioRoutingGroups()
    .buildRequest()
    .post(AudioRoutingGroup);

```