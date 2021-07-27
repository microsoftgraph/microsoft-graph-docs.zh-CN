---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f93002d8046e48a2a6402bb9010cc19e8205bc01
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580371"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const chatMessage = {
    body: {
        contentType: 'html',
        content: '<div><div><at id=\"0\">General</at>&nbsp;Hello there!</div></div>'
    },
    mentions: [
        {
            id: 0,
            mentionText: 'General',
            mentioned: {
                conversation: {
                    id: '19:0b50940236084d258c97b21bd01917b0@thread.skype',
                    displayName: 'General',
                    conversationIdentityType: 'channel'
                }
            }
        }
    ]
};

await client.api('/teams/68a3e365-f7d9-4a56-b499-24332a9cc572/channels/19:0b50940236084d258c97b21bd01917b0@thread.skype/messages')
    .post(chatMessage);

```