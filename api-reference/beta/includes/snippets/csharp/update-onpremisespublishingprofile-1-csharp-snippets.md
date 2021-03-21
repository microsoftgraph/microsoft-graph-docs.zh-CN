---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 230806e227ae80574954dbb3de152e8d0fdd20ae
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963212"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var hybridAgentUpdaterConfiguration = new HybridAgentUpdaterConfiguration
{
    UpdateWindow = new UpdateWindow
    {
        UpdateWindowStartTime = new TimeOfDay(0, 0, 0),
        UpdateWindowEndTime = new TimeOfDay(23, 59, 0)
    }
};

var onPremisesPublishingProfiles = new OnPremisesPublishingProfile();
onPremisesPublishingProfiles.HybridAgentUpdaterConfiguration = hybridAgentUpdaterConfiguration;

await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"]
    .Request()
    .UpdateAsync(onPremisesPublishingProfiles);

```