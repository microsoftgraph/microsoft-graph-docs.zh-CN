---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 510ad31949da3e4bb6b29a020083dcd2fd3cd90c
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "35717400"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var jobs = await graphClient.ServicePrincipals["{id}"].Synchronization.Jobs
    .Request()
    .GetAsync();

```