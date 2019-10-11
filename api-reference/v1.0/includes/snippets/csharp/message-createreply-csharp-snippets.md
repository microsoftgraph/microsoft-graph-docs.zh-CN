---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2acaaf13bac2dbb12e11e527259e6114c7f7201b
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428847"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{id}"]
    .CreateReply(null,null)
    .Request()
    .PostAsync();

```