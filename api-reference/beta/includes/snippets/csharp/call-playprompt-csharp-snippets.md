---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2e43e1335384a4bc083ed396c41841adbc3cf6f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786316"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

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

var loop = false;

await graphClient.Communications.Calls["{call-id}"]
    .PlayPrompt(prompts,loop,clientContext)
    .Request()
    .PostAsync();

```