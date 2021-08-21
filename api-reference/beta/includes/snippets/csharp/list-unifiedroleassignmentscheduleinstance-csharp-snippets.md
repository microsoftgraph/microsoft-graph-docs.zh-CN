---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b3a99db6919f009d60a1460679abab3067f5859c6b330b15f653743c3ffdf21
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103922"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleAssignmentScheduleInstances = await graphClient.RoleManagement.Directory.RoleAssignmentScheduleInstances
    .Request()
    .GetAsync();

```