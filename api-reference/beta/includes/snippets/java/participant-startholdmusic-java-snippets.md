---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fa209b4690f015386ffb08d6e53a6700020f27e5
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59507294"
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