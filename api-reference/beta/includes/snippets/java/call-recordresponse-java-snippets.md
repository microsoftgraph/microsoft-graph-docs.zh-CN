---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 063775989958f713ae7ba4082e1b7e16000712a944e2005a87fbf888576256c4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219283"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean bargeInAllowed = true;

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

Boolean playBeep = true;

LinkedList<String> stopTonesList = new LinkedList<String>();
stopTonesList.add("#");
stopTonesList.add("1");
stopTonesList.add("*");

graphClient.communications().calls("{id}")
    .recordResponse(CallRecordResponseParameterSet
        .newBuilder()
        .withPrompts(promptsList)
        .withBargeInAllowed(bargeInAllowed)
        .withInitialSilenceTimeoutInSeconds(initialSilenceTimeoutInSeconds)
        .withMaxSilenceTimeoutInSeconds(maxSilenceTimeoutInSeconds)
        .withMaxRecordDurationInSeconds(maxRecordDurationInSeconds)
        .withPlayBeep(playBeep)
        .withStreamWhileRecording(null)
        .withStopTones(stopTonesList)
        .withClientContext(clientContext)
        .build())
    .buildRequest()
    .post();

```