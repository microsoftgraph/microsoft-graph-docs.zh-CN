---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cdd46c79a4d91b156bb9f2d1a2a4ab2b65f67460
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461602"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleDefinition = new UnifiedRoleDefinition
{
    Description = "Update basic properties of application registrations",
    DisplayName = "Application Registration Support Administrator",
    RolePermissions = new List<UnifiedRolePermission>()
    {
        new UnifiedRolePermission
        {
            AllowedResourceActions = new List<String>()
            {
                "microsoft.directory/applications/basic/read"
            }
        }
    }
};

await graphClient.RoleManagement.Directory.RoleDefinitions["0d55728d-3e24-4309-9b1b-5ac09921475a"]
    .Request()
    .UpdateAsync(unifiedRoleDefinition);

```