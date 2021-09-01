---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0768974380a705865efd9f97d97fcbd6e3eababcb06039815a018467d8f6f7a
ms.sourcegitcommit: 24d0ea8e2bcb54c2f397133460c3d26fb0ba705f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/11/2021
ms.locfileid: "58785449"
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