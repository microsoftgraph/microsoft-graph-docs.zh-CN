---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 869a6348853614a2781ed64e3bdf25240bf5185c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959047"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleAssignments = await graphClient.RoleManagement.Directory.RoleAssignments
    .Request()
    .Filter("roleDefinitionId eq '62e90394-69f5-4237-9190-012177145e10'")
    .Expand("principal")
    .GetAsync();

```