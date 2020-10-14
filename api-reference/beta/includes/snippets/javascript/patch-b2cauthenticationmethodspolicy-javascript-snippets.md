---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44860ed5906e08b5201b5871ce0aff539ed76977
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458046"
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

let res = await client.api('/policies/b2cAuthenticationMethodsPolicy')
    .version('beta')
    .update(b2cAuthenticationMethodsPolicy);

```