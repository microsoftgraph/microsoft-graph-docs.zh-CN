---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b483867fd3bc2c10c22ef74f80e5a75df829b20
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961208"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appliesTo = await graphClient.Policies.TokenLifetimePolicies["{tokenLifetimePolicy-id}"].AppliesTo
    .Request()
    .GetAsync();

```