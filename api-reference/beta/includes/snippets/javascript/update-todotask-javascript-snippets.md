---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a8187242808d44dd528d7472ddafb6e97f6a1ff
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/16/2020
ms.locfileid: "47843067"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const todoTask = {
    dueDateTime:
    {
        dateTime:"2020-07-25T16:00:00",
        timeZone:"Eastern Standard Time"
    }
};

let res = await client.api('/me/todo/lists/AAMkADA1MTHgwAAA=/tasks/721a35e2-35e2-721a-e235-1a72e2351a72')
    .version('beta')
    .update(todoTask);

```