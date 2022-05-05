---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d89f771652a77231ba187468c9d2fd54a281dda0
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207035"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleEligibilityScheduleRequests = await graphClient.RoleManagement.Directory.RoleEligibilityScheduleRequests
    .Request()
    .GetAsync();

```