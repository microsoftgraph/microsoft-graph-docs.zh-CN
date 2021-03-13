---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 661128933d718e98ea6d66677bc0dfc6efd9ff66
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800573"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onlineMeeting = {
  startDateTime: '2019-07-12T14:30:34.2444915-07:00',
  endDateTime: '2019-07-12T15:00:34.2464912-07:00',
  subject: 'User Token Meeting'
};

await client.api('/me/onlineMeetings')
    .version('beta')
    .post(onlineMeeting);

```