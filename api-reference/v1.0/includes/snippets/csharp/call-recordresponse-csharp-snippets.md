---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4287f5cd31ee263162fe82f072daa0a8667c386c232c4c65d7f76e1de43bc74f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279208"
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