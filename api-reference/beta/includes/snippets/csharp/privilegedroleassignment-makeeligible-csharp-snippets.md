---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d555a3a7e36645ca4cee8f07a83c4dd1ef019bc0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728487"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.PrivilegedRoleAssignments["{id}"]
    .MakeEligible()
    .Request()
    .PostAsync();

```