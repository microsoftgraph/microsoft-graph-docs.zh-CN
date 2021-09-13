---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae96c15cef8a15501b0cb0db71ab4169b34b3afd4d5c6b528221d2f65e7a8207
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105394"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.FeatureRolloutPolicies["{featureRolloutPolicy-id}"].AppliesTo["{directoryObject-id}"].Reference
    .Request()
    .DeleteAsync();

```