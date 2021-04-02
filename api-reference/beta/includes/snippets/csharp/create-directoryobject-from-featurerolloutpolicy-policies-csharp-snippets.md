---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5fd0df330559ed6d29a0b517ec2d63ef0e496c1d
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508902"
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