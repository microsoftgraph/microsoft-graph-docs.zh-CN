---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c6c2b460b7082a16cfc7a049dfe1290d6a9929f5ae8dba5f5bc0c14b525b7115
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902588"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AdministrativeUnits["{administrativeUnit-id}"].ScopedRoleMembers["{scopedRoleMembership-id}"]
    .Request()
    .DeleteAsync();

```