---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5e32db7cef17be05df01f959e54842bfdc887db
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753832"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const channel = {
    displayName: "TestChannelModeration",
    description: "Test channel moderation.",
    membershipType: "standard",
    moderationSettings: {
        userNewMessageRestriction: "everyoneExceptGuests",
        replyRestriction: "everyone",
        allowNewMessageFromBots: true,
        allowNewMessageFromConnectors: true
    }
};

let res = await client.api('/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels')
    .version('beta')
    .post(channel);

```