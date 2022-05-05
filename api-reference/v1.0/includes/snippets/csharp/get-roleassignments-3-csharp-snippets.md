---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e5b4e00870a9e0b13e5b551c4cc93f0bb1e3ff8d
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207438"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleAssignments = await graphClient.RoleManagement.EntitlementManagement.RoleAssignments
    .Request()
    .Filter("appScopeId eq '/AccessPackageCatalog/4cee616b-fdf9-4890-9d10-955e0ccb12bc'")
    .Expand("principal")
    .GetAsync();

```