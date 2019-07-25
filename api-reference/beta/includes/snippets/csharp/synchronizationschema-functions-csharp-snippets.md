---
description: 自动生成的文件。 不修改
ms.openlocfilehash: db18181d98ffaa5d4985b2093997e55b84016496
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869175"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var functions = await graphClient.ServicePrincipals["{id}"].Synchronization.Jobs["{jobId}"].Schema
    .Functions()
    .Request()
    .GetAsync();

```