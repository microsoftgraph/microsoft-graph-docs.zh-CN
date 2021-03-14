---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 793d6dc8bf9e8cc65c97e77f04681a06c05b24e0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783472"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bargeInAllowed = true;

var clientContext = "d45324c1-fcb5-430a-902c-f20af696537c";

var prompts = new List<Prompt>()
{
    new MediaPrompt
    {
        MediaInfo = new MediaInfo
        {
            Uri = "https://cdn.contoso.com/beep.wav",
            ResourceId = "1D6DE2D4-CD51-4309-8DAA-70768651088E"
        }
    }
};

var maxRecordDurationInSeconds = 10;

var initialSilenceTimeoutInSeconds = 5;

var maxSilenceTimeoutInSeconds = 2;

var playBeep = true;

var stopTones = new List<String>()
{
    "#",
    "1",
    "*"
};

await graphClient.Communications.Calls["{call-id}"]
    .RecordResponse(prompts,bargeInAllowed,initialSilenceTimeoutInSeconds,maxSilenceTimeoutInSeconds,maxRecordDurationInSeconds,playBeep,stopTones,clientContext)
    .Request()
    .PostAsync();

```