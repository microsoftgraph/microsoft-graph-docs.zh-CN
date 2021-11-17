---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 728820026c172d947425038cb660805c6c1390d5d7bfee616df55c2f54239906
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158389"
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