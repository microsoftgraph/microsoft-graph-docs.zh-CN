---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 48024917e0f13d874862c89094798e5128e84851083a2439721039a12a3ebc6a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378430"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authenticationMethodConfiguration = {
  '@odata.type': '#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration',
  state: 'String'
};

await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator')
    .update(authenticationMethodConfiguration);

```