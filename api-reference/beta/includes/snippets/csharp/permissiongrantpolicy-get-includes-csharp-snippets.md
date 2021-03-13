---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a79fb251ebce881f15f1c3b6cfa1104dfb0b637
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807863"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var includes = await graphClient.Policies.PermissionGrantPolicies["{permissionGrantPolicy-id}"].Includes
    .Request()
    .GetAsync();

```