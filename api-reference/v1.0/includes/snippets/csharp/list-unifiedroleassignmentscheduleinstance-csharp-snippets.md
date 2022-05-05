---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33d5828ab51fa3c46e37dc8c451f16f1b0265b8e
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207318"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleAssignmentScheduleInstances = await graphClient.RoleManagement.Directory.RoleAssignmentScheduleInstances
    .Request()
    .GetAsync();

```