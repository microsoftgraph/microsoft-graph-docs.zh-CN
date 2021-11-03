---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 567b00ef8867ec44b310483193babd6148c8a2648c7a3cfafabdb50de2b14064
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104534"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var approvalStep = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentApprovals["{approval-id}"].Steps["{approvalStep-id}"]
    .Request()
    .GetAsync();

```