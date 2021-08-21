---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb97651436daa35dc2686fdceac8730d9b2748dd75b30d1bc0a2609bea401dd8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215782"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var assignments = await graphClient.PrivilegedRoles["{privilegedRole-id}"].Assignments
    .Request()
    .GetAsync();

```