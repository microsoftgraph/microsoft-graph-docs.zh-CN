---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7bed170a4e4a481e172326459ff837d0db0175deba4cce7e64ee89e6abd7f824
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903640"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const resultInfo = {
  value: [
    'externalId-value1',
    'externalId-value2'
  ]
};

await client.api('/security/tiIndicators/deleteTiIndicatorsByExternalId')
    .version('beta')
    .post(resultInfo);

```