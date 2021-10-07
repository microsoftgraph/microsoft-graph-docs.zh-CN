---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a1034d26a883cb5a6f76c985fb3607cb95ee92ecf559584b517d3e07dad99c4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161193"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authenticationMethodConfiguration = {
    '@odata.type': '#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration',
    state: 'enabled'
};

await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator')
    .version('beta')
    .update(authenticationMethodConfiguration);

```