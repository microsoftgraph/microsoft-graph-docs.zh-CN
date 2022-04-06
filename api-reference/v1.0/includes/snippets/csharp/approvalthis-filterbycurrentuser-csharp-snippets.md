---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3ac4312230e010bd0ffc8f7a9f37d47d16d025a
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63515823"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentApprovals
    .FilterByCurrentUser(ApprovalFilterByCurrentUserOptions.Approver)
    .Request()
    .GetAsync();

```