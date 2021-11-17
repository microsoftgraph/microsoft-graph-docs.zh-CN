---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8bebc2ea1e97e79c7dfb090c78c535b9bc4ee23fa5aba7148d463ba51e3e491
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106124"
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