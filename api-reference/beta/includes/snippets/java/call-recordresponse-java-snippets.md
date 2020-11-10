---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64208da9fe260cc14692ef82fd0d663488f6269c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959562"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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
    .recordResponse(promptsList,bargeInAllowed,initialSilenceTimeoutInSeconds,maxSilenceTimeoutInSeconds,maxRecordDurationInSeconds,playBeep,null,stopTonesList,clientContext)
    .buildRequest()
    .post();

```