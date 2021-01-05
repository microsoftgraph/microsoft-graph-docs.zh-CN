---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22ca177f987370fd0629b2be255de08493e1960e
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49754021"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sendActivityNotification = {
    topic: {
        source: "text",
        value: "Deployment Approvals Channel",
        webUrl: "https://teams.microsoft.com/l/message/19:448cfd2ac2a7490a9084a9ed14cttr78c@thread.skype/1605223780000?tenantId=c8b1bf45-3834-4ecf-971a-b4c755ee677d&groupId=d4c2a937-f097-435a-bc91-5c1683ca7245&parentMessageId=1605223771864&teamName=Approvals&channelName=Azure%20DevOps&createdTime=1605223780000"
    },
    activityType: "deploymentApprovalRequired",
    previewText: {
        content: "New deployment requires your approval"
    },
    templateParameters: [
        {
            name: "deploymentId",
            value: "6788662"
        }
    ]
};

let res = await client.api('/users/{userId}/teamwork/sendActivityNotification')
    .version('beta')
    .post(sendActivityNotification);

```