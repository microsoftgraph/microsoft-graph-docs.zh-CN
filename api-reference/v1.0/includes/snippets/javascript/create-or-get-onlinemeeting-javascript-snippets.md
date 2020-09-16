---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bedcca70660ff2d0d48b96df30a31753205c2cdf
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 09/16/2020
ms.locfileid: "47842811"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onlineMeeting = {
    startDateTime: "2020-02-06T01:49:21.3524945+00:00",
    endDateTime: "2020-02-06T02:19:21.3524945+00:00",
    subject: "Create a meeting with customId provided",
    externalId: "7eb8263f-d0e0-4149-bb1c-1f0476083c56",
    participants: {
        attendees: [
            {
                identity: {
                    user: {
                        id: "1f35f2e6-9cab-44ad-8d5a-b74c14720000"
                    }
                },
                upn: "test1@contoso.com"
            }
        ]
    }
};

let res = await client.api('/me/onlineMeetings/createOrGet')
    .post(onlineMeeting);

```