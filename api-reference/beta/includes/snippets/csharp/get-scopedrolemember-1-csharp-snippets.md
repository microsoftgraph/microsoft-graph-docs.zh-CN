---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3555f5ad14b666a55a117d14a5416227b0c470cf
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942996"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var scopedRoleMembership = await graphClient.AdministrativeUnits["{administrativeUnit-id}"].ScopedRoleMembers["{scopedRoleMembership-id}"]
    .Request()
    .GetAsync();

```