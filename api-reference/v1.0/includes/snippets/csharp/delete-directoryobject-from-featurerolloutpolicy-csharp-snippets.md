---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c58221eb3b7791ceaaa4ff72c9bba5584ec0251
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201544"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.FeatureRolloutPolicies["{featureRolloutPolicy-id}"].AppliesTo["{directoryObject-id}"].Reference
    .Request()
    .DeleteAsync();

```