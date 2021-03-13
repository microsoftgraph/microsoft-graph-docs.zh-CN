---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8012a36a69236870e86b96f97337d226d1620da3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810182"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const b2cAuthenticationMethodsPolicy = {
    isEmailPasswordAuthenticationEnabled: false,
    isUserNameAuthenticationEnabled: true
};

await client.api('/policies/b2cAuthenticationMethodsPolicy')
    .version('beta')
    .update(b2cAuthenticationMethodsPolicy);

```