---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39aeea3e2c9deec3d23858fcd0f8bdc7f0c59f8c
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316911"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sendActivityNotification = {
    topic: {
        source: 'entityUrl',
        value: 'https://graph.microsoft.com/beta/chats/19:1c3af46e9e0f4a5293343c8813c47619@thread.v2'
    },
    activityType: 'taskCreated',
    previewText: {
        content: 'New Task Created'
    },
    recipient: {
        '@odata.type': 'microsoft.graph.chatMembersNotificationRecipient',
        chatId: '19:1c3af46e9e0f4a5293343c8813c47619@thread.v2'
    },
    templateParameters: [
        {
            name: 'taskId',
            value: 'Task 12322'
        }
    ] 
};

await client.api('/chats/19:1c3af46e9e0f4a5293343c8813c47619@thread.v2/sendActivityNotification')
    .version('beta')
    .post(sendActivityNotification);

```