---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47497673e5fdbc9efe94b689bb700f90faca6544
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948011"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sendActivityNotification = {
    topic: {
        source: 'entityUrl',
        value: 'https://graph.microsoft.com/beta/chats/{chatId}/messages/{messageId}'
    },
    activityType: 'approvalRequired',
    previewText: {
        content: 'Deployment requires your approval'
    },
    recipient: {
        '@odata.type': 'Microsoft.Teams.GraphSvc.aadUserNotificationRecipient',
        userId: '569363e2-4e49-4661-87f2-16f245c5d66a'
    },
    templateParameters: [
        {
            name: 'approvalTaskId',
            value: '2020AAGGTAPP'
        }
    ]
};

await client.api('/chats/{chatId}/sendActivityNotification')
    .version('beta')
    .post(sendActivityNotification);

```