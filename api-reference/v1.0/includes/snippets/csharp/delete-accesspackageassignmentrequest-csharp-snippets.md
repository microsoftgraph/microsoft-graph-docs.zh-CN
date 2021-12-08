---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9fa6126a332c4c768ec480e1fa22722f42218156
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61334566"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.EntitlementManagement.AssignmentRequests["{accessPackageAssignmentRequest-id}"]
    .Request()
    .DeleteAsync();

```