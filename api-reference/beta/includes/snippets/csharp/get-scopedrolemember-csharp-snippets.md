---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7dc12db52a40c85c4ed05df2a020facddf1a24b3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794970"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var scopedRoleMembers = await graphClient.AdministrativeUnits["{administrativeUnit-id}"].ScopedRoleMembers
    .Request()
    .GetAsync();

```