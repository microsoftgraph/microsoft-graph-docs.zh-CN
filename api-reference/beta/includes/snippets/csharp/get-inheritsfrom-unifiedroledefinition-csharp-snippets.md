---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e2f304eb7042a233a5ad79e0bd7e812309acc18
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778074"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleDefinition = await graphClient.RoleManagement.Directory.RoleDefinitions["{unifiedRoleDefinition-id}"]
    .Request()
    .Expand("inheritsPermissionsFrom")
    .GetAsync();

```