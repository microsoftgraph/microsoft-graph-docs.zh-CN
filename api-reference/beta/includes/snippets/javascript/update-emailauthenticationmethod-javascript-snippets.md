---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4f0afd29efc30de10aee9d6a3c2e048110893dd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806995"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const emailAuthenticationMethod = {
  emailAddress: 'kim@contoso.com'
};

await client.api('/users/kim@contoso.com/authentication/emailMethods/3ddfcfc8-9383-446f-83cc-3ab9be4be18f')
    .version('beta')
    .put(emailAuthenticationMethod);

```