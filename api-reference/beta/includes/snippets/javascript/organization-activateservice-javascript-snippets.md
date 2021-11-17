---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5fc4b17990e0fda427cf574a0a98cac4eefeb60a7358c2edb433ef055040afc7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333145"
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