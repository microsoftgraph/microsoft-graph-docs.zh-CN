---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b5dadceffe4a144129eface19ad1f73c0022873f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519901"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var functions = await graphClient.ServicePrincipals["{id}"].Synchronization.Jobs["{jobId}"].Schema.Functions()
    .Request()
    .GetAsync();

```