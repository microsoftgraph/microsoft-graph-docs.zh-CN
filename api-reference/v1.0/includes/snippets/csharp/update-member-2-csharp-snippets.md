---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ae7e92e0ed1169153915243d35e1f21313cf3a9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963615"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationMember = new AadUserConversationMember
{
    Roles = new List<String>()
    {
        "owner"
    }
};

await graphClient.Teams["{team-id}"].Members["{conversationMember-id}"]
    .Request()
    .UpdateAsync(conversationMember);

```