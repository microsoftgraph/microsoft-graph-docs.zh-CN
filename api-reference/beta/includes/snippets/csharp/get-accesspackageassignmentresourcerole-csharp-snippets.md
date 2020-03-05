---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da5680af31ea6a197dc443c89bc5750d8764b01c
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40911794"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignmentResourceRole = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentResourceRoles["{id}"]
    .Request()
    .GetAsync();

```