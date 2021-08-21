---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d524a25cdd0c0c1ca96e3985d6b670a5e247c2648942079ad247fed443009ea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278269"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleEligibilityScheduleRequests = await graphClient.RoleManagement.Directory.RoleEligibilityScheduleRequests
    .Request()
    .GetAsync();

```