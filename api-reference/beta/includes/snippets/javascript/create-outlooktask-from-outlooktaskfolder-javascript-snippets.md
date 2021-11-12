---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0709a5ad56822a5f2d77bc1d325ff13ced83b2d583f464b3cf1d96569038c55a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163392"
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