---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 990469523094417db99548435e029d5bd898598bb621ec02280d532f849e4bc9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106676"
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