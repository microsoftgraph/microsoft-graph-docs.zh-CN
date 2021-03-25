---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76767dae82ef48806d69ac1eda66a7542aaef7c6
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201615"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var featureRolloutPolicies = await graphClient.Policies.FeatureRolloutPolicies
    .Request()
    .GetAsync();

```