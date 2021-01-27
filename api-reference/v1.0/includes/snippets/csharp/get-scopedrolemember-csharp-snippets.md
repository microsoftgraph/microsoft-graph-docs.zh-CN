---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc94ba21b35458db105494176159f8070c81f6e1
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49984937"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var scopedRoleMembership = await graphClient.Directory.AdministrativeUnits["{id}"].ScopedRoleMembers["{id}"]
    .Request()
    .GetAsync();

```