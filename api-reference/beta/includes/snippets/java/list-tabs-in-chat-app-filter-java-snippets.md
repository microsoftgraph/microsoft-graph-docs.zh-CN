---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c9130eca75366f9e4a25f3652d94721bafdb579471fbc9a52c8e0d9dc77fc16
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277353"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsTabCollectionPage tabs = graphClient.chats("19:d65713bc498c4a428c71ef9353e6ce20@thread.v2").tabs()
    .buildRequest()
    .filter("teamsApp/id eq 'com.microsoft.teamspace.tab.web'")
    .expand("teamsApp")
    .get();

```