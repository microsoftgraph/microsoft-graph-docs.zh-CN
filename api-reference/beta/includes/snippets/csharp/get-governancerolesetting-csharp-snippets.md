---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4578139588d3203f9e6f0b5c63cefedd9311d12d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499754"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var governanceRoleSetting = await graphClient.PrivilegedAccess["azureResources"].RoleSettings["80dc5d6f-8d89-47b3-953f-01dc909ed3f9"]
    .Request()
    .GetAsync();

```