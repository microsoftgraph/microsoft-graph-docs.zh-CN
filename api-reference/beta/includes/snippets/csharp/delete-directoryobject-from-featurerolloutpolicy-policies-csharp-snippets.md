---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c58221eb3b7791ceaaa4ff72c9bba5584ec0251
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508706"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.FeatureRolloutPolicies["{featureRolloutPolicy-id}"].AppliesTo["{directoryObject-id}"].Reference
    .Request()
    .DeleteAsync();

```