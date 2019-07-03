---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d555a3a7e36645ca4cee8f07a83c4dd1ef019bc0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478281"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.PrivilegedRoleAssignments["{id}"]
    .MakeEligible()
    .Request()
    .PostAsync();

```