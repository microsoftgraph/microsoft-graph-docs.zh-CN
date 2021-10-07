---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80ccccab3c9e384af20c6219e8be1772084ee75d
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/06/2021
ms.locfileid: "60214669"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var customPrompt = new MediaPrompt
{
    MediaInfo = new MediaInfo
    {
        Uri = "https://bot.contoso.com/onHold.wav"
    }
};

var clientContext = "d45324c1-fcb5-430a-902c-f20af696537c";

await graphClient.Communications.Calls["{call-id}"].Participants["{participant-id}"]
    .StartHoldMusic(customPrompt,clientContext)
    .Request()
    .PostAsync();

```