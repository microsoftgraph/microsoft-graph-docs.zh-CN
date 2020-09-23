---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f91d33256bfd511fd4593f6cd0fd1880f54ae7b2
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223505"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var scopedRoleMembers = await graphClient.Directory.AdministrativeUnits["{id}"].ScopedRoleMembers
    .Request()
    .GetAsync();

```