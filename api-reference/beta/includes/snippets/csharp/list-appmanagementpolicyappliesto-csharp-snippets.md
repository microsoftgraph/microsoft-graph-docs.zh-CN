---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 02b2c901212b37895873bba4aa450711f3fb90f8
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58258989"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appliesTo = await graphClient.Policies.AppManagementPolicies["{appManagementPolicy-id}"].AppliesTo
    .Request()
    .GetAsync();

```