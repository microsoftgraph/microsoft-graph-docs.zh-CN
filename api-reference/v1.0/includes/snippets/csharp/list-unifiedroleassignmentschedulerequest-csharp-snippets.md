---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f6e5139ad987f5ff65ac386faab9171834c29c2
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207237"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleAssignmentScheduleRequests = await graphClient.RoleManagement.Directory.RoleAssignmentScheduleRequests
    .Request()
    .GetAsync();

```