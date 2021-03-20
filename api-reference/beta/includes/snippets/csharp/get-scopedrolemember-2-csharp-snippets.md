---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7dc12db52a40c85c4ed05df2a020facddf1a24b3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942964"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var scopedRoleMembers = await graphClient.AdministrativeUnits["{administrativeUnit-id}"].ScopedRoleMembers
    .Request()
    .GetAsync();

```