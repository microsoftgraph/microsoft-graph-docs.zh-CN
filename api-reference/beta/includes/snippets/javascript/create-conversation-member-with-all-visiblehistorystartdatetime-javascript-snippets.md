---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 602af99be3ef7f196a6c6200ddabaac3e93384be
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753223"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationMember = {
    @odata.type: "#microsoft.graph.aadUserConversationMember",
    user@odata.bind: "https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5",
    visibleHistoryStartDateTime: "0001-01-01T00:00:00Z"
};

let res = await client.api('/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members')
    .version('beta')
    .post(conversationMember);

```