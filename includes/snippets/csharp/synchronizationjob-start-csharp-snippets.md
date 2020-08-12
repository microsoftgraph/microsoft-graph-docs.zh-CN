---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2478b99008a79a75d8b5fdee81c53561ff908f44
ms.sourcegitcommit: 8e18d7fe3c869b2fd48872365116175d3bdce1b7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/12/2020
ms.locfileid: "46643787"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{id}"].Synchronization.Jobs["{jobId}"]
    .Start()
    .Request()
    .PostAsync();

```