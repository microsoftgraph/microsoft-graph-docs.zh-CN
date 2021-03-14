---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b78d6bea048741e3530c1def052291c0bed0d1c7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798286"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const invitation = {
  invitedUserEmailAddress: 'yyy@test.com',
  inviteRedirectUrl: 'https://myapp.contoso.com'
};

await client.api('/invitations')
    .post(invitation);

```