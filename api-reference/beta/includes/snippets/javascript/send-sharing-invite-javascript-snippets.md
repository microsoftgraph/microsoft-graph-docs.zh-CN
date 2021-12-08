---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 945e075799836423b41f41cc910de589ad7f3b42
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61348794"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  recipients: [
    {
      email: 'robin@contoso.org'
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