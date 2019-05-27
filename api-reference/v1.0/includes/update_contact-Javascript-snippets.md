---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 16c1afc802e1b96ee7fa595fae16aa5f562b38d8
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34475762"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contact = {
  homeAddress: {
    street: "123 Some street",
    city: "Seattle",
    state: "WA",
    postalCode: "98121"
  },
  birthday: "1974-07-22"
};

let res = await client.api('/me/contacts/{id}')
    .update({contact : contact});

```