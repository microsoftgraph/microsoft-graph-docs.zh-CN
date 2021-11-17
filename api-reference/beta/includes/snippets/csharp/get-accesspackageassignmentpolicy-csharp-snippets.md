---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 52c7e729594f428527e8f674299802218efd44d5b9f116e85c036d6a37c208e1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902818"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignmentPolicy = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentPolicies["{accessPackageAssignmentPolicy-id}"]
    .Request()
    .GetAsync();

```