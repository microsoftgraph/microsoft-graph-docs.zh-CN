---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2239dcce419b9c3e296454d5d476fd65f57b3e20
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458747"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissionGrantPolicies = await graphClient.Policies.PermissionGrantPolicies
    .Request()
    .GetAsync();

```