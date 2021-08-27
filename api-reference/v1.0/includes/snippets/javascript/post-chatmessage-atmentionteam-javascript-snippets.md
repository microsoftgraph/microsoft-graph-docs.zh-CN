---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 428584005c42df489f34e5c5c74ee80302d417b816c9eb8488cd9f99f5ff0df0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409164"
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