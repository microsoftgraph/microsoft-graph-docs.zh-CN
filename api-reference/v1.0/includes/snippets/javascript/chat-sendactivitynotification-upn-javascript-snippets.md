---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2701d2810f6e27e7c9f180e5b2e17d3528e74618
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696492"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sendActivityNotification = {
    topic: {
        source: 'entityUrl',
        value: 'https://graph.microsoft.com/v1.0/chats/{chatId}/messages/{messageId}'
    },
    activityType: 'approvalRequired',
    previewText: {
        content: 'Deployment requires your approval'
    },
    recipient: {
        '@odata.type': 'Microsoft.Teams.GraphSvc.aadUserNotificationRecipient',
        userId: 'jacob@contoso.com'
    },
    templateParameters: [
        {
            name: 'approvalTaskId',
            value: '2020AAGGTAPP'
        }
    ]
};

await client.api('/chats/{chatId}/sendActivityNotification')
    .post(sendActivityNotification);

```