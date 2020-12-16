---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a16f53752d6cf0f1d8371997c44d9225631d5e1
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689806"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsTab teamsTab = new TeamsTab();
teamsTab.displayName = "My Contoso Tab - updated again";

graphClient.chats("19:d65713bc498c4a428c71ef9353e6ce20@thread.v2").tabs("794f0e4e-4d10-4bb5-9079-3a465a629eff")
    .buildRequest()
    .patch(teamsTab);

```