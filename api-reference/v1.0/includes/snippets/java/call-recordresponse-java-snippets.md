---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 959daf9216b443384fee0b0ea49a5a7fdb3f4c2d
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44682149"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

boolean bargeInAllowed = true;

String clientContext = "d45324c1-fcb5-430a-902c-f20af696537c";

LinkedList<Prompt> promptsList = new LinkedList<Prompt>();
MediaPrompt prompts = new MediaPrompt();
MediaInfo mediaInfo = new MediaInfo();
mediaInfo.uri = "https://cdn.contoso.com/beep.wav";
mediaInfo.resourceId = "1D6DE2D4-CD51-4309-8DAA-70768651088E";
prompts.mediaInfo = mediaInfo;

promptsList.add(prompts);

int maxRecordDurationInSeconds = 10;

int initialSilenceTimeoutInSeconds = 5;

int maxSilenceTimeoutInSeconds = 2;

boolean playBeep = true;

LinkedList<String> stopTonesList = new LinkedList<String>();
stopTonesList.add("#");
stopTonesList.add("1");
stopTonesList.add("*");

graphClient.communications().calls("{id}")
    .recordResponse(promptsList,bargeInAllowed,initialSilenceTimeoutInSeconds,maxSilenceTimeoutInSeconds,maxRecordDurationInSeconds,playBeep,stopTonesList,clientContext)
    .buildRequest()
    .post();

```