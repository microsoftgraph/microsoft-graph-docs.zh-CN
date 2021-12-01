---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65d8af47d5b5a56eae6c450941ffb005f54c4e452707d26d098fdf28e53061ff
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273905"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  recipients: [
    {
      email: 'ryan@contoso.org'
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
    .version('beta')
    .post(permission);

```