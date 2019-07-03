---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 61c4b0d7491e81087219bbf9d5babf7f9581a8c7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499487"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedApproval = new PrivilegedApproval
{
    UserId = "userId-value",
    RoleId = "roleId-value",
    ApprovalType = "approvalType-value",
    ApprovalState = ApprovalState.Pending,
    ApprovalDuration = "datetime-value"
};

await graphClient.PrivilegedApproval
    .Request()
    .AddAsync(privilegedApproval);

```