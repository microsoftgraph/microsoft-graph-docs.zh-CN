---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e265c88aee8ba0f9440c314f735b7b6bcd6b7d8
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819842"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sendActivityNotificationToRecipients = {
    topic: {
        source: 'entityUrl',
        value: 'https://graph.microsoft.com/beta/appCatalogs/teamsApps/{teamsAppId}'
    },
    activityType: 'pendingFinanceApprovalRequests',
    previewText: {
        content: 'Internal spending team has a pending finance approval requests'
    },
    recipients: [
        {
            '@odata.type': 'microsoft.graph.aadUserNotificationRecipient',
            userId: '569363e2-4e49-4661-87f2-16f245c5d66a'
        },
        {
            '@odata.type': 'microsoft.graph.aadUserNotificationRecipient',
            userId: 'ab88234e-0874-477c-9638-d144296ed04f'
        },
        {
            '@odata.type': 'microsoft.graph.aadUserNotificationRecipient',
            userId: '01c64f53-69aa-42c7-9b7f-9f75195d6bfc'
        }
    ],
    templateParameters: [
        {
            name: 'pendingRequestCount',
            value: '5'
        }
    ] 
};

await client.api('/teamwork/sendActivityNotificationToRecipients')
    .version('beta')
    .post(sendActivityNotificationToRecipients);

```