---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dcfb62c4cb7be23d2c832054f63230d94a3b488d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520448"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  recipients: [
    {
      email: "ryan@contoso.org"
    }
  ],
  message: "Here's the file that we're collaborating on.",
  requireSignIn: true,
  sendInvitation: true,
  roles: [ "write" ],
  password: "password123",
  expirationDateTime: "2018-07-15T14:00:00.000Z"
};

let res = await client.api('/me/drive/items/{item-id}/invite')
    .version('beta')
    .post(permission);

```