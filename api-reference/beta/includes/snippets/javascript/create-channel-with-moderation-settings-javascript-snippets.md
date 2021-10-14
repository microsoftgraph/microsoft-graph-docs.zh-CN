---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d365548069d26fa318448fd0d5f970ceb761a09a677b498f85dd14ac85af6156
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164018"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const channel = {
    displayName: 'TestChannelModeration',
    description: 'Test channel moderation.',
    membershipType: 'standard',
    moderationSettings: {
        userNewMessageRestriction: 'everyoneExceptGuests',
        replyRestriction: 'everyone',
        allowNewMessageFromBots: true,
        allowNewMessageFromConnectors: true
    }
};

await client.api('/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels')
    .version('beta')
    .post(channel);

```