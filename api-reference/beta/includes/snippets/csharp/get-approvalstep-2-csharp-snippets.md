---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c761697962af44d751a5bcca8f397719ba0a4b7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942541"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var approvalStep = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentApprovals["{approval-id}"].Steps["{approvalStep-id}"]
    .Request()
    .GetAsync();

```