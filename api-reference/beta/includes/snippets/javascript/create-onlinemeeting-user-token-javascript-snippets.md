---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 17b4ef4e8a1e86bb3de53852f80caae2266170714f7c10a76e34dc17e62e2dc3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104436"
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