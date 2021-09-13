---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 740b66e8472bd8b625e9cc1163f35726171bdab0908f99062a2f35a8dbcfe167
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105301"
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
    .update(todoTask);

```