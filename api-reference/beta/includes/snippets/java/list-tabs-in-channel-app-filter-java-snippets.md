---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 505b78ea27add1969efe44b7b1957259c95b5750
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983269"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsTabCollectionPage tabs = graphClient.teams("6903fa93-605b-43ef-920e-77c4729f8258").channels("19:33b76eea88574bd1969dca37e2b7a819@thread.skype").tabs()
    .buildRequest()
    .filter("teamsApp/id eq 'com.microsoft.teamspace.tab.planner'")
    .expand("teamsApp")
    .get();

```