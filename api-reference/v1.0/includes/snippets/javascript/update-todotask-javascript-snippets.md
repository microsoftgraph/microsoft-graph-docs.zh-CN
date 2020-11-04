---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1083e20ce397dd4e7ea0f2fe1f88b9db96712fda
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905323"
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
    .update(todoTask);

```