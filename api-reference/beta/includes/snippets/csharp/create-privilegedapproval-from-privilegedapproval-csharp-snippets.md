---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79d17a2e2450acb74df556f0b9a5f6b7bfb79ae7
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683912"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedApproval = new PrivilegedApproval
{
    UserId = "userId-value",
    RoleId = "roleId-value",
    ApprovalType = "approvalType-value",
    ApprovalState = ApprovalState.Pending,
    ApprovalDuration = new Duration("datetime-value")
};

await graphClient.PrivilegedApproval
    .Request()
    .AddAsync(privilegedApproval);

```