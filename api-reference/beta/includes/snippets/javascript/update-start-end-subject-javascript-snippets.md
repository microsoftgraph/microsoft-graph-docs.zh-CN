---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8bd9fc6363977b55b99d8e5192d7fb66e3fb0e22
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775645"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onlineMeeting = {
  startDateTime: '2020-09-09T14:33:30.8546353-07:00',
  endDateTime: '2020-09-09T15:03:30.8566356-07:00',
  subject: 'Patch Meeting Subject'
};

await client.api('/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi')
    .version('beta')
    .update(onlineMeeting);

```