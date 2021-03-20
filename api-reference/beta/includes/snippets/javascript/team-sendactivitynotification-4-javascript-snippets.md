---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4fe3ee80365f51b12dd17539cfd08f6a3e1b694d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941936"
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
    templateParameters: [
        {
            name: 'deploymentId',
            value: '6788662'
        }
    ]
};

await client.api('/users/{userId}/teamwork/sendActivityNotification')
    .version('beta')
    .post(sendActivityNotification);

```