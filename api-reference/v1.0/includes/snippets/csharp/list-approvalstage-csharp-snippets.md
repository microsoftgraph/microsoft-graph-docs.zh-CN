---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4fa410899d32f7e728dc8eb547117051caf4559f
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63515909"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stages = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentApprovals["{approval-id}"].Stages
    .Request()
    .GetAsync();

```