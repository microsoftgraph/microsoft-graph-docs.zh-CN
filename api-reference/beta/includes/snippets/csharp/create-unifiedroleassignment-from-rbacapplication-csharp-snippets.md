---
description: 自动生成的文件。 不修改
ms.openlocfilehash: df3b96bb3d40d1742ae0b1a19c2404a6a795945a
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461274"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignment = new UnifiedRoleAssignment
{
    PrincipalId = "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
    RoleDefinitionId = "b0f54661-2d74-4c50-afa3-1ec803f12efe",
    ResourceScope = "/"
};

await graphClient.RoleManagement.Directory.RoleAssignments
    .Request()
    .AddAsync(unifiedRoleAssignment);

```