---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35a2ef1c68ed15dfa780fd271b39594c89fbb9baa99002380d3c851ab85f97aa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219839"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleManagementPolicy = await graphClient.Policies.RoleManagementPolicies["{unifiedRoleManagementPolicy-id}"]
    .Request()
    .GetAsync();

```