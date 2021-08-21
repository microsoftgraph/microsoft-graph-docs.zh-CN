---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0cc7e24f9735dd540b0220f24f68dedb8234e1cfb9a5fa2cd9d4c82a7066d83d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219841"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleEligibilityScheduleInstance = await graphClient.RoleManagement.Directory.RoleEligibilityScheduleInstances["{unifiedRoleEligibilityScheduleInstance-id}"]
    .Request()
    .GetAsync();

```