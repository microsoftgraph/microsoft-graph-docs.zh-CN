---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 612013fa6f028bc0caa53c17e38df7c2402ecbe3c75ddd42fc73def5a01f7f70
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221086"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var includes = await graphClient.Policies.PermissionGrantPolicies["{permissionGrantPolicy-id}"].Includes
    .Request()
    .GetAsync();

```