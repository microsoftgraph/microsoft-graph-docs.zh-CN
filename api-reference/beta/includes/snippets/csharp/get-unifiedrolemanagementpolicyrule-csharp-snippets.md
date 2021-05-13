---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0f07aa83f55b50b3784c25d6d5d49030971b964
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474781"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleManagementPolicyRule = await graphClient.Policies.RoleManagementPolicies["{unifiedRoleManagementPolicy-id}"].Rules["{unifiedRoleManagementPolicyRule-id}"]
    .Request()
    .GetAsync();

```