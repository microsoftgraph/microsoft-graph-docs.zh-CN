---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7855fbf3bc9fb4c03063c2cc41de033349b64d2a
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48622068"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Security.SecurityActions["{id}"]
    .CancelSecurityAction()
    .Request()
    .PostAsync();

```