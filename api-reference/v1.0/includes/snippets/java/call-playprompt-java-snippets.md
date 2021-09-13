---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37f10bcb472d45d9b48691ab5c5dafa756a243fd1a73b93c2f663e63a10e16dc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279694"
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