---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a080feea7a806f44f5c2a7fd583b9bcc160f4bd4
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758979"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleManagementPolicies = await graphClient.Policies.RoleManagementPolicies
    .Request()
    .Filter("scopeId eq '/' and scopeType eq 'DirectoryRole'")
    .GetAsync();

```