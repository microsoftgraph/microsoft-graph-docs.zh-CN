---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5fe57a4fb90971b156a90919f8cf44b3d2a175cb
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50274900"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appliesTo = await graphClient.Policies.TokenIssuancePolicies["{id}"].AppliesTo
    .Request()
    .GetAsync();

```