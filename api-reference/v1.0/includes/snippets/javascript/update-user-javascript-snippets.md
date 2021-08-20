---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0856d9905fed8fd4838e368f8f8ad85e90ec61959829bc3357cbbd8a56d23549
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104450"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  businessPhones: [
    '+1 425 555 0109'
  ],
  officeLocation: '18/2111'
};

await client.api('/me')
    .update(user);

```