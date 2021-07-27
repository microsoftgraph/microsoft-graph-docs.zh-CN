---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06e8b26e419c56dae41428596b5944dc99a8ad1a
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580367"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const chatMessage = {
    body: {
        contentType: 'html',
        content: '<div><div><at id=\"0\">GraphTesting</at>&nbsp;Hello team</div></div>'
    },
    mentions: [
        {
            id: 0,
            mentionText: 'GraphTesting',
            mentioned: {
                conversation: {
                    id: '68a3e365-f7d9-4a56-b499-24332a9cc572',
                    displayName: 'GraphTesting',
                    conversationIdentityType: 'team'
                }
            }
        }
    ],
    reactions: []
};

await client.api('/teams/68a3e365-f7d9-4a56-b499-24332a9cc572/channels/19:0b50940236084d258c97b21bd01917b0@thread.skype/messages')
    .post(chatMessage);

```