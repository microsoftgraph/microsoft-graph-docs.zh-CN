---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6107dbf984833ff537622240c966a65c064ca99
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473046"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authenticationMethodConfiguration = {
  @odata.type: "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration",
  state: "String"
};

let res = await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator')
    .version('beta')
    .update(authenticationMethodConfiguration);

```