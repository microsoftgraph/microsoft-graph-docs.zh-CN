---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f36d1583ac23df66e52c32fdd242adc33dd87db
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612340"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var clientContext = "d45324c1-fcb5-430a-902c-f20af696537c";

var participantMixerLevels = new List<ParticipantMixerLevel>()
{
    new ParticipantMixerLevel
    {
        Participant = "550fae72-d251-43ec-868c-373732c2704f",
        Exclusive = true,
        Ducking = new AudioDuckingConfiguration
        {
            RampActive = 50,
            RampInactive = 50,
            LowerLevel = 10,
            UpperLevel = 50
        },
        SourceLevels = new List<AudioSourceLevel>()
        {
            new AudioSourceLevel
            {
                Participant = "632899f8-2ea1-4604-8413-27bd2892079f",
                Level = 50,
                DuckOthers = false
            }
        }
    }
};

await graphClient.App.Calls["{id}"].Participants
    .ConfigureMixer(participantMixerLevels,clientContext)
    .Request()
    .PostAsync();

```