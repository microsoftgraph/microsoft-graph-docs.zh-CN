---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4e1adef058dac141bc4a819ef73474463f66633
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976205"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsTabCollectionPage tabs = graphClient.chats("19:d65713bc498c4a428c71ef9353e6ce20@thread.v2").tabs()
    .buildRequest()
    .filter("teamsApp/id eq 'com.microsoft.teamspace.tab.web'")
    .expand("teamsApp")
    .get();

```