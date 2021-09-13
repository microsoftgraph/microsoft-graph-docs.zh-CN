---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6f9aad7e1b56cf35627f44fa52559b33fb9a17753146e5a7cff63cab03b104a9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332610"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "comment-value";

var sendResponse = true;

await graphClient.Me.Events["{event-id}"]
    .Accept(comment,sendResponse)
    .Request()
    .PostAsync();

```