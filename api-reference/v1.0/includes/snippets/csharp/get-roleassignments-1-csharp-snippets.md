---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 869a6348853614a2781ed64e3bdf25240bf5185c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59130413"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleAssignments = await graphClient.RoleManagement.Directory.RoleAssignments
    .Request()
    .Filter("roleDefinitionId eq '62e90394-69f5-4237-9190-012177145e10'")
    .Expand("principal")
    .GetAsync();

```