---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 739becd29ab56d9e0708fc3d607aed70bc447348
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690135"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITeamsTabCollectionPage tabs = graphClient.teams("6903fa93-605b-43ef-920e-77c4729f8258").channels("19:33b76eea88574bd1969dca37e2b7a819@thread.skype").tabs()
    .buildRequest()
    .filter("teamsApp/id eq 'com.microsoft.teamspace.tab.planner'")
    .expand("teamsApp")
    .get();

```