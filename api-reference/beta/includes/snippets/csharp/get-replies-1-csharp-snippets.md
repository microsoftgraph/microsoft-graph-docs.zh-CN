---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e76a7b8012c9787e45017d558ed61b5b19e6603
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947797"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var replies = await graphClient.Chats["{chat-id}"].Messages["{chatMessage-id}"].Replies
    .Request()
    .GetAsync();

```