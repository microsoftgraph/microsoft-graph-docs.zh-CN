---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 481efa9c9ff69832bda11ec1ecf52ba63bf62b68
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933792"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onlineMeeting = {
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
    .post({onlineMeeting : onlineMeeting});

```