---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a714f35f05666e367003866251666c1907af640
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509025"
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