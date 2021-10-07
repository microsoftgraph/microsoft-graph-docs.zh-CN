---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fa209b4690f015386ffb08d6e53a6700020f27e5
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/06/2021
ms.locfileid: "60214668"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MediaPrompt customMediaPrompt = new MediaPrompt();
MediaInfo mediaInfo = new MediaInfo();
mediaInfo.uri = "https://bot.contoso.com/onHold.wav";
customPrompt.mediaInfo = mediaInfo;

String clientContext = "d45324c1-fcb5-430a-902c-f20af696537c";

graphClient.communications().calls("e141b67c-90fd-455d-858b-b48a40b9cc8d").participants("fa1e9582-7145-4ca3-bcd8-577f561fcb6e")
    .startHoldMusic(ParticipantStartHoldMusicParameterSet
        .newBuilder()
        .withCustomPrompt(customPrompt)
        .withClientContext(clientContext)
        .build())
    .buildRequest()
    .post();

```