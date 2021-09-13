---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a87a143489bd6482876f31e4514069f30ef100c4a64bc48dd6a2f087f329918f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332978"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var featureRolloutPolicy = await graphClient.Policies.FeatureRolloutPolicies["{featureRolloutPolicy-id}"]
    .Request()
    .Expand("appliesTo")
    .GetAsync();

```