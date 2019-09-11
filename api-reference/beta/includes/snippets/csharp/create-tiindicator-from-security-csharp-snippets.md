---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b3502a8ef18502eedc1585dcdab7ead92cebb2fe
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/11/2019
ms.locfileid: "36845956"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tiIndicator = new TiIndicator
{
    Action = TiAction.Alert,
    ActivityGroupNames = new List<String>()
    {
    },
    Confidence = 0,
    Description = "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.",
    ExpirationDateTime = DateTimeOffset.Parse("2019-03-01T21:43:37.5031462+00:00"),
    ExternalId = "Test--8586509942679764298MS501",
    FileHashType = FileHashType.Sha256,
    FileHashValue = "aa64428647b57bf51524d1756b2ed746e5a3f31b67cf7fe5b5d8a9daf07ca313",
    KillChain = new List<String>()
    {
    },
    MalwareFamilyNames = new List<String>()
    {
    },
    Severity = 0,
    Tags = new List<String>()
    {
    },
    TargetProduct = "Azure Sentinel",
    ThreatType = "WatchList",
    TlpLevel = TlpLevel.Green
};

await graphClient.Security.TiIndicators
    .Request()
    .AddAsync(tiIndicator);

```