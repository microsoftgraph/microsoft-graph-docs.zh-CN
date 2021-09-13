---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f019801faeefed3fbe3ffc7eeb0498d634bcc74067fead2089a6d5f0efb33b8c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409571"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "Cancelling for this week due to all hands";

await graphClient.Me.Events["{event-id}"]
    .Cancel(comment)
    .Request()
    .PostAsync();

```