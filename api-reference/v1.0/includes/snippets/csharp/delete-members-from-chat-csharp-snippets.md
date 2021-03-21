---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce3e8ce6e6b0e914e740c03bacf16ef4f977cc41
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958414"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Chats["{chat-id}"].Members["{conversationMember-id}"]
    .Request()
    .DeleteAsync();

```