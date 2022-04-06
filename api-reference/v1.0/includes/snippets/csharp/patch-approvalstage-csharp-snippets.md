---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 293edb283a0303be069651bd126badd45c6150a1
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516061"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var approvalStage = new ApprovalStage
{
    ReviewResult = "Approve",
    Justification = "OK"
};

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentApprovals["{approval-id}"].Stages["{approvalStage-id}"]
    .Request()
    .UpdateAsync(approvalStage);

```