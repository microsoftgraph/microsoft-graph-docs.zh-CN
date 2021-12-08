---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 047b54e65b94cef4ed4c6624150cfed92829a1e1
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61342838"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var assignmentRequests = await graphClient.IdentityGovernance.EntitlementManagement.AssignmentRequests
    .Request()
    .GetAsync();

```