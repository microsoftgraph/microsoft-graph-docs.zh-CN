---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31af26cf2457113d157fd968b1ba8b51cc720771
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475341"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleEligibilitySchedule = await graphClient.RoleManagement.Directory.RoleEligibilitySchedules["{unifiedRoleEligibilitySchedule-id}"]
    .Request()
    .GetAsync();

```