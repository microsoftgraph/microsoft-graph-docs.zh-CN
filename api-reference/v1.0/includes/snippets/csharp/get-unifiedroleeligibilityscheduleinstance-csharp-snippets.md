---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d2454466b84b32e23b9b383835ae897c574edc81
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204889"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleEligibilityScheduleInstance = await graphClient.RoleManagement.Directory.RoleEligibilityScheduleInstances["{unifiedRoleEligibilityScheduleInstance-id}"]
    .Request()
    .GetAsync();

```