---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aeafac5f843203de3b2f1f6add4ca51004e4814c
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52473997"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignments
    .FilterByCurrentUser(AccessPackageAssignmentFilterByCurrentUserOptions.Target)
    .Request()
    .GetAsync();

```