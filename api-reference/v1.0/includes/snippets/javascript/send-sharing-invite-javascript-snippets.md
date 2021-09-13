---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 257454bfd181d3190f2a8e2b0b0e861c972cebc01a575211511929a6ed62ae78
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904136"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  recipients: [
    {
      email: 'ryan@contoso.com'
    }
  ],
  message: 'Here\'s the file that we\'re collaborating on.',
  requireSignIn: true,
  sendInvitation: true,
  roles: [ 'write' ],
  password: 'password123',
  expirationDateTime: '2018-07-15T14:00:00.000Z'
};

await client.api('/me/drive/items/{item-id}/invite')
    .post(permission);

```