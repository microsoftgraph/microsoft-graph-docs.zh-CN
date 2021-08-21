---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc8e17800163574e705cc0be178a3a5916477ef76f9e11f7d4a90531af404aa4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274122"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignmentSchedule = await graphClient.RoleManagement.Directory.RoleAssignmentSchedules["{unifiedRoleAssignmentSchedule-id}"]
    .Request()
    .GetAsync();

```