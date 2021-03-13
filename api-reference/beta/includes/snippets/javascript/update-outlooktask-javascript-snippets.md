---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 118047153e2f415bdcb16bc66c562cbf76c84c1c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808577"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookTask = {
  dueDateTime: {
      dateTime: '2016-05-06T16:00:00',
      timeZone: 'Eastern Standard Time'
  }
};

await client.api('/me/outlook/tasks/AAMkADA1MTHgwAAA=')
    .version('beta')
    .update(outlookTask);

```