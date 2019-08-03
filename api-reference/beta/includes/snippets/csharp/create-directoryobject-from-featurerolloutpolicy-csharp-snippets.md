---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 903466b1ef0b5d52b841f9d005b1a930d92e3202
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36172830"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id"," https://graph.microsoft.com/beta/directoryObjects/2441b489-4f12-4882-b039-8f6006bd66da"}
    }
};

await graphClient.Directory.FeatureRolloutPolicies["{id}"].AppliesTo.References
    .Request()
    .AddAsync(directoryObject);

```