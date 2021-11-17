---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a186df97b47613b0daed60fb98412d07ed19bf97e7367daa8510475e2abd478a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220580"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.RoleManagement.Directory.RoleAssignments["{unifiedRoleAssignment-id}"]
    .Request()
    .DeleteAsync();

```