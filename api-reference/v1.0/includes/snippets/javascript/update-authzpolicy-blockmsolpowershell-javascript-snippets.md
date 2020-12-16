---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5451e2b8ca5465a191a6301c460a6fb6b7abdbee
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691406"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authorizationPolicy = {
   blockMsolPowerShell:true
};

let res = await client.api('/policies/authorizationPolicy')
    .update(authorizationPolicy);

```