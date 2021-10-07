---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eea22c90c13e901bf3f868fbdcd0526565863f62cb7a1e3a7772694f35eff133
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378618"
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