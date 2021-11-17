---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f55f7034cc24d24374ad06a6eee88c66d79fe807d9ad9679059f70afdabe3ab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106123"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onlineMeeting = {
    startDateTime: '2020-02-06T01:49:21.3524945+00:00',
    endDateTime: '2020-02-06T02:19:21.3524945+00:00',
    subject: 'Create a meeting with customId provided',
    externalId: '7eb8263f-d0e0-4149-bb1c-1f0476083c56',
    participants: {
        attendees: [
            {
                identity: {
                    user: {
                        id: '1f35f2e6-9cab-44ad-8d5a-b74c14720000'
                    }
                },
                role: 'presenter',
                upn: 'test1@contoso.com'
            }
        ]
    }
};

await client.api('/me/onlineMeetings/createOrGet')
    .version('beta')
    .post(onlineMeeting);

```