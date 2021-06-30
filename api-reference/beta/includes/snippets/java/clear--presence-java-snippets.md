---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b453148281c1d7e7b29f4d0963aac5abf2aa5d3
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208245"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String sessionId = "22553876-f5ab-4529-bffb-cfe50aa89f87";

graphClient.users("fa8bf3dc-eca7-46b7-bad1-db199b62afc3").presence()
    .clearPresence(PresenceClearPresenceParameterSet
        .newBuilder()
        .withSessionId(sessionId)
        .build())
    .buildRequest()
    .post();

```