---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 569092490589d665babf74e3d2c8cc09d47c28a9420fdd6bdeeef113ca239f01
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279563"
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