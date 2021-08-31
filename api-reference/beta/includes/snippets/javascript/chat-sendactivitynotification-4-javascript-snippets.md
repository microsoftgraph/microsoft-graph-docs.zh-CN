---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a598299df331f2982a6222bf29795069615eaea451968da9d009588d63132bd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106686"
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