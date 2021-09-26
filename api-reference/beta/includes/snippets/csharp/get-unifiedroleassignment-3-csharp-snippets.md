---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab22d1d53282aae6a2915772de893b5c8618346d4f3f842340e80a57c97ff49c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278353"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignmentMultiple = await graphClient.RoleManagement.CloudPC.RoleAssignments["{unifiedRoleAssignmentMultiple-id}"]
    .Request()
    .Expand("roleDefinition")
    .GetAsync();

```