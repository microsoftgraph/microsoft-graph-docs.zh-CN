---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2bf95e12712c2af426e2b939d933b47bc555856689cd7cec033dcede969e1bf7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105109"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var rules = await graphClient.Policies.RoleManagementPolicies["{unifiedRoleManagementPolicy-id}"].Rules
    .Request()
    .GetAsync();

```