---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a91ef4710b0f49aebc71c8942ff8b2660bbb21f66320743eb430ade30a624d1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332848"
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