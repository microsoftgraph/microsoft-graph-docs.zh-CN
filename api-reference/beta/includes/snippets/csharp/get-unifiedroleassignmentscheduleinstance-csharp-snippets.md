---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39922c0107acc285559f49da46e0629cf54498153d7b2fa522941b1ad7868d8c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332472"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignmentScheduleInstance = await graphClient.RoleManagement.Directory.RoleAssignmentScheduleInstances["{unifiedRoleAssignmentScheduleInstance-id}"]
    .Request()
    .GetAsync();

```