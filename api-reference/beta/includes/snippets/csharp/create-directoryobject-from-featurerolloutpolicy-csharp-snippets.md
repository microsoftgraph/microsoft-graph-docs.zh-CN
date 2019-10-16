---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6bcde1e0791d923949d730fbd569e1fe2088783b
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37544168"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "2441b489-4f12-4882-b039-8f6006bd66da"
};

await graphClient.Directory.FeatureRolloutPolicies["{id}"].AppliesTo.References
    .Request()
    .AddAsync(directoryObject);

```