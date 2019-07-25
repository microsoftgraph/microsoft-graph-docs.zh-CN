---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 083f6c8c50c88aa2c1000d5c23613601a6c7c08e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734432"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  recipients: [
    {
      email: "ryan@contoso.com"
    }
  ],
  message: "Here's the file that we're collaborating on.",
  requireSignIn: true,
  sendInvitation: true,
  roles: [ "write" ]
};

let res = await client.api('/me/drive/items/{item-id}/invite')
    .post(permission);

```