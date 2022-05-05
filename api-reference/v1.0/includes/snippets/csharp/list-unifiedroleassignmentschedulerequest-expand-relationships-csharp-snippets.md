---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a53aa2aad8141fd82f5c2f6ce3c8ffcfe00522c2
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207263"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleAssignmentScheduleRequests = await graphClient.RoleManagement.Directory.RoleAssignmentScheduleRequests
    .Request()
    .Expand("roleDefinitionId")
    .Select("principalId,action,roleDefinitionId")
    .GetAsync();

```