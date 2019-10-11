---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af0d59e99448d80ebf5e6ba88610ee717d4ab9f9
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428848"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{id}"]
    .CreateReplyAll(null,null)
    .Request()
    .PostAsync();

```