---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6584919c523bd29127352a77c3ff55efb1499f3
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516473"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var approval = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentApprovals["{approval-id}"]
    .Request()
    .GetAsync();

```