---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33c669b2bbd8c717fadce0f254abe992fb2e2e54
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973804"
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