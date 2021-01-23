---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db69d5eff7e35e274e53fe433cc9223332daf7e1
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945419"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var scopedRoleMembership = await graphClient.AdministrativeUnits["{id}"].ScopedRoleMembers["{id}"]
    .Request()
    .GetAsync();

```