---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dcb577e5d13cf5658325a88f40d703fbf2db12d8
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52473440"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleManagementPolicies = await graphClient.Policies.RoleManagementPolicies
    .Request()
    .GetAsync();

```