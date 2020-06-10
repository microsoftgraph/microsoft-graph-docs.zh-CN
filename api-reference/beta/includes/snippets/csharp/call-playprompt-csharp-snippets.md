---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 880c40a783a5da6bd0b0edacfc9c20a8f7121bbe
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681599"
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

await graphClient.Communications.Calls["57dab8b1-894c-409a-b240-bd8beae78896"]
    .PlayPrompt(prompts,loop,clientContext)
    .Request()
    .PostAsync();

```