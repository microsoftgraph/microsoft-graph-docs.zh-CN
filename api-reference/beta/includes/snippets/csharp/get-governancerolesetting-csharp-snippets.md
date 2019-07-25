---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4578139588d3203f9e6f0b5c63cefedd9311d12d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712156"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var governanceRoleSetting = await graphClient.PrivilegedAccess["azureResources"].RoleSettings["80dc5d6f-8d89-47b3-953f-01dc909ed3f9"]
    .Request()
    .GetAsync();

```