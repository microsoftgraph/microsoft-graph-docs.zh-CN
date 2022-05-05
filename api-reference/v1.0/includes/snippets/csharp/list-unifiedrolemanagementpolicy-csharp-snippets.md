---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a080feea7a806f44f5c2a7fd583b9bcc160f4bd4
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207647"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleManagementPolicies = await graphClient.Policies.RoleManagementPolicies
    .Request()
    .Filter("scopeId eq '/' and scopeType eq 'DirectoryRole'")
    .GetAsync();

```