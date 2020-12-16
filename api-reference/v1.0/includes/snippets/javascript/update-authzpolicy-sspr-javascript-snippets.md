---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c71a0b890d4d132c800c8a8172b07d557c2ae315
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691414"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authorizationPolicy = {
   allowedToUseSSPR:true
};

let res = await client.api('/policies/authorizationPolicy')
    .update(authorizationPolicy);

```