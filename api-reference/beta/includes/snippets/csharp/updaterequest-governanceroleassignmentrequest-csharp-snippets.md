---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d93e234ecfb6e5abba65312e640643dfc677feb9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713877"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.PrivilegedAccess["azureResources"].RoleAssignmentRequests["7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee"]
    .UpdateRequest(decision,assignmentState,schedule,reason)
    .Request()
    .PostAsync();

```