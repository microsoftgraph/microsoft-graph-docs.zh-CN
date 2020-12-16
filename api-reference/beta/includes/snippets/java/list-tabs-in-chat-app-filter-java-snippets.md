---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5645b4509f0c971dd5aad37ec9de8e37144300e6
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689931"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITeamsTabCollectionPage tabs = graphClient.chats("19:d65713bc498c4a428c71ef9353e6ce20@thread.v2").tabs()
    .buildRequest()
    .filter("teamsApp/id eq 'com.microsoft.teamspace.tab.web'")
    .expand("teamsApp")
    .get();

```