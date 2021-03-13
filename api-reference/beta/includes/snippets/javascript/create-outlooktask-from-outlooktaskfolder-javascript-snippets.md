---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29d08a94a84de0be4e6c9d1a5cc6c9f39e7a69d9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774311"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookTask = {
  subject: 'Shop for dinner',
  startDateTime: {
      dateTime: '2016-04-23T18:00:00',
      timeZone: 'Pacific Standard Time'
  },
  dueDateTime: {
      dateTime: '2016-04-25T13:00:00',
      timeZone: 'Pacific Standard Time'
  }
};

await client.api('/me/outlook/taskfolders('AAMkADIyAAAhrbPXAAA=')/tasks')
    .version('beta')
    .post(outlookTask);

```