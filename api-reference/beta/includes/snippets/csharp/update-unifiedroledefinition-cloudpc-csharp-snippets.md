---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c341a0e6a51fb1091862a1f729f28848cc7edaf7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62089124"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleDefinition = new UnifiedRoleDefinition
{
    Description = "Update basic properties and permission of application registrations",
    DisplayName = "ExampleCustomRole",
    RolePermissions = new List<UnifiedRolePermission>()
    {
        new UnifiedRolePermission
        {
            AllowedResourceActions = new List<String>()
            {
                "Microsoft.CloudPC/CloudPCs/Read",
                "Microsoft.CloudPC/CloudPCs/Reprovision"
            }
        }
    }
};

await graphClient.RoleManagement.CloudPC.RoleDefinitions["{unifiedRoleDefinition-id}"]
    .Request()
    .UpdateAsync(unifiedRoleDefinition);

```