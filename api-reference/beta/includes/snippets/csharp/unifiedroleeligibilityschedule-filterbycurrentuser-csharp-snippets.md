---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7d5f17aa7e805e4a8760007e4d117cf825b5e9d
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58513142"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.RoleManagement.Directory.RoleEligibilitySchedules
    .FilterByCurrentUser(RoleEligibilityScheduleFilterByCurrentUserOptions.Principal)
    .Request()
    .GetAsync();

```