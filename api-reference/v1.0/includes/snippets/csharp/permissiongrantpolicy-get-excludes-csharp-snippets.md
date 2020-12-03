---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50daf78f80ab150c99c5a03f46b88f93c20aa84c
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523269"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var excludes = await graphClient.Policies.PermissionGrantPolicies["microsoft-application-admin"].Excludes
    .Request()
    .GetAsync();

```