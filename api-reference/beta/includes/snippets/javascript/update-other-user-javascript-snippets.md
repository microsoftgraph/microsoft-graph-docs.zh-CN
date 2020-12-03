---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b6a4e255ecfa649538033b3ea5e65fb2cc944d0
ms.sourcegitcommit: d09d720b56ed6f1fad556e2a3730c2e850db355f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/02/2020
ms.locfileid: "49556204"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  businessPhones: [
    "+1 425 555 0109"
  ],
  officeLocation: "18/2111"
};

let res = await client.api('/users/{id}')
    .version('beta')
    .update(user);

```