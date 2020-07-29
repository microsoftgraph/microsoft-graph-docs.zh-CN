---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e6319a1ed12f00369e2861852e8c17eeea1e421
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46512299"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onlineMeeting = {
  startDateTime: "2020-09-09T14:33:30.8546353-07:00",
  endDateTime: "2020-09-09T15:03:30.8566356-07:00",
  subject: "Patch Meeting Subject"
};

let res = await client.api('/me/onlineMeetings/{id}')
    .version('beta')
    .update(onlineMeeting);

```