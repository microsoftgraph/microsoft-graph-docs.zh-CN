---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d2543fa58579b18df8d25c2fe364b1572201b6c3
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "66040920"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Directory.AdministrativeUnits["{administrativeUnit-id}"].Members
    .Request()
    .GetAsync();

```