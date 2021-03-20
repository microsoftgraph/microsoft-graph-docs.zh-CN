---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c4c0e92555e09a68123f26fe5c92b920da2fa625
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978184"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsTab teamsTab = new TeamsTab();
teamsTab.displayName = "My Contoso Tab - updated again";

graphClient.chats("19:d65713bc498c4a428c71ef9353e6ce20@thread.v2").tabs("794f0e4e-4d10-4bb5-9079-3a465a629eff")
    .buildRequest()
    .patch(teamsTab);

```