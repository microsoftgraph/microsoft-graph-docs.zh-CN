---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d45de46ffbd1e417159bc02760c4a2cd758ba25
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777662"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedApproval = new PrivilegedApproval
{
    ApprovalState = ApprovalState.Pending,
    ApproverReason = "approverReason-value"
};

await graphClient.PrivilegedApproval["{privilegedApproval-id}"]
    .Request()
    .UpdateAsync(privilegedApproval);

```