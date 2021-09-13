---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a4b0efd5e07d44a39af8c4207f179531c5e3df785bf93afb9e96164f5aac9a2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332968"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String clientContext = "d45324c1-fcb5-430a-902c-f20af696537c";

graphClient.communications().calls("57dab8b1-894c-409a-b240-bd8beae78896").participants("2765eb15-01f8-47c6-b12b-c32111a4a86f")
    .mute(ParticipantMuteParameterSet
        .newBuilder()
        .withClientContext(clientContext)
        .build())
    .buildRequest()
    .post();

```