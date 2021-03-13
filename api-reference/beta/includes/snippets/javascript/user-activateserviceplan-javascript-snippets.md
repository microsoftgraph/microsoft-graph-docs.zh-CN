---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5939bdbba9a9806d5b8b229047854374ad6267eb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775041"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const activateServicePlan = {
  servicePlanId: '28f42d6f-8034-4a0f-9d8a-a218a63b3299',
  skuId: '465a2a90-5e59-456d-a7b8-127b9fb2e484'
};

await client.api('/me/activateServicePlan')
    .version('beta')
    .post(activateServicePlan);

```