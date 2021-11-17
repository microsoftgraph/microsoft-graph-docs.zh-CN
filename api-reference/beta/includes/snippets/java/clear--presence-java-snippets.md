---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c41affc96954a768a095cd0fb7999854e73b2e048605c6a8a2c38181c57638ed
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163943"
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