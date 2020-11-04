---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 356f69e400c82273433fa24fbc9979c3790085c3
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48907334"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const emailAuthenticationMethod = {
  emailAddress: "kim@contoso.com"
};

let res = await client.api('/users/kim@contoso.com/authentication/emailMethods/3ddfcfc8-9383-446f-83cc-3ab9be4be18f')
    .version('beta')
    .put(emailAuthenticationMethod);

```