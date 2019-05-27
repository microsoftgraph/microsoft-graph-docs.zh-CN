---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d555a3a7e36645ca4cee8f07a83c4dd1ef019bc0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443171"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.PrivilegedRoleAssignments["{id}"]
    .MakeEligible()
    .Request()
    .PostAsync();

```