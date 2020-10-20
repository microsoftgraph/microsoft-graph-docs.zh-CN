---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 510ad31949da3e4bb6b29a020083dcd2fd3cd90c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48617377"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var jobs = await graphClient.ServicePrincipals["{id}"].Synchronization.Jobs
    .Request()
    .GetAsync();

```