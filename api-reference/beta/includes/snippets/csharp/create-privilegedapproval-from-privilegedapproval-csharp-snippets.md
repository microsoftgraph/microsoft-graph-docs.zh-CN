---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 680516f18ee0139a91a426e05efbb9fe7cdcb1a0a973b74df4a8738329b42697
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903392"
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