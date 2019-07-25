---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 57059aad3a8b2c19823cb90fca4d54663077a696
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716874"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var value = new List<TiIndicator>()
{
    new TiIndicator
    {
        ActivityGroupNames = new List<String>()
        {
        },
        Confidence = 0,
        Description = "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.",
        ExpirationDateTime = "2019-03-02T00:44:03.1668987+03:00",
        ExternalId = "Test--8586509942423126760MS164-0",
        FileHashType = FileHashType.Sha256,
        FileHashValue = "b555c45c5b1b01304217e72118d6ca1b14b7013644a078273cea27bbdc1cf9d6",
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
    },
    new TiIndicator
    {
        ActivityGroupNames = new List<String>()
        {
        },
        Confidence = 0,
        Description = "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.",
        ExpirationDateTime = "2019-03-02T00:44:03.1748779+03:00",
        ExternalId = "Test--8586509942423126760MS164-1",
        FileHashType = FileHashType.Sha256,
        FileHashValue = "1796b433950990b28d6a22456c9d2b58ced1bdfcdf5f16f7e39d6b9bdca4213b",
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
    }
};

await graphClient.Security.TiIndicators
    .SubmitTiIndicators(value)
    .Request()
    .PostAsync();

```