---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 487bdd0f286692319d73b0e495b52fb81995299e
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873229"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const 721a35e2-35e2-721a-e235-1a72e2351a72 = {
    dueDateTime:
    {
        dateTime:"2020-07-25T16:00:00",
        timeZone:"Eastern Standard Time"
    }
};

let res = await client.api('/me/todo/lists/AAMkADA1MTHgwAAA=/tasks/721a35e2-35e2-721a-e235-1a72e2351a72')
    .version('beta')
    .update(721a35e2-35e2-721a-e235-1a72e2351a72);

```