---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bfa7039769893f5c756ef36fd02304a4198ff1e6
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36172869"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Directory.FeatureRolloutPolicies["df85e4d9-e8c4-4033-a41c-73419a95c29c"].AppliesTo["2441b489-4f12-4882-b039-8f6006bd66da"].Reference
    .Request()
    .DeleteAsync();

```