---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fddf7097d6b250a984cf7b8ef38e2e1ccbc0a234
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36174708"
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
    ExpirationDateTime = "2019-03-01T21:43:37.5031462+00:00",
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