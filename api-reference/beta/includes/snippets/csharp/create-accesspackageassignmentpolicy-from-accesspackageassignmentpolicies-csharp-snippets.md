---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2afab06f946f28a6560ece0b9ba204b945dc104e
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37992859"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignmentPolicy = new AccessPackageAssignmentPolicy
{
    AccessPackageId = "56ff43fd-6b05-48df-9634-956a777fce6d",
    DisplayName = "direct",
    Description = "direct assignments by administrator",
    IsEnabled = true
};

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentPolicies
    .Request()
    .AddAsync(accessPackageAssignmentPolicy);

```