---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 92ace5ca57738fdba9063813191b28bb0c897aa1c3853529debeb7d647d91136
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277553"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appliesTo = await graphClient.Policies.ClaimsMappingPolicies["{claimsMappingPolicy-id}"].AppliesTo
    .Request()
    .GetAsync();

```