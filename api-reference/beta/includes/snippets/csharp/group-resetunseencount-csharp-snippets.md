---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29dd5074e76826e36977ebe901ee1daee148bf61
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796991"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{group-id}"]
    .ResetUnseenCount()
    .Request()
    .PostAsync();

```