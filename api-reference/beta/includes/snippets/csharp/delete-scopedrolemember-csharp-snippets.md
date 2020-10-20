---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ddabb21e62ba3dd90cb6ab215fe826b11e02ee89
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613115"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AdministrativeUnits["{id}"].ScopedRoleMembers["{id}"]
    .Request()
    .DeleteAsync();

```