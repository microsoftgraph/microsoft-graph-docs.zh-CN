---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ffcccf2269a01b6d63e87bbdff4f91a14a9e402c
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2019
ms.locfileid: "36636879"
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
    .update(contact);

```