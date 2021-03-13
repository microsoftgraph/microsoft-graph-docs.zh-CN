---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1dad14ae618f9e50d9807c2b898bacd30d8a58a2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781788"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onlineMeeting = {
    chatInfo: {
        threadId: '19:7ebda77322dd4505ac4dedb5b67df076@thread.tacv2'
    },
    startDateTime: '2020-02-06T01:49:21.3524945+00:00',
    endDateTime: '2020-02-06T02:19:21.3524945+00:00',
    externalId: '7eb8263f-d0e0-4149-bb1c-1f0476083c56',
    participants: {
        attendees: [
            {
                identity: {
                    user: {
                        id: '1f35f2e6-9cab-44ad-8d5a-b74c14720000'
                    }
                },
                upn: 'test1@contoso.com'
            }
        ]
    },
    subject: 'Create a meeting with customId provided'
};

await client.api('/me/onlineMeetings/createOrGet')
    .version('beta')
    .post(onlineMeeting);

```