---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0f36d1583ac23df66e52c32fdd242adc33dd87db
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730596"
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