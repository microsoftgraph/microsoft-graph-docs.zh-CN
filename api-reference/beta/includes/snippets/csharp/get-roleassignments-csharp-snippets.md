---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7b31dcd3b7af292141c88fe2437ed31bdf9b632
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081714"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleAssignments = await graphClient.RoleManagement.Directory.RoleAssignments
    .Request()
    .Filter(" principalId eq 'f1847572-48aa-47aa-96a3-2ec61904f41f'")
    .GetAsync();

```