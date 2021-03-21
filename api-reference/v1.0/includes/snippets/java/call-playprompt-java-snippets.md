---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 418e1d0485a13419de1ebe80de1ccd7ace6dfaf1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974168"
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

graphClient.communications().calls("57dab8b1-894c-409a-b240-bd8beae78896")
    .playPrompt(CallPlayPromptParameterSet
        .newBuilder()
        .withPrompts(promptsList)
        .withClientContext(clientContext)
        .build())
    .buildRequest()
    .post();

```