---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 77fafb086743f0064111174b725e4a27c5dee0fc
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/11/2019
ms.locfileid: "36845949"
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
    },
    IsEnabled = true
};

await graphClient.RoleManagement.Directory.RoleDefinitions
    .Request()
    .AddAsync(unifiedRoleDefinition);

```