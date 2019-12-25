---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eaaa70fb83e0685fc436de1d35980cec803b7071
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865864"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onlineMeeting = {
  startDateTime:"2019-07-12T14:30:34.2444915-07:00",
  endDateTime:"2019-07-12T15:00:34.2464912-07:00",
  subject:"User Token Meeting"
};

let res = await client.api('/me/onlineMeetings')
    .post(onlineMeeting);

```