---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d6f98c53b3dea4204e63b5ae02927fdea2b7ec7dedfa4900f140ff72ba50291
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902568"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var scopedRoleMembers = await graphClient.AdministrativeUnits["{administrativeUnit-id}"].ScopedRoleMembers
    .Request()
    .GetAsync();

```