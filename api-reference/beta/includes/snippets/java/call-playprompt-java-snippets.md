---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5355650571412bcc27b5d1ee6753190c604a8180
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967907"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String clientContext = "d45324c1-fcb5-430a-902c-f20af696537c";

LinkedList<Prompt> promptsList = new LinkedList<Prompt>();
MediaPrompt prompts = new MediaPrompt();
MediaInfo mediaInfo = new MediaInfo();
mediaInfo.uri = "https://cdn.contoso.com/beep.wav";
mediaInfo.resourceId = "1D6DE2D4-CD51-4309-8DAA-70768651088E";
prompts.mediaInfo = mediaInfo;

promptsList.add(prompts);

Boolean loop = false;

graphClient.communications().calls("57dab8b1-894c-409a-b240-bd8beae78896")
    .playPrompt(CallPlayPromptParameterSet
        .newBuilder()
        .withPrompts(promptsList)
        .withLoop(loop)
        .withClientContext(clientContext)
        .build())
    .buildRequest()
    .post();

```