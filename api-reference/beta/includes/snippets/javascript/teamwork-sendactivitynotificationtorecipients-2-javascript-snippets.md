---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e700b54ee8117754f359d17346b53e76157289e5
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819841"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sendActivityNotificationToRecipients = {
    topic: {
        source: 'text',
        value: 'Deployment Approvals Channel',
        webUrl: 'https://teams.microsoft.com/l/message/19:448cfd2ac2a7490a9084a9ed14cttr78c@thread.skype/1605223780000?tenantId=c8b1bf45-3834-4ecf-971a-b4c755ee677d&groupId=d4c2a937-f097-435a-bc91-5c1683ca7245&parentMessageId=1605223771864&teamName=Approvals&channelName=Azure%20DevOps&createdTime=1605223780000'
    },
    activityType: 'deploymentApprovalRequired',
    previewText: {
        content: 'New deployment requires your approval'
    },
    templateParameters: [
        {
            name: 'deploymentId',
            value: '6788662'
        }
    ],
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
    ]
};

await client.api('/teamwork/sendActivityNotificationToRecipients')
    .version('beta')
    .post(sendActivityNotificationToRecipients);

```