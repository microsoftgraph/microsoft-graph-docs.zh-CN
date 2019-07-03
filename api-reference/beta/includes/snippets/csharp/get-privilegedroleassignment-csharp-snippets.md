---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3bb4156f2cfbb9a9ee1eeaa5487fa06d1427bb00
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478717"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoleAssignment = await graphClient.PrivilegedRoleAssignments["{id}"]
    .Request()
    .GetAsync();

```