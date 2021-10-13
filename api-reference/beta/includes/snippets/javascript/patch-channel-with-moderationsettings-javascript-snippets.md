---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 055afef3527adff0cf795ac97f3b1f01d072d17df9c069349ed55d23e5e925c3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103743"
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

await client.api('/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2')
    .version('beta')
    .update(channel);

```