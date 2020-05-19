---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f0c10f7a97beb9981aca0dc5bdab0c725bf5abc
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40911885"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onlineMeeting = {
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