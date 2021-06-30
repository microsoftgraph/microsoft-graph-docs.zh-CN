---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d287a1b05cbf6b80a392dd89e38fd9618c4b79d
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207668"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const activateService = {
    skuId: '6fd2c87f-b296-42f0-b197-1e91e994b900',
    servicePlanId: 'a23b959c-7ce8-4e57-9140-b90eb88a9e97'
};

await client.api('/organization/{:organizationId}/activateService')
    .version('beta')
    .post(activateService);

```