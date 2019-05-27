---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4578139588d3203f9e6f0b5c63cefedd9311d12d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34471108"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var governanceRoleSetting = await graphClient.PrivilegedAccess["azureResources"].RoleSettings["80dc5d6f-8d89-47b3-953f-01dc909ed3f9"]
    .Request()
    .GetAsync();

```