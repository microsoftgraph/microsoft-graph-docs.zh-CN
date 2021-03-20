---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97e43ecfacccb4aa221b48093cc79e565bd44330
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948013"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sendActivityNotification = {
    topic: {
        source: 'entityUrl',
        value: 'https://graph.microsoft.com/beta/chats/{chatId}'
    },
    activityType: 'taskCreated',
    previewText: {
        content: 'New Task Created'
    },
    recipient: {
        '@odata.type': 'microsoft.graph.aadUserNotificationRecipient',
        userId: '569363e2-4e49-4661-87f2-16f245c5d66a'
    },
    templateParameters: [
        {
            name: 'taskId',
            value: 'Task 12322'
        }
    ] 
};

await client.api('/chats/{chatId}/sendActivityNotification')
    .version('beta')
    .post(sendActivityNotification);

```