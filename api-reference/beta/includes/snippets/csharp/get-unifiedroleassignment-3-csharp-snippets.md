---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4727fe89178bc4a373e0725b2040e6e0d9abf76c
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869973"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignmentMultiple = await graphClient.RoleManagement.CloudPC.RoleAssignments["{unifiedRoleAssignmentMultiple-id}"]
    .Request()
    .Expand("roleDefinition")
    .GetAsync();

```