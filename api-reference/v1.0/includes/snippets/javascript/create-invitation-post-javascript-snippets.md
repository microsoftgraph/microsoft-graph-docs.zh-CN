---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57ebd54b1ccfa74141c0d3fcd7f2cc56caae569e158214b71b1168fd39f1a3b2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332753"
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