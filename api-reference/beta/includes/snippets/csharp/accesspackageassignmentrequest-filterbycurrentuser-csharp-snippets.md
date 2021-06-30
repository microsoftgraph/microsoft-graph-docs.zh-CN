---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c559b3e11063881b288cd606f5e0c617726768de
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211920"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentRequests
    .FilterByCurrentUser(AccessPackageAssignmentRequestFilterByCurrentUserOptions.Target)
    .Request()
    .GetAsync();

```