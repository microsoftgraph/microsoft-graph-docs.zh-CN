---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5bd4b45f7749cd6e673d883b91560239753b62aa522448077e70a897fab4ec9c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328745"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignmentMultiple = new UnifiedRoleAssignmentMultiple
{
    DisplayName = "My test role assignment 1",
    Description = "My role assignment description",
    RoleDefinitionId = "b5c08161-a7af-481c-ace2-a20a69a48fb1",
    PrincipalIds = new List<String>()
    {
        "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
        "c1518aa9-4da5-4c84-a902-a31404023890"
    }
};

await graphClient.RoleManagement.CloudPC.RoleAssignments
    .Request()
    .AddAsync(unifiedRoleAssignmentMultiple);

```