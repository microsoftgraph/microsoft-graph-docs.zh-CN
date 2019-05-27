---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 61c4b0d7491e81087219bbf9d5babf7f9581a8c7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439909"
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