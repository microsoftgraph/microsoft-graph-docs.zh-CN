---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7438079fe58026afc53f7e22d5fb9a6a3eeeb111
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49944768"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignment = await graphClient.RoleManagement.Directory.RoleAssignments["lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1"]
    .Request()
    .Expand("directoryScope")
    .GetAsync();

```