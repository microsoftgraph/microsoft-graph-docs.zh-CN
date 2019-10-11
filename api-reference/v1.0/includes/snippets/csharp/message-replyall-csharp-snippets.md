---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7cb13124870b446d5d80e30327b1538158d033bf
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428851"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "comment-value";

await graphClient.Me.Messages["{id}"]
    .ReplyAll(null,comment)
    .Request()
    .PostAsync();

```