---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b941fe827b0b737a7f3b79faa493e5214f19927e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789596"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const todoTask = {
   dueDateTime: {
      dateTime: '2020-07-25T16:00:00',
      timeZone: 'Eastern Standard Time'
   }
};

await client.api('/me/todo/lists/AAMkADA1MTHgwAAA=/tasks/721a35e2-35e2-721a-e235-1a72e2351a72')
    .version('beta')
    .update(todoTask);

```