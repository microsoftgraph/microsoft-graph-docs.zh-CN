---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 52762a4102bed50064819b9bd067296324b8bb0c
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201398"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var featureRolloutPolicy = await graphClient.Directory.FeatureRolloutPolicies["{featureRolloutPolicy-id}"]
    .Request()
    .Expand("appliesTo")
    .GetAsync();

```