---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ea5008e387f7918712d391780d5b9b571f7f024
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42589890"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tokenLifetimePolicy = {
  @odata.id:"https://graph.microsoft.com/beta/policies/tokenLifetimePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
};

let res = await client.api('/applications/{id}/tokenLifetimePolicies')
    .version('beta')
    .post(tokenLifetimePolicy);

```