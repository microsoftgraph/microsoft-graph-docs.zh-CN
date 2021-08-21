---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0bbbc5a64f88e41c8e09b7be99f6948f33be4ea6713c9b930165b1687a986ae9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215770"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleEligibilityScheduleRequest = await graphClient.RoleManagement.Directory.RoleEligibilityScheduleRequests["{unifiedRoleEligibilityScheduleRequest-id}"]
    .Request()
    .GetAsync();

```