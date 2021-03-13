---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a99f23b2ab35eef90036849add00a2224abf6914
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800441"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authenticationMethodConfiguration = {
    '@odata.type': '#microsoft.graph.smsAuthenticationMethodConfiguration',
    id: 'Sms',
    state: 'enabled'
};

await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/sms')
    .version('beta')
    .update(authenticationMethodConfiguration);

```