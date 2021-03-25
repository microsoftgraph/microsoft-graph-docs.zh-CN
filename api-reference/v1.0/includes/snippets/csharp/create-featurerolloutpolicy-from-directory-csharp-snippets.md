---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 791de5ca8bec051eb4cfbeb0f5a1723929caa2b1
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201579"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var featureRolloutPolicy = new FeatureRolloutPolicy
{
    DisplayName = "PassthroughAuthentication rollout policy",
    Description = "PassthroughAuthentication rollout policy",
    Feature = StagedFeatureName.PassthroughAuthentication,
    IsEnabled = true,
    IsAppliedToOrganization = false
};

await graphClient.Policies.FeatureRolloutPolicies
    .Request()
    .AddAsync(featureRolloutPolicy);

```