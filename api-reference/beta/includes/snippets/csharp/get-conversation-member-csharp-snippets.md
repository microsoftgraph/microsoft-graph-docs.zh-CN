---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 408e6ba2f66a0b2fce06eac17006ecc77c40944714bf6323e19633d24a2700bf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161285"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationMember = await graphClient.Chats["{chat-id}"].Members["{conversationMember-id}"]
    .Request()
    .GetAsync();

```