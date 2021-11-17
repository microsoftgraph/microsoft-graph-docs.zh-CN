---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f635a2a8eb0108e78b0336f6fa6b1429d49f83c142a9fd8e8b39a4d44b0bebc7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105735"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var excludes = await graphClient.Policies.PermissionGrantPolicies["{permissionGrantPolicy-id}"].Excludes
    .Request()
    .GetAsync();

```