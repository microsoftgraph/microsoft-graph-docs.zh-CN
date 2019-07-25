---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3bb4156f2cfbb9a9ee1eeaa5487fa06d1427bb00
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728508"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoleAssignment = await graphClient.PrivilegedRoleAssignments["{id}"]
    .Request()
    .GetAsync();

```