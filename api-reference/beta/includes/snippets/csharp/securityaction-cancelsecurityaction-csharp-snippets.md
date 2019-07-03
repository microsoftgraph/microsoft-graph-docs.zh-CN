---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7855fbf3bc9fb4c03063c2cc41de033349b64d2a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500215"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Security.SecurityActions["{id}"]
    .CancelSecurityAction()
    .Request()
    .PostAsync();

```