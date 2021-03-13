---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 75ed2d69d804ab26a680e8209a6726142103a0fc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780203"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const channel = {
    displayName: 'UpdateChannelModeration',
    description: 'Update channel moderation.',
    moderationSettings: {
        userNewMessageRestriction: 'moderators',
        replyRestriction: 'everyone',
        allowNewMessageFromBots: true,
        allowNewMessageFromConnectors: true
    }
};

await client.api('/teams/{team-id}/channels/{channel-id}')
    .version('beta')
    .update(channel);

```