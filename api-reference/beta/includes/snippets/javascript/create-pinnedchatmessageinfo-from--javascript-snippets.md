---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a9c166fde83765294597d1d928bc99b42527af60
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65693864"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const pinnedChatMessageInfo = {
   'message@odata.bind':'https://graph.microsoft.com/beta/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages/1616964509832'
};

await client.api('/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/pinnedMessages')
    .version('beta')
    .post(pinnedChatMessageInfo);

```