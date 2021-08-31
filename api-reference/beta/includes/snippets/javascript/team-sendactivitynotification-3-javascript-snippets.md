---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 21f02d78e61e39f80d47d2e26eef249e92f6b31b202ff79bf12012d529a6c118
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107133"
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