---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6316ceefa1e25fbef48fb0de6d9b837c2c45d42c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785033"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sendActivityNotification = {
    topic: {
        source: 'text',
        value: 'Deployment Approvals Channel',
        webUrl: 'https://teams.microsoft.com/l/message/19:448cfd2ac2a7490a9084a9ed14cttr78c@thread.skype/1605223780000?tenantId=c8b1bf45-3834-4ecf-971a-b4c755ee677d&groupId=d4c2a937-f097-435a-bc91-5c1683ca7245&parentMessageId=1605223771864&teamName=Approvals&channelName=Azure%20DevOps&createdTime=1605223780000'
    },
    activityType: 'deploymentApprovalRequired',
    previewText: {
        content: 'New deployment requires your approval'
    },
    recipient: {
        '@odata.type': 'Microsoft.Teams.GraphSvc.aadUserNotificationRecipient',
        userId: '569363e2-4e49-4661-87f2-16f245c5d66a'
    },
    templateParameters: [
        {
            name: 'deploymentId',
            value: '6788662'
        }
    ]
};

await client.api('/teams/{teamId}/sendActivityNotification')
    .version('beta')
    .post(sendActivityNotification);

```