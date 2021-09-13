---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e95bf7ac47e797c2652fd89e1fad790b59ab7b84eeb54c41d7e56ddbb76c45ce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378474"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Directory.AdministrativeUnits["{administrativeUnit-id}"].ScopedRoleMembers["{scopedRoleMembership-id}"]
    .Request()
    .DeleteAsync();

```