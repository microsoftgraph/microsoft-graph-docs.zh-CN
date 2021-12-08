---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a37647783b047c0939b35750d35ff7069b2552b1
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61342883"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.IdentityGovernance.EntitlementManagement.Assignments
    .FilterByCurrentUser(AccessPackageAssignmentFilterByCurrentUserOptions.Target)
    .Request()
    .GetAsync();

```