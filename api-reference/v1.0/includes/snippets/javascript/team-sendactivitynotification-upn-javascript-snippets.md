---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a22c105456d237e99d39a864aba7463fc777ec30
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60691586"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sendActivityNotification = {
    topic: {
        source: 'entityUrl',
        value: 'https://graph.microsoft.com/v1.0/teams/{teamId}/channels/{channelId}/tabs/{tabId}'
    },
    activityType: 'reservationUpdated',
    previewText: {
        content: 'You have moved up the queue'
    },
    recipient: {
        '@odata.type': 'Microsoft.Teams.GraphSvc.aadUserNotificationRecipient',
        userId: 'jacob@contoso.com'
    },
    templateParameters: [
        {
            name: 'reservationId',
            value: 'TREEE433'
        },
        {
            name: 'currentSlot',
            value: '23'
        }
    ]
};

await client.api('/teams/{teamId}/sendActivityNotification')
    .post(sendActivityNotification);

```