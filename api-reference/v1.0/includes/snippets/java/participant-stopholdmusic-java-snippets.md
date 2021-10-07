---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 45c16d33222bb5f84308d5351681b5c0cb39d0a6
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/06/2021
ms.locfileid: "60214621"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String clientContext = "d45324c1-fcb5-430a-902c-f20af696537c";

graphClient.communications().calls("e141b67c-90fd-455d-858b-b48a40b9cc8d").participants("fa1e9582-7145-4ca3-bcd8-577f561fcb6e")
    .stopHoldMusic(ParticipantStopHoldMusicParameterSet
        .newBuilder()
        .withClientContext(clientContext)
        .build())
    .buildRequest()
    .post();

```