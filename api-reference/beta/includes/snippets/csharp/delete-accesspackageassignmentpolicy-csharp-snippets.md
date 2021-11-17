---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f1354e543678bd3264ee79d3bac77e6706847c1f586f6e851a8c586a90db75b9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902819"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentPolicies["{accessPackageAssignmentPolicy-id}"]
    .Request()
    .DeleteAsync();

```