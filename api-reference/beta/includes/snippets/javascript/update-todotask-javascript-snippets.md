---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65394d86c69c266b531e7f1f05266b78a8e7cd40
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48375717"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const todoTask = {
   dueDateTime:{
      dateTime:"2020-07-25T16:00:00",
      timeZone:"Eastern Standard Time"
   }
};

let res = await client.api('/me/todo/lists/AAMkADA1MTHgwAAA=/tasks/721a35e2-35e2-721a-e235-1a72e2351a72')
    .version('beta')
    .update(todoTask);

```