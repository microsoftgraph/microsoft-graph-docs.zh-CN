---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bde54a630bb201f046456dba445ecd9d10362ed7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800776"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var claimsMappingPolicy = await graphClient.Policies.ClaimsMappingPolicies["{claimsMappingPolicy-id}"]
    .Request()
    .GetAsync();

```