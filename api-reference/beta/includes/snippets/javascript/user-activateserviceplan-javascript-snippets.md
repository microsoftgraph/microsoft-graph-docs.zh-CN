---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f0b2bd3b478f8ccb7576f2bef20c27790b3111689fb40dd58a0c652febe38209
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333380"
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