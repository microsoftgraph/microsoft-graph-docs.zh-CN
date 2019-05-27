---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 59747d0f9db174a15bdf57cbae6ec3adee872ba9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34460718"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const OnlineMeeting = {
  meetingType: "meetNow",
  participants: {
    organizer: {
      identity: {
        user: {
          id: "550fae72-d251-43ec-868c-373732c2704f"
        }
      }
    }
  },
  subject: "subject-value"
};

let res = await client.api('/app/onlineMeetings')
    .version('beta')
    .post({OnlineMeeting : OnlineMeeting});

```