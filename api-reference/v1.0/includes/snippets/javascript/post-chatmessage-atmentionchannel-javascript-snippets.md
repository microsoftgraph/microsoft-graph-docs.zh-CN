---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 56db1700a77a3b7acb01ccc79355248bee383606ecdd335e17cf4f3c15a63ba1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334153"
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