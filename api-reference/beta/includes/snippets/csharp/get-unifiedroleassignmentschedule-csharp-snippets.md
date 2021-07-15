---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35f9adbe54ab02e5d1fb38759182768258c99f68
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440241"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignmentSchedule = await graphClient.RoleManagement.Directory.RoleAssignmentSchedules["{unifiedRoleAssignmentSchedule-id}"]
    .Request()
    .GetAsync();

```