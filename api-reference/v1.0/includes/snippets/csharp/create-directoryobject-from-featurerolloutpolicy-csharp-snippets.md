---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1cf0b6dad0823902aafec9f3571e1052fb6eb823879d1698afd10978a319711b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332981"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "2441b489-4f12-4882-b039-8f6006bd66da"
};

await graphClient.Policies.FeatureRolloutPolicies["{featureRolloutPolicy-id}"].AppliesTo.References
    .Request()
    .AddAsync(directoryObject);

```