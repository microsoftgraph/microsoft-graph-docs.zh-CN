---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9208f14e254008a1031b5482fb72edf21ef569de
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37995380"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onlineMeeting = {
  isBroadcast: "false",
  startDateTime:"2019-09-09T14:33:30.8546353-07:00",
  endDateTime:"2019-09-09T15:03:30.8566356-07:00",
  subject:"Application Token Meeting",
  participants: {
    organizer: {
      identity: {
        user: {
          id: "550fae72-d251-43ec-868c-373732c2704f"
        }
      }
    }
  }
};

let res = await client.api('/communications/onlineMeetings')
    .version('beta')
    .post(onlineMeeting);

```