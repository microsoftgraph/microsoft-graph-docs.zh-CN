---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a86cdeeff9a716ba3c02f1db364381923733f16656bb75154333f768013f582
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328798"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const emailAuthenticationMethod = {
  emailAddress: 'kim@contoso.com'
};

await client.api('/users/kim@contoso.com/authentication/emailMethods')
    .version('beta')
    .post(emailAuthenticationMethod);

```