---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ec47b2c184f49eeb152cd34e4bc347df146ec6c
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428784"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{id}"]
    .CreateForward(null,null,null)
    .Request()
    .PostAsync();

```