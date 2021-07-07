---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a40dc6692fb3373c6ac07ceb4c31d4fb1fea0694
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317126"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sendActivityNotification = {
    topic: {
        source: 'entityUrl',
        value: 'https://graph.microsoft.com/beta/teams/e8bece96-d393-4b9b-b8da-69cedef1a7e7'
    },
    activityType: 'pendingFinanceApprovalRequests',
    previewText: {
        content: 'Internal spending team has a pending finance approval requests'
    },
    recipient: {
        '@odata.type': 'microsoft.graph.channelMembersNotificationRecipient',
        teamId: 'e8bece96-d393-4b9b-b8da-69cedef1a7e7',
        channelId: '19:3d61a2309f094f4a9310b20f1db37520@thread.tacv2'
    },
    templateParameters: [
        {
            name: 'pendingRequestCount',
            value: '5'
        }
    ] 
};

await client.api('/teams/e8bece96-d393-4b9b-b8da-69cedef1a7e7/sendActivityNotification')
    .version('beta')
    .post(sendActivityNotification);

```